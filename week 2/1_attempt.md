Assignment 2

Initial Code
import pandas as pd
df_raw = pd.read_csv('teaching_prices_messy.csv')
print("--- Data Info ---")
df_raw.info()
print(df_raw.head(10))
print("\n--- Missing Values ---")
print(df_raw.isnull().sum())
print("\n--- Statistics ---")
print(df_raw.describe(include='all'))


Problem Diagnosis & Planned Decisions


Problem 1: Inconsistent Data formatting

Column(s) Affected: item

Code Used:
print(df_raw['item_name'].unique())
print(df_raw['item_name'].value_counts(dropna=False))

Planned Decision: Correct

Problem 2: Missing Values

Column(s) Affected: price
Code Used: 
print(df_raw[df_raw['price'].isna()])

Planned Decision: Flag 


Problem 4: Duplicate Records

Column(s) Affected: Entire Rows

Code Used:
print("Duplicate rows count:", df_raw.duplicated().sum())
print(df_raw[df_raw.duplicated(keep=False)])


Planned Decision:  Exclude

Problem 5: Incorrect Data Types

Column(s) Affected: price stored as string

Code Used:
print(df_raw.dtypes)


Planned Decision: Correct

