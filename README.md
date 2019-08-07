# IEEE-CIS Fraud Detection (Kaggle)
https://www.kaggle.com/c/ieee-fraud-detection/overview

## Overview
In this competition, we benchmark machine learning models on a challenging large-scale dataset. The data comes from Vesta's real-world e-commerce transactions and contains a wide range of features from device type to product features. We also have the opportunity to create new features to improve your results.

## Evaluation
Submissions are evaluated on area under the ROC curve between the predicted probability and the observed target.
For each TransactionID in the test set, you must predict a probability for the isFraud variable.

## Data
In this competition we are predicting the probability that an online transaction is fraudulent, as denoted by the binary target isFraud.

The data is broken into two files identity and transaction, which are joined by TransactionID. Not all transactions have corresponding identity information.

__Categorical Features - Transaction__

* ProductCD
* card1 - card6
* addr1, addr2
* P_emaildomain
* R_emaildomain
* M1 - M9

__Categorical Features - Identity__
* DeviceType
* DeviceInfo
* id_12 - id_38
The TransactionDT feature is a timedelta from a given reference datetime (not an actual timestamp).

__Files__

* train_{transaction, identity}.csv - the training set
* test_{transaction, identity}.csv - the test set (you must predict the isFraud value for these observations)
* sample_submission.csv - a sample submission file in the correct format
