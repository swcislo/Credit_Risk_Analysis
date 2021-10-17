# Credit_Risk_Analysis
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, different techniques were employed to train and evaluate models with unbalanced classes. The decision was made to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

## Overview
A credit card credit dataset from LendingClub, a peer-to-peer lending services company, was utilized to oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Then a comparison of the two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, were used to predict credit risk. An evaluation of the performance of these models was completed. A written recommendation was provided on whether they should be used to predict credit risk.

## Results

### RandomOverSampler model
<img width="641" alt="1" src="https://user-images.githubusercontent.com/85801155/137637059-69e32957-fc20-4225-ac96-3a8d9775b3b1.png">

-Balanced Accuracy Score is 64%

-High Risk Precision is 1% with a sensitivity of 68%

-Low Risk Precision is 100% with a sensitivity of 61%

### SMOTE model
<img width="645" alt="2" src="https://user-images.githubusercontent.com/85801155/137637057-9f0f25d6-e48f-4d3b-b389-2de63254700a.png">

-Balanced Accuracy Score is 64%

-High Risk Precision is 1% with a sensitivity of 68%

-Low Risk Precision is 100% with a sensitivity of 61%

### ClusterCentroids
<img width="644" alt="3" src="https://user-images.githubusercontent.com/85801155/137637056-6dae721d-50e2-45cf-96f0-2151c2f67c74.png">

-Balanced Accuracy Score is 52%

-High Risk Precision is 1% with a sensitivity of 43%

-Low Risk Precision is 100% with a sensitivity of 60%

### SMOTEENN model
<img width="642" alt="4" src="https://user-images.githubusercontent.com/85801155/137637055-3df762f3-e585-465f-941a-4208924d8dbd.png">

-Balanced Accuracy Score is 62%

-High Risk Precision is 1% with a sensitivity of 54%

-Low Risk Precision is 100% with a sensitivity of 71%

### BalancedRandomForestClassifier model
<img width="643" alt="5" src="https://user-images.githubusercontent.com/85801155/137637054-51ee311f-3ec9-4416-aae5-debaebf4b5ab.png">

-Balanced Accuracy Score is 79%

-High Risk Precision is 4% with a sensitivity of 91%

-Low Risk Precision is 100% with a sensitivity of 67%


### EasyEnsembleClassifier model
<img width="643" alt="6" src="https://user-images.githubusercontent.com/85801155/137637053-6995bd98-c543-48af-b67e-f0a554ee773d.png">

-Balanced Accuracy Score is 93%

-High Risk Precision is 7% with a sensitivity of 94%

-Low Risk Precision is 100% with a sensitivity of 91%

## Summary

None of the models have strong precision for predicting if a credit risk is high which is the purpose of analysis. 
