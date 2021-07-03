# Credit_Risk_Analysis

## Overview of the loan prediction risk analysis:
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we'll need to employ different techniques to train and evaluate models with unbalanced classes. This analysis uses Python's imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I'll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I'll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I'll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Then I will evaluate the performance of these models and see how well these predict data.

## Results:

- Random Oversampling:

![RandomOverSampler.PNG](https://github.com/tjavaheripour/Credit_Risk_Analysis/blob/main/Images/RandomOverSampler.PNG)

- SMOTE oversampling:

![SMOTE.PNG](https://github.com/tjavaheripour/Credit_Risk_Analysis/blob/main/Images/SMOTE.PNG)

- Cluster Centroids Undersampling:

![Undersampling.PNG](https://github.com/tjavaheripour/Credit_Risk_Analysis/blob/main/Images/Undersampling.PNG)

- SMOTEENN (combinatorial approach of over- and undersampling):

![SMOTEENN.PNG](https://github.com/tjavaheripour/Credit_Risk_Analysis/blob/main/Images/SMOTEENN.PNG)

- Balanced Random Forest Classifier:

![BalancedRandomForestClassifier.PNG](https://github.com/tjavaheripour/Credit_Risk_Analysis/blob/main/Images/BalancedRandomForestClassifier.PNG)

- Easy Ensemble Classifier:

![EasyEnsembleClassifier.PNG](https://github.com/tjavaheripour/Credit_Risk_Analysis/blob/main/Images/EasyEnsembleClassifier.PNG)
