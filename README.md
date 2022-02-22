# Credit_Risk_Analysis

## Overview of the analysis

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Results

I tried 6 ways of supervised training, and I'll explain them one by one below: 

### Naive_Random_Oversampling
![Naive_Random_Oversampling](https://raw.githubusercontent.com/yumik20/Credit_Risk_Analysis/main/Screenshots/1_Naive_Random_Oversampling.png)

Accuracy Score: 64.76%
Precision High Risk: 1%
Precision Low Risk: 100%
Recall High Risk: 61%
Recall Low Risk: 68%
F1 High Risk:2%
F1 Low Risk:81% 



### SMOTE_Oversampling
![SMOTE_Oversampling](https://raw.githubusercontent.com/yumik20/Credit_Risk_Analysis/main/Screenshots/2_SMOTE_Oversampling.png)

Accuracy Score: 65.14%
Precision High Risk: 1%
Precision Low Risk: 100%
Recall High Risk: 61%
Recall Low Risk: 69%
F1 High Risk:2%
F1 Low Risk:81% 



### Under_sampling
![Under_sampling](https://raw.githubusercontent.com/yumik20/Credit_Risk_Analysis/main/Screenshots/3_Under_sampling.png)


Accuracy Score: 54.47%
Precision High Risk: 1%
Precision Low Risk: 100%
Recall High Risk: 69%
Recall Low Risk: 40%
F1 High Risk:1%
F1 Low Risk:57% 


### Combination_Sampling
![Combination_Sampling](https://raw.githubusercontent.com/yumik20/Credit_Risk_Analysis/main/Screenshots/4_Combination_Sampling.png)


Accuracy Score: 62.04%
Precision High Risk: 1%
Precision Low Risk: 100%
Recall High Risk: 64%
Recall Low Risk: 60%
F1 High Riskk:2%
F1 Low Risk:75% 


### Balanced_Random_Forest_Classifier
![Balanced_Random_Forest_Classifier](https://raw.githubusercontent.com/yumik20/Credit_Risk_Analysis/main/Screenshots/5_Balanced_Random_Forest_Classifier.png)


Accuracy Score: 78.85%
Precision High Risk: 3%
Precision Low Risk: 100%
Recall High Risk: 70%
Recall Low Risk: 87%
F1 High Risk:6%
F1 Low Risk:93% 


### Easy_Ensemble_AdaBoost_Classifier
![Easy_Ensemble_AdaBoost_Classifier](https://raw.githubusercontent.com/yumik20/Credit_Risk_Analysis/main/Screenshots/6_Easy_Ensemble_AdaBoost_Classifier.png)

Accuracy Score: 93.16%
Precision High Risk: 9%
Precision Low Risk: 100%
Recall High Risk: 92%
Recall Low Risk: 94%
F1 High Risk:16%
F1 Low Risk:97% 


## Summary
Based on the data above, it seems that Easy_Ensemble_AdaBoost_Classifier and Balanced_Random_Forest_Classifier have better training results than the rest of methods for our dataset.

Balanced_Random_Forest_Classifier
Accuracy Score: 78.85%
Recall High Risk: 70%
Recall Low Risk: 87%


Easy_Ensemble_AdaBoost_Classifier
Accuracy Score: 93.16%
Recall High Risk: 92%
Recall Low Risk: 94%


I would recommend to use Easy_Ensemble_AdaBoost_Classifier model to predict loans in our case.  
