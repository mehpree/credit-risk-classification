# Credit Risk Classification Challenge
![image](https://github.com/mehpree/credit-risk-classification/assets/131678606/ecd215d4-9ff0-40f6-84b7-2cce6eb1203d)

## Overview
In this challenge, I tackled the task of building and evaluating a machine learning model for credit risk assessment. The goal was to use historical lending data from a peer-to-peer lending services company to create a model that can predict the creditworthiness of borrowers.

## Step 1: Data Preprocessing and Splitting
### Data Loading
1. I started by reading the "lending_data.csv" dataset from the Resources folder into a Pandas DataFrame.

2. To prepare the data for modeling, I created the labels set (`y`) from the "loan_status" column, where 0 indicates a healthy loan, and 1 indicates a high risk of default. 

3. The remaining columns were used to create the features DataFrame (`X`).

4. I then split the data into training and testing datasets using the `train_test_split` function.

## Step 2: Creating and Evaluating a Logistic Regression Model
### Logistic Regression Model
1. I built a logistic regression model using the training data (`X_train` and `y_train`).

2. Predictions for the testing data labels were generated using the fitted model and the testing feature data (`X_test`).

3. To assess the model's performance, I carried out the following:
   - Generated a confusion matrix.
   - Printed the classification report.

4. Question: I evaluated how well the logistic regression model predicts both the 0 (healthy loan) and 1 (high-risk loan) labels.

## Step 3: Writing a Credit Risk Analysis Report
### Credit Risk Analysis Report
I have prepared a brief report on the performance of the machine learning model used in this challenge. This report is included as the README.md file in my GitHub repository.

### Report Structure
The report follows the structure provided in the "Starter_Code.zip" template and contains the following sections:

1. **Summary**: A brief summary of the challenge and the objective.

2. **Data Preprocessing and Splitting**: An explanation of the data loading and splitting process.

3. **Logistic Regression Model**: Details on building and evaluating the logistic regression model.

4. **Model Performance Analysis**: An analysis of how well the model predicts both healthy and high-risk loans.

The report serves as documentation of the analysis performed in this challenge, summarizing the model's performance and findings.

This concludes the Credit Risk Classification Challenge, where I successfully built and evaluated a logistic regression model for predicting credit risk. The report provides insights into the model's effectiveness in identifying high-risk loans.


1.  **An overview of the analysis:**  Explain the purpose of this analysis.
    
2.  **The results:**  Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.
    
3.  **A summary:**  Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.

## References
Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.
