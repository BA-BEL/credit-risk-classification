# Report

## Overview of the Analysis


The purpose of this analysis was to create a regression model that predicts healthy and high-risk loans.

The model was trained and tested with a dataset that includes the following features:

* Loan size
* Interest rate
* Borrower income
* Debt-to-income ratio
* Number of accounts
* Derogatory marks
* Total debt

This dataset was split into training and validation partitions.

In the whole dataset, there were 75036 healthy loans (with a target value of 0) and 2500 high-risk loans (target = 1).

A logistic regression model was used to fit and predict the data; furthermore, a second model was tested with generated oversampled data (where healthy loans and high-risk loans were equal) to test whether the original model is overfitted. The result of this indicates that it is not as both models performed similarly.


## Results

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.



  * Balanced accuracy: 95.20%
  * Precision: 100% and 85% for predictions of 0 and 1 respectively.
  * Recall: 99% and 91% for predictions of 0 and 1 respectively.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

  * Balanced accuracy: 99.37%
  * Precision: 100% and 84% for predictions of 0 and 1 respectively.
  * Recall: 99% and 99% for predictions of 0 and 1 respectively.

## Summary

The logistic regression model is a promising model as it performed as desired for the original data and for the randomly oversampled data.

* Considering that the performance is similar across both models, it is indicated that the original model is not overfitted.

The original model is promising as it contains a high balanced accuracy score, in addition to high precision and recall.

* It is worth noting that there is a lower precision for the model's predictions of high-risk loans, but in comparison to the 100% precision of healthy loans, this performance can be acceptable depending on the firm's goals

* * A precision of 100% in the model for classifying healthy loans means that of all loans predicted to be healthy, they have been healthy.

* * On the other hand, the 85% precision for predicting high-risk loans means that 15% of the time, the model incorrectly predicts a *healthy* loan to be high-risk.

* * * In summary, this means that, in practice, the model will have an extremely high likelihood of correctly predicting healthy loans with the risk of incorrectly classifying some healthy loans as high-risk.

This model is recommend provided that the lender wants to minimize high-risk loans with a slight risk of incorrectly classifying some potentially healthy loans as high-risk.

* Overall, it ought to be tried for a pilot run.
