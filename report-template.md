## Overview of the Analysis


**Purpose**: 
The purpose of this analysis was to build and evaluate machine learning models for predicting loan risk based on lending information that was derived from 'lending_data.csv'. Specifically, we aimed to predict whether a loan is a healthy loan (0) or a high-risk loan (1) using various machine learning techniques and training and test models.

**Data Preprocessing and Splitting**: 

The dataset included the loan size, interest rate, the borrower's - income, number of accounts, total debt along with the information on if the client's loan was healthy (0) or or if it was at a risk of defaulting (1). A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

Split the data into training and testing datasets by using `train_test_split.

**Logistic Regression Model**: 

* I built two logistics regression models  called `log_classifier` and `oversampled_classifier` - fit those, calculated predictions and results and then evaluated their performance using `balanced_accuracy_score` & `confusion_matrix`. The results were then stored in `lending_report` and `oversampled_report`.

The machine learning process consisted of several stages, including exploratory data analysis (EDA), feature selection, model selection, model training, and model evaluation.

* Feature Selection: Identified relevant features for modeling.
* Model Selection: Chose machine learning algorithms - Logistic Regression.
* Model Training: Trained model on the original as well as resampled data which was resampled using `RandomOverSampler`

Evaluated model performance using the following metrics:
  - Logistic Regression: used logistic regression as one of the primary classification algorithms for modeling the loan risk.
  - Random Over Sampler: addressed the class imbalance issue in the dataset by oversampling the minority class (high-risk loans) to improve model performance.

## Results

* Machine Learning Model 1: lending_report a.k.a Original Data


- Precision for "High-Risk Loan" class: 0.85
- Recall for "High-Risk Loan" class: 0.91
- F1-score for "High-Risk Loan" class: 0.88


* Machine Learning Model 2: oversampled_report a.k.a Resampled Data


- Precision for "High-Risk Loan" class: 0.84
- Recall for "High-Risk Loan" class: 0.99
- F1-score for "High-Risk Loan" class: 0.91

The two classification reports you've provided show the performance of your model on two different datasets: one with resampled data using RandomOverSampler and one with the original data. Let's compare these reports:

Precision: Precision for the "High-Risk Loan" class is slightly lower in the RandomOverSampler data (0.84) compared to the original data (0.85). This means that in the resampled data, there may be a slightly higher rate of false positives for the "High-Risk Loan" class.

Recall: Recall for the "High-Risk Loan" class is the same in both reports (0.91). This indicates that both the resampled and original data have the same ability to correctly identify true positives for the "High-Risk Loan" class.

F1-Score: The F1-score for the "High-Risk Loan" class is higher in the RandomOverSampler data (0.91) compared to the original data (0.88). This indicates that the model's ability to balance precision and recall for the "High-Risk Loan" class is slightly better in the resampled data.

## Summary

Overall, it appears that the RandomOverSampler data performs slightly better in terms of F1-score for the "High-Risk Loan" class, which suggests that using oversampling has improved the model's ability to classify high-risk loans while maintaining a relatively high level of precision. However, it's essential to consider the specific objectives and trade-offs of your problem when deciding which dataset to use for your model.

Another important thing to consider while choosing the model would be what factor do we actually choose to base a candidate's 'creditworthiness' on - Healthy Loan or High-Risk Loan? Based on our deciding factor the choice of model can be changed. 