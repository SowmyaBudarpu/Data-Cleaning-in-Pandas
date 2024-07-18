# Data Cleaning and Exploratory Data Analysis (EDA)

Data cleaning and EDA are essential steps in any data analysis process. Clean data ensures accurate and reliable analysis, while EDA provides insights and understanding of the data's underlying structure. Use these steps and techniques to effectively clean your data and perform exploratory analysis.

## Data Cleaning

Data cleaning is the process of preparing raw data for analysis by removing or correcting errors, inconsistencies, and inaccuracies. Below are the key steps involved in data cleaning:

1. **Remove Duplicate Data:**
   - Identify and remove duplicate rows to ensure each record is unique.
   - Use functions like `drop_duplicates()` in pandas.

2. **Handle Missing Values:**
   - Identify missing values using functions like `isnull()` or `isna()`.
   - Decide on a strategy to handle missing values: remove, fill with a specific value, or use imputation methods.
   - Use functions like `fillna()`, `dropna()`, or imputation libraries.

3. **Correct Inconsistencies:**
   - Standardize data formats (e.g., date formats).
   - Correct inconsistent data entries (e.g., 'USA', 'U.S.A.', 'United States' should be standardized to 'USA').

4. **Filter Out Irrelevant Data:**
   - Remove columns or rows that are not relevant to the analysis.
   - Use filtering techniques based on specific conditions.

5. **Outlier Detection and Treatment:**
   - Identify outliers using statistical methods or visualization techniques.
   - Decide on a treatment method: remove, cap, or transform.

6. **Convert Data Types:**
   - Ensure each column has the correct data type (e.g., integers, floats, strings, dates).
   - Use functions like `astype()` in pandas for type conversion.

7. **Text Data Cleaning:**
   - Remove special characters, stop words, and perform text normalization for text data.

## Exploratory Data Analysis (EDA)

EDA is the process of analyzing data sets to summarize their main characteristics, often using visual methods. It helps in understanding the data, detecting patterns, and forming hypotheses.

### Filtering and Ordering

1. **Filtering Data:**
   - Apply conditions to filter rows and columns relevant to the analysis.
   - Use logical operators and pandas functions like `query()`, `loc[]`, and `iloc[]`.
   - Example: `df_filtered = df[df['age'] > 25]`

2. **Ordering Data:**
   - Sort data to identify trends and patterns.
   - Use functions like `sort_values()` to order data based on one or more columns.
   - Example: `df_sorted = df.sort_values(by=['age'], ascending=True)`

### Group By and Aggregating

1. **Grouping Data:**
   - Group data by one or more categorical columns to perform aggregate operations.
   - Use the `groupby()` function in pandas.
   - Example: `grouped_df = df.groupby('category')`

2. **Aggregating Data:**
   - Apply aggregate functions (e.g., `sum()`, `mean()`, `count()`) on grouped data.
   - Use methods like `agg()`, `transform()`, and aggregate functions.
   - Example: `aggregated_df = grouped_df.agg({'sales': 'sum', 'profit': 'mean'})`
  



