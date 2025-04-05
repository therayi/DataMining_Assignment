# Breast Cancer - Logistic Regression, Decision Tree & Random Forest
## Overview
This project applies three classification algorithms — Logistic Regression, Decision Tree, and Random Forest — to the Breast Cancer Wisconsin (Diagnostic) Dataset to classify tumors as Malignant or Benign. The goal is to compare their performance and effectiveness in terms of accuracy and robustness.

🔹 Logistic Regression
A linear model for binary classification. It estimates the probability that a data point belongs to a certain class using the sigmoid function. It’s simple, interpretable, and effective for linearly separable data.

🔹 Decision Tree
A non-linear model that splits data using feature thresholds, forming a tree-like structure. It is intuitive and interpretable but prone to overfitting on noisy datasets.

🔹 Random Forest
An ensemble technique that builds multiple decision trees and aggregates their predictions for more robust and accurate classification. It reduces overfitting and performs well on complex datasets.

## Dataset
Source: UCI Machine Learning Repository
<br>Size: 569 instances, 30 numerical features
<br>Target: Diagnosis (M = Malignant, B = Benign)
![image](https://github.com/user-attachments/assets/bce86d66-0be2-4192-8aa8-482640d90d3b)

## Preprocessing
Dropped non-informative ID column
<br>Encoded Diagnosis (M = 1, B = 0)
<br>Standardized features using StandardScaler
<br>Stratified 80-20 train-test split for balanced evaluation

## Models Applied
Logistic Regression
<br>Linear classifier, interpretable
<br>Decision Tree
<br>Non-linear, interpretable, risk of overfitting
<br>Random Forest
<br>Ensemble of decision trees, reduces variance and improves accuracy

## Evaluation Metrics
Used to assess model performance:
<br>Accuracy – Overall correctness.
<br>Precision – Quality of positive predictions.
<br>Recall – Coverage of actual positives.
<br>F1 Score – Balance between precision and recall.

![image](https://github.com/user-attachments/assets/5dfb5bea-42fd-4d73-bedd-4d9ba9cf4419)

## Plots & Visualizations
✅ Confusion Matrix (All Models)
<br>Displays True/False Positives and Negatives. Helps visually verify the model’s performance.
![image](https://github.com/user-attachments/assets/f31460b7-87ab-4ea9-b6fc-612a419645c3)
![image](https://github.com/user-attachments/assets/98f398d8-e540-44d0-be03-1696db0781c5)
![image](https://github.com/user-attachments/assets/eff7ee31-44d0-4da8-baba-ac596e16c7d4)

✅ ROC Curve & AUC (All Models)
<br>ROC curves show trade-off between TPR and FPR.
![image](https://github.com/user-attachments/assets/511d70a0-346c-478f-b6dd-380eeb462706)
<br>AUC (Area Under the Curve) closer to 1.0 indicates strong classification ability.
<br>Random Forest had the highest AUC.

✅ Correlation Heatmap (Data Preprocessing)
<br>Helps detect multicollinearity and feature relationships.
![image](https://github.com/user-attachments/assets/30106e12-5952-4c6c-8270-4119d5e19e3e)

✅ Pairplot
<br>Visualizes class separability using feature combinations.
![image](https://github.com/user-attachments/assets/3d53ff2d-53bd-4d44-b199-801544d59085)

## Comparison of Models
![image](https://github.com/user-attachments/assets/1caaa858-c581-46ec-98f4-918b30f93dce)

## Key Insights
Random Forest provided the best performance with high robustness and accuracy.
<br>Decision Tree was simple and explainable but prone to overfitting.
<br>Logistic Regression served as a strong linear baseline with high interpretability.

## References
<br>1. Breiman, L. (2001). Random forests, Machine Learning.
<br>2. Hosmer, D.W., et al. (2013). Applied Logistic Regression.
<br>3. Quinlan, J.R. (1986). Induction of Decision Trees.
<br>4. Scikit-learn documentation: https://scikit-learn.org
<br>5. UCI Dataset: https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)
