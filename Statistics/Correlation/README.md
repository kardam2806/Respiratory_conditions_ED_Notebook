corr_matrix = df_matrix.corr()

# Plotting the correlation matrix:
plt.figure(figsize=(8, 8))
sns.heatmap(corr_matrix, annot=True, cmap='coolwarm', fmt=".2f", center=0)
plt.title('Correlation Between Different Respiratory Conditions')
plt.xlabel('Respiratory Conditions', fontsize=12)
plt.ylabel('Respiratory Conditions', fontsize=12)
plt.xticks(rotation=90)
plt.yticks(rotation=0)
plt.show()
