# 🏦 Loan Default Prediction – Finance Capstone Project (Xaltius Academy)

This capstone project explores a real-world financial scenario: using machine learning to predict whether a borrower will default on a loan. The project uses historical data from Bajaj Finserv and applies several supervised learning models to identify high-risk borrowers based on financial and demographic features.

---

## 🎯 Objectives

- Predict if a borrower will default or not using historical loan data
- Apply machine learning models and evaluate performance
- Identify top risk indicators to improve lending decisions

---

## 📊 Dataset Overview

- **Records**: ~5,000 loan records  
- **Features**: 17 total including loan type, amount, interest rate, term, credit score, income level, employment type, and dates  
- **Target**: `default_status` (binary classification: Default or No Default)

---

## 🧹 Data Cleaning & Feature Engineering

- Dropped `customer_id` and `loan_id` (non-informative)
- Converted date fields into numerical durations:
  - `processing_days` (application → approval)
  - `loan_duration_days` (disbursement → due date)
- Encoded categorical variables
- Scaled numerical features for model compatibility

---

## 🤖 Models Used

| Model              | Purpose                            |
|-------------------|-------------------------------------|
| Logistic Regression | Baseline model, simple & interpretable |
| Random Forest       | Handles non-linear patterns        |
| XGBoost             | High-accuracy boosting algorithm   |
| LightGBM            | Efficient gradient boosting with better speed |

---

## 📈 Performance Summary

- **Class Imbalance**: Models were biased toward non-defaulters (majority class)
- **Best AUC**: XGBoost & LightGBM (~0.70+)
- **Best Model**: **LightGBM** — good AUC, faster than XGBoost
- **Weakest Model**: Logistic Regression (AUC ≈ 0.50, poor recall)

> ⚠️ **Recall** was a key focus: catching defaulters is more important than overall accuracy in this context.

---

## 🔍 Feature Importance

Top 5 Predictive Features:
1. `interest_rate`
2. `loan_amount`
3. `loan_duration_days`
4. `loan_term`
5. `processing_days`

> These features consistently ranked high across Random Forest, XGBoost, and LightGBM — making them strong indicators of default risk.

---

## ✅ Recommendations

- Use **SMOTE** or **ADASYN** to handle class imbalance
- Apply **threshold tuning** to increase sensitivity to defaulters
- Try **cost-sensitive learning** to penalize misclassification of high-risk borrowers
- Fine-tune hyperparameters for boosted models (LightGBM, XGBoost)

---

## 🧰 Tools & Technologies

- Python (pandas, numpy, matplotlib, seaborn)
- scikit-learn, xgboost, lightgbm
- Jupyter Notebook
- PowerPoint (presentation)

---

## 📁 Files Included

- `loan_default_prediction.ipynb` – Jupyter Notebook with full code
- `Manalo_CAPSTONE1 - Finance Dataset.pptx` – Final capstone presentation
- `README.md` – Project documentation

---

## 📫 Contact

**Fides Angelene R. Manalo**  
📧 fidesangelenemanalo@gmail.com  
🔗 https://www.linkedin.com/in/fides-angelene-manalo-da/
