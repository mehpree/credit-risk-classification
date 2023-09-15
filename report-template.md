# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of this analysis was to build and evaluate machine learning models for predicting loan risk based on lending information. Specifically, we aimed to predict whether a loan is a healthy loan (0) or a high-risk loan (1) using various machine learning techniques.

* Explain what financial information the data was on, and what you needed to predict.
	The dataset included the loan size, interest rate, the borrower's - income, number of accounts, total debt along with the information on if the client's loan was healthy (0) or or if it was at a risk of defaulting (1).
  A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.


* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
  The machine learning process consisted of several stages, including data preprocessing, exploratory data analysis (EDA), feature selection, model selection, model training, and model evaluation.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
  - Logistic Regression: used logistic regression as one of the primary classification algorithms for modeling the loan risk.
  - Random Over Sampler: addressed the class imbalance issue in the dataset by oversampling the minority class (high-risk loans) to improve model performance.

## Results

* Machine Learning Model 1: lending_report

Balanced Accuracy Score: 0.9520479254722232
Precision for Healthy Loans (0): the precision is 1.00, which means that when the model predicts a loan as healthy, it is correct 100% of the time.X%
Recall for Healthy Loans (0): the recall is 0.99, suggesting that the model correctly identifies 99% of the actual healthy loans.
Precision for High-Risk Loans (1): X%
Recall for High-Risk Loans (1): X%



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
