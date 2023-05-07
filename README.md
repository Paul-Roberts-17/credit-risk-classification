# credit-risk-classification

## Overview of the Analysis

The purpose of this analysis is to determine if a loan from a peer-to-peer lending company is at high risk of defaulting. 

The information being used to make this prediction consists of the following:
•	Loan size
•	Interest rate
•	Borrower income
•	Debt to income ratio
•	Num of accounts
•	Derogatory marks
•	Total debt
This information was used to assess whether the loan was healthy or at high risk of defaulting.

The data used to set up the model consisted of 77,536 sets of the above information. Of those 75,036 and 2,500 had already been determined to be healthy or at high risk of defaulting respectively.

The total data pool was then split into a training set and a testing set. This split was done randomly and with the following ratio; 75% training : 25% testing. The training data was used to train a logistic regression model and the testing data was then used to assess the accuracy of that model.

## Results

Logistic regression model:
•	Balanced accuracy score: 0.952
o	Overall accuracy of 95.2% for the model predicting the 77,536 sample loans
•	Precision
o	True Positive: When the model predicted a healthy loan, it was right 100% of the time.
o	False Positive: Of the loans predicted as be at high risk of default, only 85% of them actually were. 15% were healthy loans.
•	Recall
o	False Negative: This model only found 99% of the healthy loans. 1% of the healthy loans were predicted as being at high risk of default.
o	True Negative: Of the loans that are at high risk of default, this model found 91% of them.

## Summary

This model is almost perfect at predicting the healthy loans. Finding the healthy loans isn’t our main aim though. We need to find the loans that are at high risk of default and this model only finds 91% of them. 91% is a good result but missing 9% of the bad loans could cost a lot of money. As such, I don’t recommend this model as a sole means of identifying high risk loans. It does however, perform well enough to aid in the process by identifying the easier cases and leaving staff more time to find the less obvious ones.
