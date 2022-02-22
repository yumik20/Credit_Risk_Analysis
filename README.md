# Credit_Risk_Analysis

## Overview of the analysis

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Results

I tried 6 ways of supervised training, and I'll explain them one by one below: 

### Naive_Random_Oversampling
![Naive_Random_Oversampling](https://raw.githubusercontent.com/yumik20/Credit_Risk_Analysis/main/Screenshots/1_Naive_Random_Oversampling.png)

The precision for the high_risk has a very low positivity at 1% and the avg. recall is 68%. The F1 for high_risk is also 2%, which is not good. 


### SMOTE_Oversampling
![SMOTE_Oversampling](https://raw.githubusercontent.com/yumik20/Credit_Risk_Analysis/main/Screenshots/2_SMOTE_Oversampling.png)




### Under_sampling
![Under_sampling](https://raw.githubusercontent.com/yumik20/Credit_Risk_Analysis/main/Screenshots/3_Under_sampling.png)


### Combination_Sampling
![Combination_Sampling](https://raw.githubusercontent.com/yumik20/Credit_Risk_Analysis/main/Screenshots/4_Combination_Sampling.png)


### Balanced_Random_Forest_Classifier
![Balanced_Random_Forest_Classifier](https://raw.githubusercontent.com/yumik20/Credit_Risk_Analysis/main/Screenshots/5_Balanced_Random_Forest_Classifier.png)


### Easy_Ensemble_AdaBoost_Classifier
![Easy_Ensemble_AdaBoost_Classifier](https://raw.githubusercontent.com/yumik20/Credit_Risk_Analysis/main/Screenshots/6_Easy_Ensemble_AdaBoost_Classifier.png)




## Summary