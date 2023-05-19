# Credit-Risk-Classification-Challenge

## Overview of the Analysis

The purpose of this analysis is to use various techniques to train and evaluate a supervised machine learning model based on loan risk. For the analysis, I've used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers that is, if the loans were healthy or high-risk.

The first step was to load the data from CSV and then separating the data into labels and features. Then we checked the balance of the target values using `value_counts` method. After that process, we split the data into train and test data using `train_test_split` and fit the training data into a Logistic Regression model which was then used to make predictions about the healthy or high-risk loans of the test data. The first method predicted that the data contains low samples of high-risk loans. 

I've also used a Logistic Regression Model with Resampled Training Data to make predictions which showed some improvements in accuracy rate and racall rate of the test dataset.

Accuracy scores and classification reports are used to compare the performance of the models.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

- Machine Learning Model 1 (Logistic Regression on Original Data):

  - Balanced Accuracy Score : 94.43%
  - Healthy Loan Precision: 100%, Healthy Loan Recall: 100%
  - High-Risk Loan Precision: 87%, High-Risk Loan Recall: 89%

- Machine Learning Model 2 (Logistic Regression on Resampled Data):

  - Balanced Accuracy Score : 99.60%
  - Healthy Loan Precision: 100%, Healthy Loan Recall: 100%
  - High-Risk Loan Precision: 87%, High-Risk Loan Recall: 100%


## Summary

The results show that, the second model performs bertter as it has higher balance accuracy score and higher recall rate for High-risk loans. Since the second model has a very low false negetives of high-risk loans and maximizes the predictive ability of the false negetive results of high-risk loans, 2nd model should be used in this case. 