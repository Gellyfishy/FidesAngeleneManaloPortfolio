# ❤️ Heart Disease Prediction – Healthcare Capstone Project (Xaltius)

This capstone project explores a machine learning application in healthcare: predicting the presence of heart disease based on demographic, clinical, and lifestyle factors. The goal is to assist in early detection and preventive care by using data science methodologies on real patient data.

---

## 🎯 Project Objective

To build and evaluate a machine learning model that can predict whether an individual has heart disease using various health-related features, including blood pressure, cholesterol, glucose levels, and lifestyle habits.

---

## 📊 Dataset Overview

- **Source**: Healthcare dataset from Parkway Pantai (anonymized)
- **Target**: `disease` (1 = heart disease, 0 = no heart disease)
- **Features**:
  - Demographic: Age, Gender
  - Clinical: Systolic BP (`ap_hi`), Cholesterol, Glucose
  - Lifestyle: Smoking, Alcohol use, Physical activity
  - Dropped: `id`, `country`, `date` (non-informative)

---

## 🧹 Data Preparation

- No missing values or duplicates found
- Non-informative columns dropped
- Dataset split: 80% train, 20% test
- Scaled features as needed for certain models

---

## 📊 Exploratory Data Analysis (EDA)

- Half the dataset showed no heart disease
- High correlation between `ap_hi`, cholesterol, age, and disease presence
- Feature distributions visualized to assess variable importance

---

## 🤖 Modeling Techniques Used

| Model               | Accuracy | ROC-AUC |
|--------------------|----------|---------|
| Logistic Regression| 73.19%   | 0.782   |
| XGBoost            | 72.54%   | **0.795** |
| Support Vector Machine | 71.66% | 0.778 |
| Random Forest      | 71.39%   | 0.772   |
| Decision Tree      | 63.15%   | 0.631   |

- **Best Model**: XGBoost (highest ROC-AUC and robust accuracy)
- **Baseline**: Logistic Regression
- **Weakest**: Decision Tree

---

## 🔍 Feature Importance

Top predictors across multiple models:
- `Systolic Blood Pressure (ap_hi)`
- `Age`
- `Weight`
- `Height`
- `Cholesterol`

---

## 📈 ROC Curve Insights

- XGBoost achieved the highest area under the ROC curve
- ROC-AUC used due to binary classification and class balance concerns
- Logistic Regression was interpretable but underperformed vs. boosting models

---

## ✅ Recommendations & Future Work

- **Deploy XGBoost** in critical-care predictive systems for optimal performance
- Use Logistic Regression or Random Forest where **interpretability** is a must
- Future enhancements:
  - Add features like exercise, diet, medication use, and family history
  - Tune hyperparameters for complex models (e.g., XGBoost, SVM)
  - Apply k-fold cross-validation for stronger generalization
  - Address future class imbalance with SMOTE or class weighting

---

## 🧰 Tools & Technologies

- Python (`pandas`, `sklearn`, `xgboost`, `matplotlib`, `seaborn`)
- Jupyter Notebook
- PowerPoint (for capstone presentation)

---

## 📁 Files Included

- `heart_disease_prediction.ipynb` – Main Jupyter notebook
- `Manalo_CAPSTONE3 - Healthcare Dataset.pptx` – Final presentation
- `cleaned_health_data.csv` – Processed dataset (optional)
- `README.md` – Project documentation

---

## 📫 Contact

**Fides Angelene R. Manalo**  
📧 fidesangelenemanalo@gmail.com  
🔗 [LinkedIn](your-linkedin-url-here)
