# Credit_Risk_Analysis

## Overview of Analysis

Credit risk is an inherently unbalanced classification problem, since good loans outnumber risky loans easily. The purpose of this project is to use different machine learning concepts to predict credit risk using the credict card dataset from LendingClub, a peer-to-peer lending services company, by employing various techniques for training and evaluating models having unbalanced classes. As a result of this we are required to use **imbalanced-learn** and **scikit-learn** python libraries to build and evaluate the following models using resampling:

- Oversampling the data using the **RandomOverSampler** and **SMOTE** algorithms.
- Undersampling the data using the **ClusterCentroids** algorithm.
- Oversampling and Undersampling the data via the combinational approach using the **SMOTEENN** algorithm.
- Comparing two machine learning models that reduce bias, **BalancedRandomForestClassifier** and **EasyEnsembleClassifier**, for making credict risk predictions. 

## Results

This section of the project focuses on the results achieved for the RandomOverSampler Model, SMOTE Model, ClusterCentroids Model, BalancedRandomForestClassifier, EasyEnsembleClassifier. The results achieved are in terms of:

- Balanced accuracy score
- Precision
- Recall scores

### RandomOverSampler Model

This portion of the report focuses on the balanced accuracy score, precision and recall scores of the random oversampling model where the instances of the minority class are randomly selected and added to the training set until the minority and majority classes are balanced. It can be noted that in our case the minority class is the **low_risk**  loan status and the majority class is the **high_risk** status. The following results were achieved using the random oversampling model, as shown in the figure below:

- Balanced accuracy score of **67.4%**.
- High risk precision of **1%** with **74%** sensitivity/recall score.
- Low risk precision of **100%** with **61%** sensitivity/recall score.

![Random Oversampling Model]()

### SMOTE Model

This portion of the report focuses on the results achieved using another oversampling approach, the **Synthetic minority oversampling technique (SMOTE)**, which deals with increasing the size of the minority by interpolating new instances. The results of the SMOTE model is as follows as depicted in the figure below:

- Balanced accuracy score of **66.2%** which is **1.2%** less than the random over sampling method.
- High risk precision of **1%** with **63%** sensitivity/recall score.
- Low risk precision of **100%** due to high number of true negatives and sensitivity/recall score of **69%** .

![SMOTE Model]()

### ClusterCentroids Model


## SMOTEENN

### BalancedRandomForestClassifier


### EasyEnsembleClassifier
## Summary
