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

 *  Data Preparation:
   *  Loadandmerge Excel sheets.
   *  Explore data statistics, distributions, and data types.
   *  Handle missing values using appropriate techniques.
   *  Address data skewness and multicollinearity.
   *  Encode categorical features.
   *  Address data imbalance for loan defaults.
* ModelBuilding and Tuning:
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
