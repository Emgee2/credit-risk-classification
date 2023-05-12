# Module 12 Report 

## Overview of the Analysis

The purpose of this analysis was to develop machine learning models to predict loan status based on financial information. The data used in this analysis contained information related to loans, and the goal was to predict whether a loan is healthy(label 0) or high-risk(label 1).

The variables that were being predicted were the loan status labels. The 'value_counts' of the labels showed that there were 75036 instances of healthy loans(label 0) and 2500 instances of high-risk loans(label 1) in the dataset.

The analysis involved several stages of the machine learning process. Initially, the data was loaded into a pandas DataFrame, and the labels and features were separated into y and X variables, respectively. Logistic Regression was chosen as the machine learning model for this analysis. The model was instantiated and trained using the original training data. Additionally, a random oversampling technique was applied to address the class imbalance in the dataset. The oversampled training data was then used to fit the logistic regression model.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Logistic Regression with Original Training Data:

    precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384

* Machine Learning Model 2:
  * Logistic Regression with Oversampled Training Data:

  precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.84      0.99      0.91       619

    accuracy                           0.99     19384
   macro avg       0.92      0.99      0.95     19384
weighted avg       0.99      0.99      0.99     19384

## Summary

In summary, the logistic regression model trained with oversampled training data appears to perform better in terms of identifying high-risk loans, while still maintaining a good level of performance for healthy loans. The performance criteria may vary based on the specific objectives and priorities of the analysis.