# Credit Risk Analysis

## Overview of the Loan Prediction Risk Analysis
Jill commends you for all your hard work. Piece by piece, you’ve been building up your skills in data preparation, statistical reasoning, and machine learning. You are now ready to apply machine learning to solve a real-world challenge: credit card risk.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use `imbalanced-learn` and `scikit-learn` libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the `RandomOverSampler` and `SMOTE` algorithms, and undersample the data using the `ClusterCentroids` algorithm. Then, you’ll use a combinatorial approach of over and undersampling using the `SMOTEENN` algorithm. Next, you’ll compare two new machine learning models that reduce bias, `BalancedRandomForestClassifier` and `EasyEnsembleClassifier`, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

### Deliverables
This new assignment consists of three technical analysis deliverables and a written report.

1. ***Deliverable 1:*** Use Resampling Models to Predict Credit Risk
2. ***Deliverable 2:*** Use the SMOTEENN Algorithm to Predict Credit Risk
3. ***Deliverable 3:*** Use Ensemble Classifiers to Predict Credit Risk
4. ***Deliverable 4:*** A Written Report on the Credit Risk Analysis [README.md](https://github.com/DatJew/Credit_Risk_Analysis)

## Results

### Oversampling

**RandomOverSample:**  
![image](https://github.com/DataJew/Credit_Risk_Analysis/blob/main/Resources/images/CM%20-%20Naive%20Random%20Oversampling.png)


**SMOTE** 
![image](https://github.com/DataJew/Credit_Risk_Analysis/blob/main/Resources/images/CM%20-%20SMOTE%20Oversampling.png)


### Undersampling

***ClusterCentroids***  
![image](https://github.com/DataJew/Credit_Risk_Analysis/blob/main/Resources/images/CM%20-%20Undersampling.png)


### Combination (Over and Under) Sampling

***SMOTEENN***  
![image](https://github.com/DataJew/Credit_Risk_Analysis/blob/main/Resources/images/CM%20-%20Combination.png)


### Ensemble Learners

***BalancedRandomForestClassifier***
![image](https://github.com/DataJew/Credit_Risk_Analysis/blob/main/Resources/images/CM%20-%20Balanced%20RFC.png)


***EasyEnsembleClassifier***  
![image](https://github.com/DataJew/Credit_Risk_Analysis/blob/main/Resources/images/CM%20-%20Easy%20Ensemble%20Adaboost%20Classidfier.png)

## Summary

The precision is low or none for all the models.
