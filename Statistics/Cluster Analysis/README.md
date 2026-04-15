from numpy.random import RandomState
from sklearn.cluster import KMeans
from sklearn.preprocessing import StandardScaler

condition = ['Acute upper respiratory infection','Bronchiolitis', 'Bronchitis',
    'Pneumonia', 'Croup', 'Sinus infection',
    'Sore throat (including strep throat)', 'Tonsillitis']

X = df_age[condition]

scaler = StandardScaler()
X_scaled = scaler.fit_transform(X)

# Initialize and fit the model:
kmeans = KMeans(n_clusters=3, random_state=43)
kmeans.fit(X_scaled)

df_age['Cluster'] = kmeans.fit_predict(X_scaled)

# Print the results:
print(df_age[['age_group', 'Cluster']])
