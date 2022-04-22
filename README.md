# Credit Risk Analysis

## Project Purpose

Using the credit card dataset from LendingClub we used six machine learning models to predict credit risk. These models are:
  - RandomOverSampler
  - SMOTE
  - ClusterCentroids
  - SMOTEENN
  - BalancedRandomForestClassifier
  - EasyEnsembleClassifier

We assessed the performance of all six models and based on the data can make a recommendation regarding if they should be used to predict credit risk.

## Results

### RandomOverSampler Model

![](/images/randomovrsmplr.png)

The balanced accuracy score is 64%. The high risk precision is 1%, with a sensitivity percentage of 63%, and an F1 score of 2%. The low risk precision is showing 100%, with a sensitivity percentage of 65% and F1 Score of 78%.

### SMOTE

![](/images/smote.png)

The SMOTE model is very similar to the model above. The balanced accuracy is 64%. The high risk precision is 1%, with a sensitivity of 62%, and an F1 score of 2%. The low risk precision is at 100%, the sensitivity is at 66%, and an F1 score of 79%.

### ClusterCentroids

![](/images/clustercentroids.png)

The balanced accuracy of the ClusterCentroids model is 51%. The high risk precision is 1%, sensitivity is 59%, and the F1 score is 1%. The low risk precision is 100%, sensitivity is at 44%, and the F1 score is 61%.

### SMOTEENN

![](/images/smoteenn.png)

- Balanced Accuracy:62%
- High Risk Precision:1%
- High Risk Sensitivity:70% 
- High Risk F1 Score:2%
- Low Risk Precision:100%
- Low Risk Sensitivity:54%
- Low Risk F1 Score:70%

### BalancedRandomForestClassifier

![](/images/randomforest.png)

- Balanced Accuracy:79%
- High Risk Precision:3%
- High Risk Sensitivity:70% 
- High Risk F1 Score:6%
- Low Risk Precision:100%
- Low Risk Sensitivity:87%
- Low Risk F1 Score:93%

### EasyEnsembleClassifier

![](/images/ensemble.png)

- Balanced Accuracy:93%
- High Risk Precision:9%
- High Risk Sensitivity:92% 
- High Risk F1 Score:16%
- Low Risk Precision:100%
- Low Risk Sensitivity:94%
- Low Risk F1 Score:97%

## Summary

In regards to determining if a credit risk is high, all of the models have low precision. All of the models exhibit high precision for determining if a credit risk is low. Out of the six models, the Ensemble model is the strongest model to predict High Risk credit risk. The Ensemble model predicts the majority of high risk with a recall percent of 92%. However there were many instances that the model predicited a high risk, but they were actually a low risk. This would negatively impact the bank's reputation when a low risk gets marked as high risk and doesn't get approved for a loan. Customers would begin to go to other banks leading to decline in overall business. Also the high risk F1 Score is only 16%. And while no "good" F1 Score benchmark was provided on a scale of 0 - 100, 16% is still very low. 

All of the models were strong in predicting actual low risk credit risks. However since they all are still weak when trying to predict true high risk credit, even the Ensemble model, for the reasons stated above I would not recommend the bank use any of the models. 
