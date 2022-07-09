# Module 12 Report Template

## Overview of the Analysis

This analysis was done in order to train a machine learning model to predict creditworthiness of borrowers. The dataset contains
information regarding historical lending activity from a peer-to-peer lending services company. The variable to be predicted
is the 'loan_status' denoted by '0'=healthy loan and '1'=high risk loan. The original dataset contains 75,036 healthy loans
and 2,500 high risk loans. The first step was to split the data into training and testing sets then train a logistic regression
 model on the original data. The logistic regression model was fit to the data then used to make creditworthiness predictions
on the testing data. After that the model was evaluated using the balanced accuracy score, a confusion matrix, and a full
classification report of imbalanced data. Next the data was resampled using RandomOverSampler from imblearn.over_sampling
and a new model was fit to the resampled training data and the new model was then used to make creditworthiness predictions.
Likewise these new predictions were evaluated using the balanced accuracy score, a confusion matrix, and a full classification
report.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Balanced accuracy score = 95.2%
  * Precision = 85%
  * Recall = 91%


* Machine Learning Model 2:
  * Balanced accuracy score = 99.37%
  * Precision = 84%
  * Recall = 99%

## Summary

The original model is slightly more precise but overall recalls less high risk loans than the oversampled model. The sacrifice
of a small amount of precision in exchange for correctly classifying more high risk loans is a small price to pay given the
risks associated with incorrect classification. Thusly the performance of the oversampled model is to be considered better
performing and more useful given that the purpose of the problem is that it is more important to predict the high risk loans.
