# Credit Card Fraud Detection Analysis

## 📌 Project Overview
This project uses **Logistic Regression** to identify fraudulent credit card transactions. Given the highly imbalanced nature of fraud data, this model focuses on balancing precision and recall to minimize financial risk.

## 📊 Model Performance Metrics
* **Accuracy:** 99.90%
* **Precision:** 80.95% (When we predict fraud, we are right 81% of the time)
* **Recall:** 70.83% (We caught 71% of all actual fraud)
* **F1-Score:** 0.7556
* **ROC AUC Score:** 0.9769

## 🔍 Confusion Matrix Interpretation
Based on the test set of 34,093 transactions:
* **True Negatives:** 34,009 (Correctly identified as safe)
* **False Positives:** 12 (Safe transactions flagged as fraud - Type I Error)
* **False Negatives:** 21 (Fraudulent transactions missed - Type II Error)
* **True Positives:** 51 (Fraudulent transactions caught)

## 💡 Conclusion & Next Steps
The model is highly effective but has room for improvement in **Recall**. In fraud detection, missing 21 fraudulent transactions (False Negatives) is more costly than 12 false alarms. 

1. Implementing **SMOTE** to handle class imbalance.
2. Testing **Random Forest** or **XGBoost** classifiers.
