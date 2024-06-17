# Credit Risk Analytics

## Problem Statement
This project focuses on Exploratory Data Analysis (EDA) in credit risk analytics for a consumer finance company. The main goals are to:
- Identify patterns and key variables that predict loan default.
- Inform better decision-making in loan approvals, risk reduction, and portfolio optimization.
- Provide concise and informative results to support informed choices in credit risk analytics.

## Introduction

### Understanding the Challenge
Lending institutions face a significant challenge in discerning between loan applicants capable of responsible repayment and those at risk of default. The absence of robust credit histories among certain applicants necessitates precise risk assessment procedures. This challenge not only affects financial stability but also leads to missed business opportunities for lending companies.

### The Imperative of Risk Assessment
Risk analytics, a pivotal facet of modern financial services, is instrumental in navigating the intricate landscape of lending. It facilitates the data-driven decision-making process essential for minimizing financial risks and optimizing loan portfolios.

## Steps Included in the Project
1. Data Understanding
2. Missing Data Handling
3. Outlier Identification
4. Data Imbalance Analysis
5. Univariate Analysis
6. Segmented Univariate Analysis
7. Bivariate Analysis
8. Correlation Analysis

## 1. Data Understanding
### Datasets
1. **Application_data**: Contains all the information of the client at the time of application.
   - Data Structure: (307511 rows, 122 columns)
   - No. of Categorical Variables: 16
   - No. of Numerical Variables: 106
   - Target/Output Variable: TARGET

2. **Previous_application**: Contains information about the client’s previous loan data.
   - Data Structure: (1048575 rows, 37 columns)
   - No. of Categorical Variables: 16
   - No. of Numerical Variables: 21
   - Target/Output Variable: NAME_CONTRACT_STATUS

## 2. Missing Data Handling
### Merging the Data
- Identified common columns between the two datasets.
- Merged the datasets using the "SK_ID_CURR" column via a left join.

### Handling the Missing Data
- Columns with over 60% missing data are dropped.
- Numeric columns with 0% to 60% missing data are imputed with the mean.
- Categorical columns with below 40% missing data are imputed with the mode.
- Created special categories for columns with missing values greater than the mode.

## 3. Outlier Handling
- Calculated the correlation matrix.
- Used log transform for positive numeric columns to handle outliers.
- Investigated columns with numeric values exclusively between 0 and 1.
- Examined categorical columns and checked the number of unique values in each.

## 4. Data Imbalance Ratio
- Separated the dataset into "Target0" (repayers) and "Target1" (defaulters).
- Calculated the imbalance ratio.

## 5. Univariate Analysis
Analyzed categorical and numerical variables to find insights:

## 6. Segmented Univariate Analysis
Examined the relationship between the target variable and different segments:

## 7. Bivariate Analysis
Explored the relationships between numerical attributes and the target variable:

## 8. Correlation Analysis
Calculated the correlation of all attributes with the 'TARGET' variable:

## Key Findings
- 9% of total applicants are defaulters and 91% are non-defaulters.
- Female applicants are more likely to repay the loan.
- Majority applied for cash loans.
- Higher credit amounts correlate with increased defaulters.
- Lower income correlates with higher default rates.

This project provides valuable insights into credit risk analytics, aiding in better decision-making and risk management in the consumer finance sector.
