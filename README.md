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
  * Utilize Neptune for experiment tracking.
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


