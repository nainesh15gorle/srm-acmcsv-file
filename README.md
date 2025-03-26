import pandas as pd

a. Loading Data
file_path = "/content/tested.csv" # Change this to your actual file path df = pd.read_csv(file_path)

b. Data Inspection
print("First 5 rows of the dataset:") print(df.head()) print("\nSummary statistics:") print(df.describe()) print("\nMissing values in each column:") print(df.isnull().sum())

c. Data Selection (Selecting specific columns)
selected_columns = ['Age', 'Name'] # Change to actual column names df_selected = df[selected_columns]

d. Filtering (Filtering rows based on a condition)
filtered_df = df[df['Age'] > 35] # Modify condition as needed

e. Handling Missing Data
df_cleaned = df.dropna() # Removes rows with missing values

Alternatively, fill missing values
df_filled = df.fillna(df.mean()) # Replace NaN with column means

Display results
print("\nSelected Data:") print(df_selected.head())

print("\nFiltered Data:") print(filtered_df.head())

print("\nCleaned Data:") print(df_cleaned.head())import pandas as pd
