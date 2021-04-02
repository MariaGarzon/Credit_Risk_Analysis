# Predicting Credit Risk

## Overview

In 2019, more than 19 million Americans had at least one unsecured personal loan. Personal lending is growing faster than credit card, auto, mortgage, and even student debt. With such incredible growth, being able to predict credit risk with machine learning algorithms can help banks and financial institutions predict anomalies, reduce risk cases, monitor portfolios, and provide recommendations on what to do in cases of fraud. 

In this project, the following machine learning models were built and evaluated using Python to predict credit risk: 

  1) Naive Random Oversampling
  2) SMOTE Oversampling
  3) Cluster Centroid Undersampling
  4) SMOTEENN Sampling
  5) Balanced Random Forest Classifying
  6) Easy Ensemble Classifying

## Resources

- Software: Visual Studio Code 1.39.0, Jupyter Notebook 6.0.3
- Languages: Python 3.7
- Libraries: Numpy 1.17.4, scikit-learn 0.22.1

## Results

### Balanced Random Forest Classifying

- Accuracy Score: 66.8%
- Precision High Risk: 60%
- Precision Low Risk: 100%
- Recall High Risk: 34%
- Recall Low Risk: 100%


![Balance RFC](https://github.com/MariaGarzon/Credit_Risk_Analysis/blob/f21a66a50991c1a90eb54cc807c563edc37d13ae/Visuals/Balanced%20RFC.png)

### Easy Ensemble Classifying

- Accuracy Score: 92.9%
- Precision High Risk: 6.0%
- Precision Low Risk: 100%
- Recall High Risk: 92%
- Recall Low Risk: 94%

![Easy Ensemble](https://github.com/MariaGarzon/Credit_Risk_Analysis/blob/f21a66a50991c1a90eb54cc807c563edc37d13ae/Visuals/Easy_Assemble_AdaBoost.png)

### Naive Random Oversampling

- Accuracy Score: 69.0%
- Precision High Risk: 1.0%
- Precision Low Risk: 100%
- Recall High Risk: 76%
- Recall Low Risk: 63%

![Naive Random](https://github.com/MariaGarzon/Credit_Risk_Analysis/blob/f21a66a50991c1a90eb54cc807c563edc37d13ae/Visuals/Naive_Random.png)

### SMOTE Oversampling

- Accuracy Score: 67.6%
- Precision High Risk: 1%
- Precision Low Risk: 100%
- Recall High Risk: 68%
- Recall Low Risk: 68%

![SMOTE](https://github.com/MariaGarzon/Credit_Risk_Analysis/blob/f21a66a50991c1a90eb54cc807c563edc37d13ae/Visuals/SMOTE.png)

### Cluster Centroid Undersampling

- Accuracy Score: 67.6%
- Precision High Risk: 0.0%
- Precision Low Risk: 100%
- Recall High Risk: 61%
- Recall Low Risk: 43%

![Cluster_Centroid](https://github.com/MariaGarzon/Credit_Risk_Analysis/blob/f21a66a50991c1a90eb54cc807c563edc37d13ae/Visuals/Cluster_Centroids.png)

### SMOTEENN Sampling

- Accuracy Score: 65.7%
- Precision High Risk: 1.0%
- Precision Low Risk: 100%
- Recall High Risk: 78%
- Recall Low Risk: 55%

![SMOTEEN](https://github.com/MariaGarzon/Credit_Risk_Analysis/blob/f21a66a50991c1a90eb54cc807c563edc37d13ae/Visuals/SMOTEENN.png)

## Conclusion and Recommendations

Recall refers to the percentage of total relevant results correctly classified by our algorithm.

In order to minimize the risk of fraud, we need a model with a high recall rate for high risk.  
The models that scored the highest for it were:

1) Easy Ensemble Classifying (92%)
2) SMOTEENN Sampling (78%)
3) Naive Random Oversampling (76%)

The Easy Ensemle Adaboost Classifier has the highest coefficients for predicting both low-risk and high risk loan status, and highest accouracy score. Therefore, we recommend using this model for further analysis. 
