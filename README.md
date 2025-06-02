# 🧠 Stroke Prediction Using Machine Learning

This project aims to predict the likelihood of a patient having a stroke using clinical and demographic data, leveraging machine learning models. The goal is to provide early warnings that support preventive healthcare decisions.

## 📊 Problem Statement

Stroke is a leading cause of death and long-term disability worldwide. Traditional clinical risk assessment tools can miss complex interactions between risk factors. This project investigates whether machine learning can better identify patients at risk of stroke—**before symptoms appear.**

---

## 📁 Project Structure

**Source**: Public dataset with 4,981 patient records  
- **Target**: `stroke` (1 = stroke, 0 = no stroke)
- **Features**:
  - Age, Gender, BMI
  - Average glucose level
  - Hypertension, Heart disease
  - Smoking status, Work type, Residence type
 
  Imbalanced classes: ~5% of records indicate a stroke.

  ## 🛠️ Methods

- **Exploratory Data Analysis (EDA)**:
  - Correlation heatmap
  - Distribution plots by stroke status

- **Preprocessing**:
  - One-hot encoding of categorical variables
  - Imbalance handled with **SMOTE**

- **Models**:
  - Logistic Regression
  - Random Forest
  - XGBoost
 
  - - **Threshold Tuning**:
  - Selected threshold = **0.2** to optimize **recall** without sacrificing too much precision

---

## 📈 Evaluation Metrics

- **Precision**, **Recall**, **F1-Score**, **PR AUC**
- Confusion Matrix
- Precision-Recall Curve  
- Final Model: **XGBoost (threshold 0.2)**
  - Precision: 19%
  - Recall: 34%
  - F1-Score: 24%

---

## 🔬 Feature Importance

- Top 3 predictive features:
  - **Age**
  - **Average glucose level**
  - **BMI**

SHAP values will be explored in future work for better explainability.

---

## 🔍 Future Improvements

- Add more clinical variables (e.g., blood pressure, medications)
- Validate on external datasets
- Integrate SHAP for model interpretability
- Pilot deployment in clinical environments

---

## ⚖️ Ethical Considerations

- Balanced model sensitivity vs. specificity
- Patient data privacy
- Risk of false positives/negatives
- Commitment to fairness and transparency in predictions

---

## 💡 Quote

> *“Prediction is not just about algorithms — it’s about saving lives.”*

---
