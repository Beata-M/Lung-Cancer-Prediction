# 🩺 Lung Cancer Prediction Using Machine Learning

This project presents a comprehensive machine learning approach to predicting lung cancer risk based on demographic, lifestyle, and clinical features. Conducted as a capstone project for the IA650 Data Mining course at Clarkson University, it integrates data preprocessing, exploratory analysis, statistical tests, and supervised learning models.

---

## 📘 Project Summary

Lung cancer is a leading cause of cancer-related mortality globally, largely due to late diagnosis. Our project leverages machine learning to build a predictive model for early detection of pulmonary disease—a proxy for lung cancer—using data from 5,000 individuals collected between 2018 and 2022.

We explored multiple classification algorithms to identify high-risk individuals based on features such as smoking habits, pollution exposure, immune system status, and oxygen saturation.

---

## 📊 Dataset Overview

- **Source**: [Kaggle: Lung Cancer Prediction Dataset](https://www.kaggle.com/datasets/shantanugarg274/lung-cancer-prediction-dataset)
- **Size**: 5,000 patient records
- **Features**: 18 attributes (categorical, ordinal, and numerical)
- **Target Variable**: `Pulmonary Disease` (Binary: 1 = Disease, 0 = No Disease)

### Key Features:
- Age, Gender
- Smoking & Alcohol use
- Pollution exposure
- Stress on Immune System
- Breathing issues, Throat discomfort
- Oxygen saturation (SpO2)

---

## 🔍 Methods

### 📌 Data Preprocessing
- One-hot encoding for categorical variables
- Min-max normalization for ordinal variables
- Chi-square tests for feature significance
- PCA for dimensionality reduction
- Variance Inflation Factor (VIF) for multicollinearity assessment

### 📌 Feature Engineering
- Top predictors included **Smoking**, **Pollution**, **Breathing Issue**, **Stress Immune**, and **Smoking Family History**
- PCA retained 82% of variance in 4 components
- VIF values < 5 for all predictors → No multicollinearity

---

## 🤖 Machine Learning Models

| Model               | Accuracy | Disease F1 Score | AUC |
|--------------------|----------|------------------|-----|
| Logistic Regression | 86%      | 0.83             | 0.90 |
| Support Vector Classifier | 86% | 0.83             | 0.90 |
| Decision Tree       | 85%      | 0.88             | 0.86 |
| Random Forest (Tuned) | 85%    | **0.88**         | **0.87** |

- **Logistic Regression**: Interpretable model; strong precision for 'No Disease'
- **SVC (RBF)**: High accuracy; effective for non-linear data
- **Decision Tree**: High F1 for 'Disease'; prone to overfitting
- **Random Forest**: Best overall F1 score and balance; tuned via GridSearchCV

---

## 📈 Visual Results

Key plots included:
- 📊 Correlation Matrix of Features
- 📉 PCA Component Scree Plot
- 🧪 VIF Lollipop Plot
- 📉 Logistic Regression Coefficients
- 🟦 ROC Curves for all models

![Correlation_Matrix_HighRes](https://github.com/user-attachments/assets/b5bb44c2-deda-4549-a875-917866ea8857)

![VIF_Lollipop_HighRes_v2](https://github.com/user-attachments/assets/04c378fd-d4ad-474c-bc72-4ff418166966)

---

## 🧠 Insights

- Smoking increases disease odds by **~30x**
- Pollution and immune stress are significant compounding factors
- Tree-based models (especially Random Forest) perform best at identifying disease
- Logistic Regression remains useful for clinical interpretability

---

## 📂 Repository Structure

```
lung-cancer-prediction/
├── data/                 # Dataset file (.csv)
├── notebooks/            # (To be added) Jupyter notebooks
├── visuals/              # High-resolution analysis visuals
├── presentation/         # Presentation & Final Report (PDF)
├── README.md             # Project documentation
```

---

## 👥 Contributors

- **Beata Tatenda Moyo** — MS Applied Data Science, Clarkson University
- **Smallman Jimu** — IA650 Project Partner

Supervised by: **Dr. Sumona Mondal**  
Course: **IA650 – Data Mining (Spring 2025)**

---

## 📬 Contact

For questions or collaboration opportunities, connect with us via [LinkedIn](https://linkedin.com) or through this GitHub profile.
