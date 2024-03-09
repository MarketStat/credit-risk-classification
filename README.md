# credit-risk-classification

## Overview of the Analysis

The purpose of this analysis is to predict creditworthiness of borrowers using a model built from lending data provided by a peer-to-peer lending services company. The labels (dependent variable y) is loan status which determines if a loan is healthy, '0', or high-risk, '1'. The features (independent variables x) are loan size, interest rate,	borrower income,	debt to income, number of accounts,	derogatory marks and total debt. Identifying which loans will be high-risk versus healthy will help the bank operate more effectively by helping bankers make informed decisions on lending. Below are the steps used in the creation of this model.

1. Data Loading and Preprocessing - The data from the lending-data CSV is loaded into a Pandas Dataframe. Next the y and x variables are set to the loan labels (y) and features (x).  The data is then split up into training and test data using scikit-learn package 'train_test_split'.

2. Training the Model - A Logistic Regression classifier is fit with training data and predictions are saved using test data

3. Evaluating the Model - The model is evaluated using a confusion matrix and a classification report

## Results

* Machine Learning Model 1:
- Overall Accuracy - 0.99

- Healthy Loans
  - Precision - 1.00
  - Recall - 1.00
  - f1-score - 1.00

- High-Risk Loans
  - Precision - 0.87
  - Recall - 0.89
  - f1-score - 0.88

## Summary

The 0.99 accuracy score suggests this is a high-performance model. The precision and recall scores are also high, especially for healthy loans (though the difference in support for the variables may have an impact). The high accuracy score may also help minimize false positives and/or false negatives. 

This model can be used to assist bankers identifying risk level for loans.
