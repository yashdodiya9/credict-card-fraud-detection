# Credit Card Fraud Detection

This project demonstrates a machine learning pipeline to detect fraudulent credit card transactions. It tackles the challenge of a highly imbalanced dataset using SMOTE and evaluates multiple models including Logistic Regression, Random Forest, and XGBoost.

---

## Dataset

- Source: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- Total transactions: **284,807**
- Fraudulent transactions: **492** (~0.17% => highly imbalanced dataset)

**Note:** The dataset (`creditcard.csv`) is too large for GitHub and is excluded from the repository.  
To run the project locally, please [download it from Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

---

## Techniques Used

- **Preprocessing**
  - Feature scaling using `StandardScaler`
- **Handling Imbalance**
  - SMOTE (Synthetic Minority Oversampling Technique)
- **Models Implemented**
  - Logistic Regression
  - Random Forest
  - XGBoost
- **Evaluation**
  - Confusion Matrix
  - Classification Report
  - ROC-AUC Score
  - ROC Curve Plot

---

## Model Performance Summary

| Model              | ROC-AUC | Recall (Fraud) | Precision (Fraud) |
|-------------------|---------|----------------|-------------------|
| Logistic Regression | 0.9688 | 0.84           | 0.90              |
| Random Forest       | 0.9629 | 0.84           | 0.90              |
| XGBoost             | 0.9724 | 0.89           | 0.72              |

XGBoost had the highest AUC and fraud recall, indicating better fraud detection capability.

---

