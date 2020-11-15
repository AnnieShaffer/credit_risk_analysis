# Credit Risk Analaysis
## Overview
The purpose of this analysis is to create a machine learning model to find loan risk based on several different factors of the applicant history. We used resampling and ensemable learning techniques to test for accuracy, precision, and sensitivity.
## Results
### Naive Random Oversampling
![Naive Random Oversampling](https://github.com/AnnieShaffer/credit_risk_analysis/blob/main/Images/naive_random_oversampling.png)
- The balanced accuracy score is 0.68
- There is a low precision score in predicting high credit risk, and a high precision score in predicting low credit risk
- There is a higher sensitivity to high risk loans at 0.76, than lower risk loans at 0.59
### SMOTE Oversampling
![SMOTE](https://github.com/AnnieShaffer/credit_risk_analysis/blob/main/Images/smote_oversampling.png)
- The balanced accuracy score is 0.66
- There is a low precision score in predicting high credit risk, and a high precision score in predicting low credit risk
- There is a similar recall/sensitivity to both high and low risk loans at 0.63 and 0,69 respectively
### Undersampling
![Undersampling](https://github.com/AnnieShaffer/credit_risk_analysis/blob/main/Images/undersampling.png)
- The balanced accuracy score is 0.55
- There is a low precision score in predicting high credit risk, and a high precision score in predicting low credit risk
- There is a higher recall/sensitivity to high risk loans at 0.68, and a lower recall/sensitivity to low risk loans at 0.41
### Combination (Over and Under) Sampling
![Combination Sampling](https://github.com/AnnieShaffer/credit_risk_analysis/blob/main/Images/combination_sampling.png)
- The balanced accuracy score is 0.66 
- There is a low precision score in predicting high credit risk, and a high precision score in predicting low credit risk
- There is a higher sensitivity to high risk loans at 0.72, than lower risk loans at 0.57
### Balanced Random Forest Classifier
![Random Forest Classifier](https://github.com/AnnieShaffer/credit_risk_analysis/blob/main/Images/random_forest_classifier.png)
- The balanced accuracy score is 0.79
- There is a low precision score in predicting high credit risk, and a high precision score in predicting low credit risk
- There is a higher recall/sensitivity to low risk loans at 0.87, than higher risk loans at 0.70
### Easy Ensamble AdaBoost Classifier
![Easy Ensemble](https://github.com/AnnieShaffer/credit_risk_analysis/blob/main/Images/easy_ensamble_classifier.png)
- The balanced accuracy score is 0.92
- There is a low precision score in predicting high credit risk, and a high precision score in predicting low credit risk
- This test had similar recall/sensitivity scores for both high and low risk loans at 0.93 and 0.90 respectively

## Summary
Most of the models used in this analysis were not very accurate. The resampling models had low balanced accuracy scores from 0.55 to 0.68. Additionally, the recall/sensitivity scores for each of these models was low in almost all cases. On the other hand, the Ensemble Classifiers were much better at predicting the risk of applicants, specifically the Easy Ensemble Classifier. This model was able to predict credit risk accurately at a rate of 92%. If the company needed to use a model immediately, this would be the most accurate model to use, however, the model is still not the great at predicting high risk loans and this could negatively impact the company in many ways.