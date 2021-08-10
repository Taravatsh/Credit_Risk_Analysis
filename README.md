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

![Random Oversampling Model Accuracy Score]()

- High risk precision of **1%** with **74%** sensitivity/recall score.
- Low risk precision of **100%** with **61%** sensitivity/recall score.

![Random Oversampling Model Confusion Report]()

### SMOTE Model

This portion of the report focuses on the results achieved using another oversampling approach, the **Synthetic minority oversampling technique (SMOTE)**, which deals with increasing the size of the minority by interpolating new instances. The results of the SMOTE model is as follows as depicted in the figure below:

- Balanced accuracy score of **66.2%** which is **1.2%** less than the random over sampling method.

![SMOTE Model Accuracy Score]()

- High risk precision of **1%** with **63%** sensitivity/recall score.
- Low risk precision of **100%** due to high number of true negatives and sensitivity/recall score of **69%** .

![SMOTE Model Confusion Report]()

### ClusterCentroids Model

This part of the project focuses on cluster centroids undersampling which is another machine learning model used for predicting credit risk where the majority class is undersampled down to the size of the minority class. The results achieved using this undersampling technique is as follows as depicted in the figures below:

- Balanced accuracy score of **54.5%**.

![ClusterCentroids Model Accuracy Score]()

- High risk precision of **1%** with **69%** sensitivity/recall score.
- Low risk precision of **100%** with **40%** sensitivity/recall score.

![ClusterCentroids Model Confusion Report]()

## SMOTEENN

In this portion of the project, SMOTEENN  which is considered as an approach to resampling that combines aspects of both oversampling and undersampling  was used for predicting the credit risk. This model oversamples the minority class with SMOTE and cleans the resulting data via undersampling approach. The results achieved using this approach is as follows as demonstrated in the figures below:

- Balanced accuracy score of **66.2%**.

![SMOTEENN Model Accuracy Score]()

- High risk precision of **1%** with **73%** sensitivity/recall score.
- Low risk precision of **100%** with **59%** sensitivity/recall score.

![SMOTEENN Model Confusion Report]()

### BalancedRandomForestClassifier Model

In this section of the project the credit risk was predicted using another machine learning model, Balanced random forest classifier, that reduces bias. The results achieved from this model is as follows:

- Balanced accuracy score of **78.9%**.

![BalancedRandomForestClassifier Model Accuracy Score]()

- High risk precision of **3%** with **70%** sensitivity/recall score.
- Low risk precision of **100%** with **87%** sensitivity/recall score.

![BalancedRandomForestClassifier Model Confusion Report]()

### EasyEnsembleClassifier Model

Lastly, the easy ensemble classifier machine learning model was used for predicting the credit risk. The results achieved from this model as as follow:

- Balanced accuracy score of **93.1%**.

![EasyEnsembleClassifier Model Accuracy Score]()

- High risk precision of **9%** with **92%** sensitivity/recall score.
- Low risk precision of **100%** with **94%** sensitivity/recall score.

![EasyEnsembleClassifier Model Confusion Report]()

## Summary
