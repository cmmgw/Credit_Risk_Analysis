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

**Confusion Matrix**
|             | Predicted True  | Predicted False | 
|-------------|------|------|
| Actually True | 70 | 31 |
| Actually False | 6711 | 10393 |


•	Balanced Accuracy

### SMOTE Oversampling

**Confusion Matrix**
|             | Predicted True  | Predicted False | 
|-------------|------|------|
| Actually True | 64 | 37 |
| Actually False | 5291 | 11813 |



### Cluster Centroids Undersampling 

**Confusion Matrix**
|             | Predicted True  | Predicted False | 
|-------------|------|------|
| Actually True | 70 | 31 |
| Actually False | 10340 | 6764 |


### SMOTEENN Combination (Over and Under) Sampling

**Confusion Matrix**
|             | Predicted True  | Predicted False | 
|-------------|------|------|
| Actually True | 72 | 29 |
| Actually False | 7195 | 9909 |


### Balanced Random Forest Classifier

**Confusion Matrix**
|             | Predicted True  | Predicted False | 
|-------------|------|------|
| Actually True | 71 | 30 |
| Actually False | 2153 | 14951 |


### Easy Ensemble ADABoost Classifier  

**Confusion Matrix**
|             | Predicted True  | Predicted False | 
|-------------|------|------|
| Actually True | 93 | 8 |
| Actually False | 983 | 16121 |



## Summary
