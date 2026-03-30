**NAME: ANSH PRATAP SINGH**

**PRN: 25070123143**

**AIM: To study and perform data preprocessing techniques in Python using Pandas, specifically to identify, analyze, and handle missing values in a dataset**

----------------------------------------------------------------------------------------------------------------------------------------------------------------------

**THEORY**

Data Preprocessing and Handling Missing Values using Pandas

Data preprocessing is one of the most important steps in data analysis and machine learning. Raw data collected from different sources is often incomplete, inconsistent, noisy, or contains missing values. Before performing analysis, the data must be cleaned and transformed into a structured format.

Missing values occur when no data value is stored for a variable in an observation. In Python, missing values are generally represented using NaN (Not a Number). These missing values can affect statistical calculations, machine learning models, and visualization results. Therefore, identifying and handling missing data is an essential part of preprocessing.

The Pandas library in Python provides powerful tools for data manipulation and preprocessing. It offers various functions to detect, remove, or replace missing values efficiently.

In this experiment, a DataFrame is created using Pandas. The DataFrame consists of columns and rows similar to a table in a spreadsheet. Some entries intentionally contain missing values (NaN) to demonstrate different preprocessing techniques.

The first step in preprocessing is detecting missing values using functions such as isna() or isnull(). These functions return a Boolean DataFrame indicating whether a value is missing.

Once missing values are identified, different strategies can be used to handle them:

1)- Removing missing values:- 

Rows or columns containing missing data can be removed using the dropna() function.

2)- Replacing missing values:- 

Missing values can be replaced with a constant value, mean, median, or other statistical measures using the fillna() function.

3)- Data cleaning:-

Sometimes missing values are represented using symbols such as " - " or empty strings. These values must be replaced with NaN using the replace() function so that Pandas can recognize them as missing values.

4)- Data type conversion:-

Columns containing numerical values stored as strings must be converted into numeric format using pd.to_numeric().

5)- Standardizing text data

Inconsistent text formats such as "cse" and "CSE" must be standardized using string functions.

6)- Date conversion:-

Dates stored as strings can be converted into proper datetime format using pd.to_datetime() for better analysis.

Through these preprocessing techniques, the dataset becomes clean, consistent, and ready for analysis or machine learning models.

Thus, data preprocessing improves data quality, reliability, and accuracy of analytical results.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Explanation of Each Function**

1. **np.nan**:- It represents missing or undefined numerical values in NumPy and Pandas.

Purpose:- Marks missing data in datasets and it helps Pandas detect and process missing values.

2. **isna()**:- This function checks whether each element in the DataFrame is missing (NaN).

Output:- Returns True if the value is missing and False otherwise.

3. **notna()**:- This function is the opposite of isna(). It checks whether values are not missing.

Purpose:- Identifies valid data entries.

4. **isna().sum()**:- This function counts the number of missing values in each column.

Purpose:- Helps determine how many values are missing in each column.

5. **isna().sum(axis=1)**:- This counts missing values row-wise.

Purpose:- Identifies rows that contain missing data.

6. **dropna()**:- This function removes rows that contain missing values.

Purpose: Removes incomplete records from the dataset.

7. **dropna(axis=1)**:- Removes columns that contain missing values.

Purpose:- Used when entire columns contain too many missing values.

8. **fillna()**:- This function replaces missing values with a specified value.

Purpose:- Fills missing data with a constant or calculated value.

9. **replace()**:- This function replaces specific values in the dataset.

Purpose:- Converts symbols like "-" into NaN so they can be processed as missing values.

10. **pd.to_numeric()**:- Converts values into numeric format.

Purpose:- Converts strings to numbers and Invalid values are converted to NaN.

11. **str.upper()**:- Converts all text to uppercase.

Purpose:- Fixes inconsistent text formatting such as cse and CSE.

12. **pd.to_datetime()**:- Converts string values into datetime format.

Purpose:- Standardizes date formats for analysis.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**CONCLUSION**

This experiment demonstrated various data preprocessing techniques using the Pandas library. Missing values were identified using functions like isna() and notna(), and handled using methods such as dropna() and fillna(). Data cleaning techniques such as replacing incorrect values, converting data types, and standardizing text formats were also applied. These preprocessing steps ensure that the dataset becomes clean, consistent, and suitable for further analysis or machine learning applications.
