# Finance Mortgage Loan Analysis: Microsoft Power BI Implementation

## Introduction

This README provides comprehensive details on the analysis questions, visualizations, and analyses conducted for the finance-mortgage-loan dataset, focusing on Microsoft Power BI implementation.

## 1. Detail of the Data Set

The dataset used is "Finance-Mortgage_Loan_Application.xlsx," which contains information related to mortgage loan applications.

- **Size**: 700 KB

The dataset is organized into several sheets, each providing specific information:

### a. Borrower Sheet

- **Description**: Contains details about the borrowers, including personal information, contact details, and demographics.
- **Number of Rows**: 2000
- **Number of Columns**: 15
  - Key columns: Borrower Key, SSN (Social Security Number), First Name, Last Name, Email, Phone, Cell Phone, Marital Status, DOB (Date of Birth), Address, State, Zip, Sex, Ethnicity, Race

### b. Loan Sheet

- **Description**: Includes details about the loan type, purpose, co-borrower information, and other loan-specific details.
- **Number of Rows**: 2000
- **Number of Columns**: 9
  - Key columns: Loan Key, Loan ID, Property ID, Property Usage, Purpose of Loan, Credit Card Authorization, Co-Borrower SSN, Rent or Own, Loan Date

### c. Property Sheet

- **Description**: Contains information about properties related to the mortgage loans, including location and real estate agent details.
- **Number of Rows**: 2000
- **Number of Columns**: 8
  - Key columns: Property Key, Property ID, Property City, Property State, Property Zip, Real Estate Agent Name, Real Estate Agent Phone, Real Estate Agent Email

### d. Financials Sheet

- **Description**: Provides financial information such as income, assets, and liabilities related to the borrowers and their mortgage applications.
- **Number of Rows**: 2000
- **Number of Columns**: 16
  - Key columns: Financial Key, Borrower Key, Property Key, Loan Key, Years at Address, Loan Amount, Purchase Price, Number of Units, Monthly Income, Bonuses, Commission, Other Income, Checking, Savings, Retirement Fund, Mutual Fund

## 2. Data Model and DAXs

### a. Transform Data

The dataset was transformed to ensure relevance and consistency for analysis. Essential transformations were made, including:

- **Borrower Sheet**: Promoted headers and changed data types.
- **Loan Sheet**: Promoted headers and changed data types.
- **Property Sheet**: Promoted headers, changed types, inserted a merged column (city and state), and renamed columns.

### b. Data Model

The data model in Power BI integrates and establishes relationships between tables. Details are provided in the Power BI project files.

### c. DAXs

A range of DAX calculations were performed, including:

- Calculating the borrower's age and categorizing into groups.
- Calculating the total loan amount across all states and for each state.
- Computing the percentage of the loan amount for each state and age group.
- Counting credit approvals to identify trends.

## 3. Visualization and Analyses

### Dashboard 1

Provides an overview of mortgage lending in the US for 2019, including:

- **Question 1**: Top 5 states with the highest total loan amounts in 2019.
  - **Answer**: California, New York, Pennsylvania, Michigan, and Kentucky had the highest loan amounts. California alone accounted for 6.95% of the total loan amount.

- **Question 2**: Age group with the highest total loan amount.
  - **Answer**: Individuals over 55 years old had the highest total loan amount, totaling nearly 460 million USD (43.32% of the total loan amount).

- **Question 3**: Differences in mortgage lending based on marital status and gender.
  - **Answer**: Married couples had higher loan amounts, with females having higher loan amounts compared to males.

### Dashboard 2

Analyzes trends and relationships between loan amounts and monthly income, categorized by age, marital status, race, and gender.

- **Question 4**: Relationship between loan amounts and monthly income by gender.
  - **Answer**: Higher monthly income correlates with higher loan approvals, indicating the importance of financial stability in securing larger loans.

### Dashboard 3

Displays loan amount by state and age breakdown, percentage of loan amount by marital status, and the number of credit approvals by loan purpose.

- **Question 5**: Effect of loan purpose on credit approval.
  - **Answer**: Loans with the 'Purchase' purpose had the highest number of credit approvals, particularly for primary residence purchases.

### Dashboard 4

Shows loan details based on property usage in various states and highlights areas with high loan amounts.

- **Question 6**: Top 5 cities for investment property loans.
  - **Answer**: California, Pennsylvania, New York, Kentucky, and Iowa were the top cities for investment property loans.

- **Question 7**: Distribution of loans by property usage.
  - **Answer**: Most loans are for primary residences, followed by investment properties, with second homes having the smallest share.

### Dashboard 5

Displays the relationship between purchase price and monthly income over 2019 and features a multi-row card showing loan amounts by age and marital status.

- **Question 8**: Influence of total monthly income on home purchases.
  - **Answer**: Higher monthly income leads to higher home purchase investments, underscoring the importance of financial capability in purchasing decisions.

### Dashboard 6

Contains Q&A sections for interacting with the reports using natural language queries.
