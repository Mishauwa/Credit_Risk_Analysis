# Credit_Risk_Analysis

## Overview of the analysis:

In the following credit card risk analysis we want to predict whether someone has a low or high risk status to not pay back his loan. Credit card risk is hard to predict because the data is unbalanced and has a classification problem because good loans easily outnumber risky loans. Therefore it's necessary to use different techniques to train and evaluate models with unbalanced classes. The data will get oversampled by using the RandomOverSampler and SMOTE algorithms, and under sampled by using the CLusterCentroids algorithms. At the next step we use two machine learning models that reduce bias BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict the risk. For resampling the imbalanced-learn and scikit_learn libraries are used. 

Deliverable 1: Use Resampling Models to Predict Credit Risk.
Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk.
Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk.
Deliverable 4: A Written Report on the Credit Risk Analysis (README.md)


## Results:

- Naive Random Oversampling results: 
	- The balanced accuracy score is 67%.
	- The precision for the high_risk is very low with 1% and the recall is 74%



- SMOTE Oversampling results: 
	- The balanced accuracy score is 66%.
	- The precision for the high_risk is very low with 1% and the recall is 63%



- Undersampling results: 
	- The balanced accuracy score is 54%.
	- The precision for the high_risk is very low with 1% and the recall is 69%



- Combination (Over- and Undersampling) results: 
	- The balanced accuracy score is 64%.
	- The precision for the high_risk is very low with 1% and the recall is 72%



- Balanced Random Forest results: 
	- The balanced accuracy score is 78%.
	- The precision for the high_risk is very low with 4% and the recall is 68%


- Easy Ensemble results: 
	- The balanced accuracy score is 91%.
	- The precision for the high_risk is very low with 9% and the recall is 89%


## Summary:

In total we predicted the loan_status with 6 Machine Learning models. In the first 4 models we undersampled, oversampled and did a combination of both. In the other 2 models we used ensemble classifiers. In total the ensemble classifiers have a better accuracy score than the the first 4 models and also if we compare the precision and recall data of the high_risk loans in the reports we see that the ensemble classifiers are doing better. At the end the Easy Ensemble method is the most accurate and has a very high accuracy score and also better precision and recall than the other techniques.