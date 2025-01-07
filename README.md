# **Explainable AI Part 1: Data Preparation and Machine Learning**

## Overview

Loan default prediction is a critical application in the financial industry, where lenders and institutions aim to assess the risk associated with providing loans to individuals or businesses. 
The goal is to identify potential borrowers more likely to default on their loans, allowing lenders to make informed decisions and mitigate financial risks.

 In the context of loan default prediction, machine learning models have shown
 promising results in accurately predicting whether a borrower will default on a loan.
 These models leverage historical data, such as past loan performance, financial history,
 employment details, and other relevant factors, to predict the likelihood of future loan
 defaults.

 ## Aim
 
 This project aims to predict loan defaults using machine learning models (XGBoost and
 Random Forest)

 ## Data Description
 
 The dataset comprises attributes such as user IDs, loan categories, amounts, interest
 rates, tenure, employment details, income, and more. The target variable is "Defaulter,"
 indicating whether a loan will default.

  ## Data Dictionary

| Column Name          | Data Type                | Description                   |
|----------------------|--------------------------|-------------------------------|
| User id              | Integer                  | Unique user identifier        |
| Loan category        | String                   | Categorical variable          |
| Amount               | Integer                  | Loan amount                   |
| Interest Rate        | Integer                  | Interest rate                 |
| Tenure               | Integer                  | Loan tenure                   |
| Employment type      | String                   | Categorical variable          |
| Tier of Employment   | Categorical and Ordinal  | Employment tier classification|
| Industry             | Categorical              | Industry type                 |
| Role                 | Categorical              | Role description              |
| Work Experience      | Categorical and Ordinal  | Work experience category      |
| Total Income(PA)     | Integer                  | Total annual income           |
| Gender               | Categorical              | Gender of the user            |
| Married              | Categorical              | Marital status                |
| Dependents           | Integer                  | Number of dependents          |
| Home                 | Categorical              | Housing category              |
| Pincode              | Unknown                  | Pincode information           |
| Social Profile       | Categorical              | Social profile of the user    |
| Is_verified          | Categorical              | Verification status           |
| Delinq_2yrs          | Integer                  | Number of delinquencies       |
| Total Payment        | Integer                  | Total payment received        |
| Received Principal   | Integer                  | Principal amount received     |
| Interest Received    | Integer                  | Interest amount received      |
| Number of loans      | Integer                  | Number of loans taken          |
| Defaulter            | Categorical              | Loan defaulter classification |

****
**Column to be predicted "Defaulter"**


 ## Approach

 * Data Preparation:
   * Load and merge Excel sheets.
   * Handle missing values using appropriate techniques.
   * Address data skewness and multicollinearity.
   * Encode categorical features.
   * Address data imbalance for loan defaults.

* Model Building and Tuning:
  * Split the data into training and testing sets.
  * Train XGBoost and Random Forest models.
  * Fine-tune models using Hyperopt and Grid Search.
 
* Libraries Used:
    * NumPy
    * pandas
    * Matplotlib
    * plotly
    * seaborn
    * scikit-learn
    * tensorflow
    * hyperopt
    * imblearn

## Exploratory Data Analysis & Data Preparation

**Goal: To Understand**

*   **Identify data types of each column**
*  **Understand basic stastistics of all numerical columns**
*   **Check missing values**
*   **Plan for handling missing values**
****
*   **Analyze the distribution of each column**
*   **Assess the quality of data based on the distribution**
*   **Identify any skewness in the data?**
*   **Investigate the reasons behind data skewness**

****
*   **Identify and handle categorical features**
*   **Identify and handle ordinal features**
****

*   **Examine the correlation between different numeric variables**
*   **Examine the correlation between categorical variables**

****
*   **Fix data imbalance**

### Multicollinearity

![image](https://github.com/user-attachments/assets/cc98a410-9e83-4273-8e08-498796ff6488)

**Observation:**

No two variables have high correlation with each other, so there is no issue of multicollinearity. It's safe to use all variables in machine learning model building.

### Skewness

![image](https://github.com/user-attachments/assets/97865b8d-2b3d-458c-9769-9438dfc13718)

![image](https://github.com/user-attachments/assets/5715f023-fccf-4849-8e2d-73c7275eea52)

![image](https://github.com/user-attachments/assets/8f93a541-9842-4738-b245-57af0a478a84)

**Analysis after Distribution:**
1. Amount: The distribution of the 'Amount' variable is right-skewed, indicating that a majority of loan amounts are lower, while a few instances have higher values.
2. Employment Type: The distribution of the 'Employment Type' variable shows an imbalance, suggesting that certain employment types may be overrepresented in the dataset compared to others.
3. Payment: The 'Payment' variable displays a right-skewed distribution, suggesting that the majority of payment amounts are lower, with a few instances of higher payments.

### Fixing Skewness

![image](https://github.com/user-attachments/assets/f2325aee-a514-419e-ac8a-6ed387def6ae)

Using log transformation to fix skewness

### Model Training: Xgboost

![image](https://github.com/user-attachments/assets/07cabf47-9d22-4c0a-9749-da2a274e9bad)

### Model Training: RandomForest

![image](https://github.com/user-attachments/assets/7ee4a1f2-f87c-4f55-84a0-f34cf22abe6a)





