# Credit Risk Analysis

## Overview
Machine learning can be utilized to predict credit risk. By utilizing it, it will not only provide a quicker and more reliable loan experience but will also lead to a more accurate identification of good candidates for loans, which will lead to lower default rates. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, different techniques need to be employed to train and evaluate models with unbalanced classes. Numerous supervised machine learning models or algorithms have been built and evaluated to predict credit risk. 

### Supervised Machine Learning Models Utilized:
* Naïve Random Oversampling
* SMOTE Oversampling
* Cluster Centroids Undersampling 
* SMOTEENN Combination (Over and Under) Sampling
* Balanced Random Forest Classifier
* Easy Ensemble ADABoost Classifier  

### Resources Utilized to Complete Analysis
* **Data Sources:** 
[LoanStats_2019Q1.CSV](https://github.com/cmmgw/Credit_Risk_Analysis/blob/main/Resources/LoanStats_2019Q1.zip) 

* **Languages:** Python
* **Python Dependencies:** numpy, pandas, pathlib, collections, scikit-learn, imbalanced-learn
* **Tools:** MS Excel, Jupyter Notebook


## Results

### Naïve Random Oversampling

![Classification_Report_Naive_Random_Oversampling](https://github.com/cmmgw/Credit_Risk_Analysis/blob/main/Resources/Classification_Report_Naive_Random_Oversampling.JPG)

* Balanced Accuracy Score: 65.03%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 69% 
* Recall Low Risk: 61%

**Confusion Matrix**
|             | Predicted True  | Predicted False | 
|-------------|------|------|
| Actually True | 70 | 31 |
| Actually False | 6711 | 10393 |



### SMOTE Oversampling

![Classification_Report_SMOTE_Oversampling](https://github.com/cmmgw/Credit_Risk_Analysis/blob/main/Resources/Classification_Report_SMOTE_Oversampling.JPG)

* Balanced Accuracy Score: 66.21%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 63% 
* Recall Low Risk: 69%

**Confusion Matrix**
|             | Predicted True  | Predicted False | 
|-------------|------|------|
| Actually True | 64 | 37 |
| Actually False | 5291 | 11813 |



### Cluster Centroids Undersampling 

![Classification_Report_Cluster_Centroids_Undersampling](https://github.com/cmmgw/Credit_Risk_Analysis/blob/main/Resources/Classification_Report_Cluster_Centroids_Undersampling.JPG)

* Balanced Accuracy Score: 54.42%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 69% 
* Recall Low Risk: 40%

**Confusion Matrix**
|             | Predicted True  | Predicted False | 
|-------------|------|------|
| Actually True | 70 | 31 |
| Actually False | 10340 | 6764 |



### SMOTEENN Combination (Over and Under) Sampling

![Classification_Report_SMOTEENN_Combination_Sampling](https://github.com/cmmgw/Credit_Risk_Analysis/blob/main/Resources/Classification_Report_SMOTEENN_Combination_Sampling.JPG)

* Balanced Accuracy Score: 64.61%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 71% 
* Recall Low Risk: 58%

**Confusion Matrix**
|             | Predicted True  | Predicted False | 
|-------------|------|------|
| Actually True | 72 | 29 |
| Actually False | 7195 | 9909 |



### Balanced Random Forest Classifier

![Classification_Report_Balanced_Random_Forest_Classifier](https://github.com/cmmgw/Credit_Risk_Analysis/blob/main/Resources/Classification_Report_Balanced_Random_Forest_Classifier.JPG)

* Balanced Accuracy Score: 78.85%
* Precision High Risk: 3%
* Precision Low Risk: 100%
* Recall High Risk: 70% 
* Recall Low Risk: 87%

**Confusion Matrix**
|             | Predicted True  | Predicted False | 
|-------------|------|------|
| Actually True | 71 | 30 |
| Actually False | 2153 | 14951 |



### Easy Ensemble ADABoost Classifier  

![Classification_Report_Easy_Ensemble_ADABoost_Classifier](https://github.com/cmmgw/Credit_Risk_Analysis/blob/main/Resources/Classification_Report_Easy_Ensemble_ADABoost_Classifier.JPG)

* Balanced Accuracy Score: 93.16%
* Precision High Risk: 9%
* Precision Low Risk: 100%
* Recall High Risk: 92% 
* Recall Low Risk: 94%

**Confusion Matrix**
|             | Predicted True  | Predicted False | 
|-------------|------|------|
| Actually True | 93 | 8 |
| Actually False | 983 | 16121 |



## Summary
Numerous machinelearning models were utilized to determine which model is the most effective atpredicting credit risk. Accuracy, precision and sensitivity can be assessed by reviewingthe results of each model. The confusion matrix, collates the results of accuracy,precision and sensitivity and can be calculated as follows: 

Accuracy = (TruePositives (TP) + True Negatives (TN)) / Total
Precision = TotalPositives (TP) / (True Positives (TP) + False Positives (FP))
Sensitivity = TotalPositives (TP) / (True Positives (TP) + False Negatives (FN)) 

The analysis highlighted above, indicates that the precisionscores for all the models are overfit. A good balance of recall and precisionis necessary to have an effective model and most of the models lack this. However,the Easy Ensemble ADABoost Classifier model is recommended for use, due to itshigh balanced accuracy score, along with its balance of precision and recall scores.