## 📊 Customer Churn Prediction
This project predicts customer churn using machine learning techniques. It is based on a telecom dataset and includes a variety of models (Logistic Regression, Random Forest, Decision Tree) with class imbalance handling strategies such as SMOTE oversampling and class weighting.

## 🚀 Project Overview
Goal: Predict whether a customer will churn (leave the company) or not.

Data: Telecom customer data with demographic, service, and billing information.

Approach: Train multiple models, compare performance, and interpret feature importance for stakeholder insights.

## ⚙️ Features Used
Examples of features:

Gender

Senior Citizen status

Partner

Dependents

Tenure

Phone Service

Multiple Lines

Internet Service

Online Security

Contract Type

Monthly Charges

… and other relevant attributes

## 🧮 Models Applied
✅ Logistic Regression

Baseline model

Tested with and without class balancing (class_weight='balanced')

SMOTE applied to oversample minority class

✅ Random Forest

Tested with standard settings and then with class_weight='balanced'

Tuned with parameters:

n_estimators=500

max_leaf_nodes=30

max_features='sqrt'

Evaluated using ROC curve and AUC

✅ Decision Tree

Tested with and without class balancing

Compared on precision, recall, and f1-score

## 📈 Model Performance
Random Forest (balanced) achieved:

~80% overall accuracy

Class 1 (churn) recall improved to ~0.77

AUC around 0.83

Logistic Regression with SMOTE:

Slightly lower accuracy but better churn recall

Decision Tree:

Simpler but less robust compared to Random Forest

## 🔍 Interpretation
Key insights:

Tenure is highly important (short tenure → higher churn)

Monthly Charges influences churn (higher bills → higher churn)

Contract Type (month-to-month contracts → higher churn)

Feature importance from the Random Forest helps stakeholders prioritize retention strategies.

## 🖥️ How to Run
Clone the repository
Run the notebook:
jupyter notebook ChurnPrediction.ipynb
Explore the results in the notebook (ROC curves, classification reports, feature importance plots).


## 🙌 Acknowledgements
Scikit-learn
imbalanced-learn
Matplotlib, Seaborn, Plotly
