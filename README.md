# Customer Churn Prediction 🚧

Ongoing machine learning project focused on predicting customer churn in a
telecommunications setting using the Telco Customer Churn dataset.
The project emphasizes imbalanced data handling and decision threshold optimization
with business-aware evaluation metrics.

> **Status:** 🚧 Ongoing Project  
> This repository is actively being developed and continuously improved.

---

## 📌 Project Overview

Customer churn prediction is formulated as a binary classification problem.
The objective is to identify customers who are likely to leave the service and
enable proactive, data-driven retention strategies.

The project emphasizes not only model performance, but also:
- Proper handling of class imbalance
- Decision threshold optimization beyond the default 0.5
- Business-aware evaluation using F1-score, precision, and recall

---

## 🧠 Methodology

- Exploratory Data Analysis (EDA)
- Feature encoding and selection
- Baseline model: Logistic Regression
- Tree-based models:
  - Decision Tree
  - Random Forest
  - XGBoost (with SMOTE and class weighting)
- Hyperparameter tuning using GridSearchCV
- Decision threshold optimization based on F1-score

---

## 📊 Evaluation Strategy

Due to class imbalance, accuracy is not used as the primary evaluation metric.
Instead, the following metrics are prioritized:
- F1-score
- Recall (churn class)
- Precision

Decision thresholds are optimized to balance precision and recall,
which is critical in churn prediction where false negatives are costly.

---

## 🏆 Current Best Model

- **Model:** XGBoost with `scale_pos_weight`
- **Reason:** Best balance between precision, recall, and F1-score
- **Deployment-friendly:** No synthetic data generation

---

## 🚀 Future Work

- Model comparison table and visualizations
- Probability calibration analysis
- Business cost–sensitive evaluation
- Deployment as an interactive dashboard

---

## 📁 Repository Structure

```text
customer-churn-prediction/
│
├── Customer_Churn_Prediction.ipynb
├── WA_Fn-UseC_-Telco-Customer-Churn.csv
├── README.md
└── .gitignore
