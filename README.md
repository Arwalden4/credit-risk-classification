# credit-risk-classification
## Background
In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

This analysis generated a machine learning model consisting of logistic regression in order to predict the credit risk associated with loans. The dataset covered such financial data as loan sizes, interest rates, borrower income, debt-to-income ratios, and total debt. The model used this data to predict the status of loans as either healthy or risky using a logistic regression algorithm from the scikit-learn machine learning library in Python.

The stages of this machine learning process consisted of the following:

* Splitting the dataset into training and testing sets.
* Creating a logistic regression model (LogisticRegression) using the training data.
* Saving predictions on the testing labels of X and y respectively.
* Generating a confusion matrix and classification report to gauge the model's scores showing its precision and recall of the testing variables.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Accuracy: The accuracy score for the logistic regression model is .99, meaning it is 99% correct in classifying its predicted values.
    * The precision score for the model is 1.00 for predicting healthy loans ('0'), meaning it will always classify these positives correctly with no false positives. The model has a precision score of .87 for predicting high-risk loans ('1's),  indicating a medium reliability score for identifying high-risk loans with some false negatives.
    * The recall score for healthy loans ('0's) in the model is 1.00, meaning it invariably predicts the status of healthy loans correctly. For high-risk loans ('1's), the model has a score of .95, indicating a very high reliability to predict high-risk loans correctly with few false negatives.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

The classification report shows that it is fairly accurate in predicting results trained using the original data. The model does indicate some shortcomings with predicting high-risk loans, with a moderately reliable accuracy score of which the consistency can be improved. The performance of the model and its reliability is contingent on which data we would like to predict consistently. We can only identify healthy loan applications with perfect reliability, but not high-risk loans with the same degree of accuracy. This means that the company which requires this analysis will be using a model which may falsely classify high-risk loans as acceptable or healthy, ultimately threatening the company with potential losses for such applications. Therefore, the success of this model depends on what results the company would like to prioritize in its analyses and how well-equipped its financial models should be to identify toxic loans which might undermine the profitability of the firm in the long-term.


