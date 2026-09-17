# Loan Approval Dataset - Data Cleaning and EDA

## Project Overview

This project focuses on performing **Data Cleaning** and **Exploratory Data Analysis (EDA)** on a Loan Approval dataset using Python.

The main goal of this project is to understand the dataset, clean missing and inconsistent values, analyze important features, detect outliers, and generate useful insights before building a machine learning model.

This project is part of my Machine Learning and Data Science learning journey.

---

## Dataset Description

The dataset contains information about loan applicants, including personal, financial, and loan-related details.

Some of the important columns include:

- Gender
- Married status
- Dependents
- Education
- Self employed status
- Applicant income
- Coapplicant income
- Loan amount
- Loan amount term
- Credit history
- Property area
- Loan status

The target column is:

- `loan_status` - whether the loan was approved or not

---

## Tools and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Project Structure

```text
loan-approval-data-cleaning-eda/
│
├── data/
│   ├── raw/
│   │   └── train.csv
│   │
│   └── processed/
│       └── cleaned_loan_train.csv
│
├── images/
│   ├── loan_status_count.png
│   ├── education_vs_loan_status.png
│   ├── total_income_vs_loan_amount.png
│   └── correlation_heatmap.png
│
├── notebooks/
│   └── loan_approval_data_cleaning_eda.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
Steps Performed
1. Data Loading

Loaded the loan approval dataset using Pandas and performed an initial inspection of the data.

2. Basic Data Understanding

Checked:

Number of rows and columns
Column names
Data types
Summary statistics
First few records
3. Missing Value Analysis

Identified missing values in the dataset and handled them using suitable methods:

Categorical missing values were filled using mode
Numerical missing values were filled using median
4. Duplicate Check

Checked for duplicate records and handled them if present.

5. Categorical Data Cleaning

Cleaned categorical columns by removing extra spaces and checking unique values.

6. Feature Engineering

Created a new feature:

total_income = applicant_income + coapplicant_income

This helps in understanding the combined financial strength of the applicant.

7. Outlier Detection

Used boxplots to detect outliers in numerical columns such as:

Applicant income
Coapplicant income
Loan amount
8. Exploratory Data Analysis

Performed visual analysis using:

Count plots
Histograms
Boxplots
Scatter plots
Correlation heatmap
9. Correlation Analysis

Created a correlation heatmap to understand the relationship between numerical features.

Key Insights
The dataset contains both numerical and categorical features.
Missing values were present in multiple columns and were handled properly.
Applicant income and loan amount contain high-value outliers.
Loan approval is not dependent on income alone.
Credit history appears to be an important factor in loan approval.
Most loan amounts are concentrated in a moderate range, while a few applicants requested very high loan amounts.
A new feature called total_income was created to improve analysis.
The cleaned dataset is ready for machine learning model building.
Sample Visualizations
Loan Approval Status Count

Education vs Loan Status

Total Income vs Loan Amount

Correlation Heatmap

How to Run This Project
1. Clone the repository
git clone https://github.com/Kangs-build/loan-approval-data-cleaning-eda.git
2. Install required libraries
pip install -r requirements.txt
3. Open the Jupyter Notebook
jupyter notebook

Then open:

notebooks/loan_approval_data_cleaning_eda.ipynb
Project Status

Data Cleaning and Exploratory Data Analysis completed.

Next step:

Build a machine learning model to predict loan approval status.
Author

Kanaga Sundaram B
B.E. Computer Science and Engineering Student
Interested in Machine Learning, Data Science, and AI-based applications.

GitHub: Kangs-build
