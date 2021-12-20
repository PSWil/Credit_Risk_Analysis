# Credit_Risk_Analysis

## Overview

The purpose of this analysis was to create a supervised machine learning model that could accurately predict credit risk. In order to complete this task, I used 6 different methods:

1. Naive Random Oversampling
2. SMOTE Oversampling
3. Cluster Centroid Undersampling
4. SMOTEENN Sampling
5. Balanced Random Forest Classifying
6. Easy Ensemble Classifying

## Results

### Naive Random Oversampling

* Accuracy Score: 67.3%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 66%
* Recall Low Risk: 68%

![oversampling](https://github.com/PSWil/Credit_Risk_Analysis/blob/main/Images/oversampling.png)

### SMOTE Oversampling

* Accuracy Score: 67%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 70%
* Recall Low Risk: 64%

![SMOTE](https://github.com/PSWil/Credit_Risk_Analysis/blob/main/Images/smote.png)

### Cluster Centroid Undersampling

* Accuracy Score: 52%
* Precision High Risk: 0%
* Precision Low Risk: 100%
* Recall High Risk: 61%
* Recall Low Risk: 44%

![undersampling](https://github.com/PSWil/Credit_Risk_Analysis/blob/main/Images/undersampling.png)

### SMOTEENN Sampling

* Accuracy Score: 68%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 76%
* Recall Low Risk: 60%

![SMOTEENN](https://github.com/PSWil/Credit_Risk_Analysis/blob/main/Images/smoteenn.png)

### Balanced Random Forest Classifying

* Accuracy Score: 65%
* Precision High Risk: 56%
* Precision Low Risk: 100%
* Recall High Risk: 30%
* Recall Low Risk: 100%

![random_forest](https://github.com/PSWil/Credit_Risk_Analysis/blob/main/Images/random_forest.png)

### Easy Ensemble Classifying

* Accuracy Score: 92%
* Precision High Risk: 6%
* Precision Low Risk: 100%
* Recall High Risk: 91%
* Recall Low Risk: 94%

![easy_ensemble](https://github.com/PSWil/Credit_Risk_Analysis/blob/main/Images/easy_ensemble.png)

## Summary

This analysis is trying to find the best model that can detect if a loan is high risk or not. Becasue of that, we need to find a model that lets the least amount of high risk loans pass through undetected. That correlating statistic for this is the recall rate for high risk. Looking through the different models, the ones that scored the highest were:

1. Easy Ensemble Classifying (91%)
2. SMOTEENN Sampling (76%)
3. Naive Random Oversampling (72%)

While this is the most important statistic that is pulled from this analysis, another important statistic is recall rate for low risk as it shows how many low risk loans are flagged as high risk. Looking through the different models, the ones that scored the highest were:

1. Balanced Random Forest Classifying (100%)
2. Easy Ensemble Classifying (94%)

After taking these two statistics over the others, we can look at the accurary score to get a picture of how well the model performs in general. The models with the highest accuracy scores were:

1. Easy Ensemble Classify (92%)
2. SMOTEENN Sampling (68%)
3. Balanced Random Forest Classifying (65%)

While some of the above machine learning models outperform others, I recommend more research be done to identify machine learning models that yield better prediction success.

However, in a scenario where limited to the options above, I'd recommend the Easy Ensemble model. Each of its scores reveal it most likely to accurately identify and predict high risk loan applications.
