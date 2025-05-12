#  Stroke Risk Prediction Using Machine Learning

This repository contains the implementation of machine learning models to predict the risk of stroke using demographic, behavioral, and clinical data. The models aim to support early diagnosis and proactive medical intervention, improving patient outcomes and reducing the burden of long-term disability.

---

##  Project Motivation

Stroke is a leading cause of death and disability globally. Early identification of individuals at high risk allows for timely medical interventions and preventive measures. With the digitization of healthcare data, machine learning (ML) has emerged as a powerful tool to predict health risks with high accuracy.

---

##  Dataset

- **Source:** Publicly available dataset  
- **Features Used:**
  - Age  
  - Hypertension  
  - Heart Disease  
  - Type of Work  
  - Smoking Status  
  - Body Mass Index (BMI)

---

## 🛠️ Preprocessing Steps

- Handling **class imbalance** using **SMOTE** (Synthetic Minority Over-sampling Technique)
- **Feature normalization** using `MinMaxScaler`
- **Feature selection** using correlation and feature importance methods

---

##  Models Implemented

| Model               | Accuracy (%) |
|--------------------|--------------|
| Logistic Regression| ~90          |
| Random Forest      | ~95          |
| LightGBM           | ~95          |
| XGBoost            | **~96** ✅   |
| Voting Classifier  | ~95          |

- **XGBoost** achieved the highest accuracy and generalizability
- **Random Forest** provided high interpretability via feature importance
- **Voting Classifier** ensemble improved model stability
- **Logistic Regression** served as a strong baseline

---

##  Evaluation

Models were evaluated using:
- **Confusion Matrix**
- **Precision, Recall, F1-Score**
- **Balanced Accuracy**

Visuals and plots such as ROC curves and feature importance graphs are available in the [`reports/`](./reports/) and [`images/`](./images/) directories.

