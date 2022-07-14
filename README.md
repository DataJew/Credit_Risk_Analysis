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
4. ***Deliverable 4:*** A Written Report on the Credit Risk Analysis [`README.md`](https://github.com/DatJew/Credit_Risk_Analysis)

## Results
A Classification report is used to measure the quality of predictions from a classification algorithm. 

The report shows the main classification metrics precision, recall and f1-score on a per-class basis. The metrics are calculated by using true and false positives, true and false negatives. Positive and negative in this case are generic names for the predicted classes. There are four ways to check if the predictions are right or wrong:

TN / True Negative: when a case was negative and predicted negative
TP / True Positive: when a case was positive and predicted positive
FN / False Negative: when a case was positive but predicted negative
FP / False Positive: when a case was negative but predicted positive

Precision = TP/(TP + FP) ->
***What percent of your predictions were correct?***

Recall = TP/(TP+FN) ->
***What percent of the positive cases did you catch?*** 

F1 Score = 2*(Recall * Precision) / (Recall + Precision) ->
***What percent of positive predictions were correct?*** 

How many predictions are True and how many are False. More specifically, True Positives, False Positives, True negatives and False Negatives are used to predict the metrics of a classification report as shown below:

### Oversampling

***RandomOverSample***  
![image](https://github.com/DataJew/Credit_Risk_Analysis/blob/main/Resources/images/CM%20-%20Naive%20Random%20Oversampling.png)


***SMOTE*** 
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
For all models, utilizing **BalancedRandomForestClassifier** is the most effective as it provides the highest Score for all Risk loans.
The precision is low or none for all the models. In General, the **EasyEnsembleClassifier** algorythm will perform a High-Risk loan precision with more accuracy than the additional models.
