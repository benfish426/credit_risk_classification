# credit_risk_classification

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* The purpose of this analysis is to predict the creditworthiness of borrowers by training and evaluating a model based on a dataset provided to us. 
* The dataset contained financial information on lending activities from a peer-to-peer lending services company. The dataset was comprised of the following columns: loan_size	interest_rate  borrower_income  debt_to_income  num_of_accounts  derogatory_marks  total_debt  loan_stat. We needed to predict the loan_status for future loans.
* The first thing I chose to do after isolating the loan_stat column was perform a value_counts() to see how many 0's and 1's were counted in the dataset. The results showed that the given dataset is not balanced with a ratio of 30:1
* As part of this analysis, there were several stages of the machine learning process I went through. First, there was a brief preprocessing component (set up data for splitting into train/test). Then, I trained the model by using the train_test_split module from 
sklearn.model_selection. Next, I was able to use the LogisticRegression module to fit the model we created using the trained data. I validated my X_test data by comparing it to the fitted model. Lastly, I was able to evaluate how the model performed by creating both a confusion matrix as well as running a classification report.

## Results

* Machine Learning Model for Training 0 (Healthy Loan):
    * F1-Score: 1.00
    * Precision: 1.00
    * Recall scores: 1.00

* Machine Learning Model for Training 1 (High Risk Loan):
    * F1-Score: 0.88
    * Precision: 0.86
    * Recall scores: 0.90

Accuracy: 0.99

* Machine Learning Model for Testing 0 (Healthy Loan):
    * F1-Score: 1.00
    * Precision: 1.00
    * Recall scores: 0.99

* Machine Learning Model for Testing 1 (High Risk Loan):
    * F1-Score: 0.88
    * Precision: 0.85
    * Recall scores: 0.90

Accuracy: 0.99

## Summary

* The logistic regression model performs best here. This is evident from the high ratings in F1-Score, precision, and recall. Another significant statistic we can use to reinforce using the logistic regression model here is the accuracy which was calculated to be 99%.
