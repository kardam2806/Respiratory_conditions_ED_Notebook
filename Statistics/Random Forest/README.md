import pandas as pd
from sklearn.ensemble import RandomForestRegressor
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import LabelEncoder
import matplotlib.pyplot as plt
import seaborn as sns

# Prepare the data:
df_rf = df_anova.copy()

# Label encoding:
le_age = LabelEncoder()
le_cond = LabelEncoder()

df_rf['age_group_encoded'] = le_age.fit_transform(df_rf['age_group'])
df_rf['Condition_encoded'] = le_cond.fit_transform(df_rf['Condition'])

# Define Features (X) and Target (y)
X = df_rf[['age_group_encoded', 'Condition_encoded']]
y = df_rf['Average_ED_visits']

# Split into Training and Testing sets (80% train, 20% test)
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)


# Build and Train the Random Forest
# n_estimators=100 means we are using 100 decision trees
rf_model = RandomForestRegressor(n_estimators=100, random_state=42)
rf_model.fit(X_train, y_train)


# Check Feature Importance
# This tells us which factor was the most "predictive"
importances = rf_model.feature_importances_
feature_names = X.columns
feature_importance_df = pd.DataFrame({'Feature': feature_names, 'Importance': importances}).sort_values(by='Importance', ascending=False)


# Visualize Feature Importance
plt.figure(figsize=(10, 6))
sns.barplot(x='Importance', y='Feature', data=feature_importance_df, palette='viridis')
plt.title('Feature Importance from Random Forest', fontsize=14)
plt.xlabel('Importance', fontsize=14)
plt.ylabel('Feature', fontsize=14)
plt.xticks(fontsize=14)
plt.yticks(fontsize=14)
plt.title('Which Factors Drive ED Visits? (Random Forest Feature Importance)', fontsize=14)
plt.show()

print(feature_importance_df)
