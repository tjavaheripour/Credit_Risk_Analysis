# Credit_Risk_Analysis

## Overview of the loan prediction risk analysis:
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we'll need to employ different techniques to train and evaluate models with unbalanced classes. This analysis uses Python's imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I'll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I'll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I'll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Then I will evaluate the performance of these models and see how well these predict data.

## Results:

### 1- Random Oversampling:

- Accuracy Score: 66%
- Precision High Risk: 1%
- Precision Low Risk: 100%
- Recall High Risk: 74%
- Recall Low Risk: 58%

![RandomOverSampler.PNG](https://github.com/tjavaheripour/Credit_Risk_Analysis/blob/main/Images/RandomOverSampler.PNG)

### 2- SMOTE oversampling:

- Accuracy Score: 65%
- Precision High Risk: 1%
- Precision Low Risk: 100%
- Recall High Risk: 62%
- Recall Low Risk: 68%

![SMOTE.PNG](https://github.com/tjavaheripour/Credit_Risk_Analysis/blob/main/Images/SMOTE.PNG)

### 3- Cluster Centroids Undersampling:

- Accuracy Score: 54%
- Precision High Risk: 1%
- Precision Low Risk: 100%
- Recall High Risk: 69%
- Recall Low Risk: 40%

![Undersampling.PNG](https://github.com/tjavaheripour/Credit_Risk_Analysis/blob/main/Images/Undersampling.PNG)

### 4- SMOTEENN (combinatorial approach of over- and undersampling):

- Accuracy Score: 68%
- Precision High Risk: 1%
- Precision Low Risk: 100%
- Recall High Risk: 77%
- Recall Low Risk: 59%

![SMOTEENN.PNG](https://github.com/tjavaheripour/Credit_Risk_Analysis/blob/main/Images/SMOTEENN.PNG)

### 5- Balanced Random Forest Classifier:

- Accuracy Score: 79%
- Precision High Risk: 3%
- Precision Low Risk: 100%
- Recall High Risk: 70%
- Recall Low Risk: 87%

![BalancedRandomForestClassifier.PNG](https://github.com/tjavaheripour/Credit_Risk_Analysis/blob/main/Images/BalancedRandomForestClassifier.PNG)

### 6- Easy Ensemble Classifier:

- Accuracy Score: 93%
- Precision High Risk: 9%
- Precision Low Risk: 100%
- Recall High Risk: 92%
- Recall Low Risk: 94%

![EasyEnsembleClassifier.PNG](https://github.com/tjavaheripour/Credit_Risk_Analysis/blob/main/Images/EasyEnsembleClassifier.PNG)

## Summary:

This analysis is trying to find the best model that can detect if a loan is high risk or not. So, we need to find a model with the highest percentage of accuracy score, balance of precision, and recall scores.
Looking at the different models, I derived the followings :

The highest high-risk recall: Easy Ensemble Classifier with 92%
The highest low-risk recall: Easy Ensemble Classifier with 94%
The highest accuracy : Easy Ensemble Classifier with 93%
The highest precision score for high risk : Easy Ensemble Classifier with 9%

Therefore, I would recommend the Easy Ensemble Classifier machine learning model to use for predicting high risk loans.
