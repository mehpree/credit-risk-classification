# Credit Risk Classification Challenge
![Alt text](image-1.png)

## Overview
In this challenge, I tackled the task of building and evaluating a machine learning model for credit risk assessment. The goal was to use historical lending data from a peer-to-peer lending services company to create a model that can predict the creditworthiness of borrowers.

## Step 1: Data Preprocessing and Splitting
### Data Loading
1. I started by reading the "lending_data.csv" dataset from the Resources folder into a Pandas DataFrame.

2. To prepare the data for modeling, I created the labels set (`y`) from the "loan_status" column, where 0 indicates a healthy loan, and 1 indicates a high risk of default. 

3. The remaining columns were used to create the features DataFrame (`X`).

4. I then split the data into training and testing datasets using the `train_test_split` function.

## Step 2: Creating and Evaluating both Logistic Regression Models

1. I built two logistics regression models  called `log_classifier` and `oversampled_classifier` - fit those, calculated predictions and results and then evaluated their performance using `balanced_accuracy_score` & `confusion_matrix`. The results were then stored in `lending_report` and `oversampled_report`.

2. To assess the model's performance, I carried out the following:
   - Generated a confusion matrix.
   - Printed the classification report.

3. Question: I evaluated how well the logistic regression model predicts both the 0 (healthy loan) and 1 (high-risk loan) labels.

## For a detailed Credit Analysis Report please go through the OverviewAnalysis.md document.

This concludes the Credit Risk Classification Challenge, where I successfully built and evaluated a logistic regression model for predicting credit risk. The report provides insights into the model's effectiveness in identifying high-risk loans.

## References
Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.
