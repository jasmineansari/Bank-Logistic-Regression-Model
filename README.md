# Bank-Logistic-Regression-Model
Overhauled the data landscape through a judicious blend of cleansing, exploratory data analysis, and outlier mitigation. Implemented  advanced feature selection techniques, deftly addressing multicollinearity. Culminated in a logistic regression model boasting a  commendable accuracy level of 0.92.

## Overview
The provided file is a Jupyter Notebook that performs a logistic regression analysis on a bank customer dataset. The goal is to build a classification model that can predict whether a customer will choose a new service offered by the bank (e.g. loan, mortgage, etc.).

## Data Exploration
1. The dataset contains information about 41,195 bank customers, including features such as age, job, marital status, education, default status, housing loan, personal loan, contact type, and more. [1]
2. The target variable 'y' is a binary classification indicating whether the customer subscribed to the new service (yes/no). [1]
3. The dataset has 21 columns and 41,195 rows. There are 76 missing values across the dataset. [1]
4. The data is checked for duplicates, and 11 duplicate rows are removed. 

## Data Preprocessing
1. The missing values are handled by dropping the rows with any missing data. 
2. The categorical features are encoded using appropriate methods (e.g. one-hot encoding). 
3. The data is split into training and testing sets. 

## Model Building
1. A logistic regression model is built using the preprocessed data. 
2. The model is trained on the training set and evaluated on the testing set. 
3. The model's performance metrics, such as accuracy, precision, recall, and F1-score, are calculated.

## Code Overview:
1. **Importing Libraries:** The code starts by importing necessary libraries such as NumPy, Pandas, Matplotlib, and Seaborn.
2. **Loading the Dataset:** The dataset "bank-additional-full_final (1).csv" is loaded into a Pandas DataFrame named 'df' using the `pd.read_csv()` function.
3. **Data Exploration:**
   - The code displays the first few rows of the dataset to provide an overview of the data structure.
   - It then uses `df.info()` to show information about the dataset, including the number of non-null values and data types of each column.
   - The code further checks for missing values in each column using `df.isnull().sum()` to identify any data cleaning requirements.

## Key Points:
- The dataset contains 41,199 entries and 21 columns, including features like age, job, marital status, education, contact type, and more.
- Data cleaning steps are performed to handle missing values in the dataset.
- The code provides insights into the distribution of missing values across different columns.

## Conclusion:
The code in the Jupyter Notebook sets the foundation for a logistic regression analysis on the bank customer dataset by loading the data, exploring its structure, and identifying potential data cleaning tasks. Further steps would involve preprocessing the data, building a logistic regression model, training it, and evaluating its performance for predicting customer behavior related to a new service offered by the bank.
