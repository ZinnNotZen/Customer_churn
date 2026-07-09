# Customer_churn
Exploring data to see what factors impact the churn rate of telecommunications company.

<img width="653" height="862" alt="Executive Overview" src="https://github.com/user-attachments/assets/5ca0be57-2d8a-4d2c-93b0-fab15f44c19c" />


## Project Overview

This project analyzes customer churn data from a telecommunications company to identify the factors associated with customer attrition and to develop a predictive model capable of identifying customers at risk of leaving.

The project follows a complete data analytics workflow, including data cleaning, exploratory data analysis (EDA), statistical testing, feature engineering, predictive modeling, and business recommendations.

## Research Questions

1. What factors are associated with customer churn?
2. Can customer churn be predicted using customer demographic and service information?

## Dataset

The dataset contains customer demographics, account information, subscribed services, billing details, and whether the customer churned.
The dataset was quired from Kaggle at this link: https://www.kaggle.com/code/bhartiprasad17/customer-churn-prediction/input

## Methodology

* Removed duplicate records.
* Cleaned and converted data types.
* Performed exploratory data analysis on numerical and categorical variables.
* Used chi-square tests to evaluate relationships between categorical features and churn.
* Encoded categorical variables for machine learning.
* Trained a Logistic Regression model to predict customer churn.
* Evaluated model performance using accuracy, precision, recall, and F1-score.
* Tuned the classification threshold to improve predictive performance.
* Interpreted logistic regression coefficients to identify the strongest drivers of churn.

## Key Findings

* Contract type was the strongest predictor of customer churn, with longer-term contracts associated with substantially lower churn.
* Customers using fiber optic internet and electronic check payments were more likely to churn.
* Customers with technical support and online security services were less likely to churn.
* Gender and phone service showed little evidence of a meaningful relationship with churn.
* The logistic regression model achieved approximately 80% accuracy while providing interpretable insights into the factors influencing customer retention.

## Business Recommendations

* Develop targeted retention campaigns for customers on month-to-month contracts.
* Encourage enrollment in longer-term contracts through promotional incentives.
* Promote value-added services such as technical support and online security.
* Investigate why customers using electronic check payments experience higher churn rates.
* Use the predictive model to identify high-risk customers and proactively offer retention incentives.

## Technologies Used

* Python
* pandas
* NumPy
* Matplotlib
* scikit-learn
* SciPy
* Jupyter Notebook

## Future Improvements

* Compare Logistic Regression with tree-based models such as Random Forest and Gradient Boosting.
* Perform hyperparameter tuning and cross-validation.
* Investigate feature engineering techniques and model explainability methods to further improve predictive performance.

## Data Notes

Several features related to internet service (e.g., InternetService_No and OnlineSecurity_No internet service) have identical coefficients because they are highly correlated. This multicollinearity is expected given the structure of the dataset and should be considered when interpreting individual coefficients.
