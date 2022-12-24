# Credit_Risk_Analysis

## Overview of the analysis:

In the following credit card risk analysis we want to predict whether someone has a low or high risk status to not pay back his loan. Credit card risk is hard to predict because the data is unbalanced and has a classification problem because good loans easily outnumber risky loans. Therefore it's necessary to use different techniques to train and evaluate models with unbalanced classes. The data will get oversampled by using the RandomOverSampler and SMOTE algorithms, and under sampled by using the CLusterCentroids algorithms. At the next step we use two machine learning models that reduce bias BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict the risk. For resampling the imbalanced-learn and scikit_learn libraries are used. 

- Deliverable 1: Use Resampling Models to Predict Credit Risk.
- Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk.
- Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk.
- Deliverable 4: A Written Report on the Credit Risk Analysis (README.md)


## Results:

- Naive Random Oversampling results: 
	- The balanced accuracy score is 67%.
	- The precision for the high_risk is very low with 1% and the recall is 74%

<img width="1088" alt="Naive_Random_OS" src="https://user-images.githubusercontent.com/69826498/209418884-704e1416-03fe-47fc-8ce8-a5e8a8d122db.png">

- SMOTE Oversampling results: 
	- The balanced accuracy score is 66%.
	- The precision for the high_risk is very low with 1% and the recall is 63%

<img width="1088" alt="SMOTE" src="https://user-images.githubusercontent.com/69826498/209418887-6cb8007e-6e7b-49c2-83b7-1bcc162f71ae.png">

- Undersampling results: 
	- The balanced accuracy score is 54%.
	- The precision for the high_risk is very low with 1% and the recall is 69%

<img width="1088" alt="Undersampling" src="https://user-images.githubusercontent.com/69826498/209418908-291a5723-3cec-4a67-8a49-31945187bc49.png">

- Combination (Over- and Undersampling) results: 
	- The balanced accuracy score is 64%.
	- The precision for the high_risk is very low with 1% and the recall is 72%
	
<img width="1088" alt="Combination" src="https://user-images.githubusercontent.com/69826498/209418914-417faf43-2954-46a2-9920-8fb4519b03ff.png">

- Balanced Random Forest results: 
	- The balanced accuracy score is 78%.
	- The precision for the high_risk is very low with 4% and the recall is 68%

<img width="1088" alt="Random_Forest" src="https://user-images.githubusercontent.com/69826498/209418926-d50c39b0-7e1d-4da6-a85c-5a30d3d6a162.png">

- Easy Ensemble results: 
	- The balanced accuracy score is 91%.
	- The precision for the high_risk is very low with 9% and the recall is 89%

<img width="1088" alt="Easy_Ensemble" src="https://user-images.githubusercontent.com/69826498/209418935-360262dd-4046-4abc-b649-c067f7e84f3d.png">

## Summary:

In total we predicted the loan_status with 6 Machine Learning models. In the first 4 models we undersampled, oversampled and did a combination of both. In the other 2 models we used ensemble classifiers. In total the ensemble classifiers have a better accuracy score than the the first 4 models and also if we compare the precision and recall data of the high_risk loans in the reports we see that the ensemble classifiers are doing better. At the end the Easy Ensemble method is the most accurate and has a very high accuracy score and also better precision and recall than the other techniques.
