# new-repo
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Step 1: Load the data
df = pd.read_csv('your_dataset.csv')  # or .xlsx using pd.read_excel()

# Step 2: Create a correlation matrix (common for heatmaps)
corr_matrix = df.corr()

# Step 3: Plot the heatmap
plt.figure(figsize=(10, 8))
sns.heatmap(corr_matrix, annot=True, cmap='coolwarm', linewidths=0.5)
plt.title("Heatmap of Correlation Matrix")
plt.show()
