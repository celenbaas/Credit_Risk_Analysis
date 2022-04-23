# Credit_Risk_Analysis

## Overview

The concept around this analysis is to apply machine learning to solve a real-world challenge for credit card risk.  Credit card risk is an unbalanced classification problem since good loans outnumber risky loans.  Because of this I tested different techniques to train and evaluate models with unbalanced classes.  Library’s used were Imbalanced-learn and scikit-learn.

## Results

Six models were run to evaluate credit risk.

**Balanced Accuracy Score** Blends together the precision and recall getting an overall metric.

**Precision** looks at the actual positive divided by the total predicted positive.

**Recall** looks at correct positive perditions and considers any false negative predictions. This looks at how accurate a positive outcome was predicted. In cases where there is significant impact of a false negative, we would want the model to have a high recall, which means there are few false negatives.

o Oversampling
I compared two oversampling algorithms to determine which resulted in the best performance.  These algorithms were naive random oversampling and SMOTE algorithm.

**Naive Random Oversampling**
The balanced accuracy score is 63.67%, the classification summary is shown below.
<img width="449" alt="Naive Random Oversampling" src="https://user-images.githubusercontent.com/96347024/164938653-a3191e54-f843-4a15-ad88-540258018b3b.png">

**SMOTE Oversampling**
The balanced accuracy score is 63.67%, the classification summary is shown below.
<img width="445" alt="SMOTE Oversampling" src="https://user-images.githubusercontent.com/96347024/164938681-7399a712-929a-4dfd-ab04-f1b067a462f3.png">


o Undersampling
I tested the Undersampling algorithm called Cluster Centroids to determine which resulted in the best performance compared to the oversampling algorithms above. 

**Cluster Centroids**
The balanced accuracy score is 63.0%, the classification summary is shown below.
<img width="439" alt="Undersampling" src="https://user-images.githubusercontent.com/96347024/164938747-c5f73f1a-9160-4ed0-9547-53d68be3f4e4.png">


o Combination (Over and Under) Sampling
I than tested the SMOTEENN algorithm which is a combination over- and under-sampling algorithm to determine if the algorithm results in the best performance compared to the other sampling algorithms above. 

**SMOTEENN**
The balanced accuracy score is 59.0%, the classification summary is shown below.
<img width="442" alt="SMOTEENN" src="https://user-images.githubusercontent.com/96347024/164938784-fc51c6bb-0d3a-47bc-91f2-91eac2cb2459.png">


o Ensemble Learners
I compared two ensemble algorithms to determine which algorithm resulted in the best performance. These algorithms were Balanced Random Forest Classifier and an Easy Ensemble AdaBoost classifier.

**Balanced Random Forest Classifier**
The balanced accuracy score is 62.9%, the classification summary is shown below.
<img width="445" alt="Balanced Random Forest Classifier" src="https://user-images.githubusercontent.com/96347024/164938804-d1ffa84c-2697-4366-a5b9-7afeb8374edd.png">

**Easy Ensemble AdaBoost Classifier**
The balanced accuracy score is 93.16%, the classification summary is shown below.
<img width="442" alt="Easy Ensemble AdaBoost Classifier" src="https://user-images.githubusercontent.com/96347024/164938827-871e1650-f7da-4a62-bb5e-8a7ff14c9525.png">


## Summary

The Easy Ensemble AdaBoost Classifier model produced the most accurate results with an accuracy score of 93.16%.  This is the model I would recommend to evaluate credit risk.
