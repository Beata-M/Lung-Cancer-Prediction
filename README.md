
# 🩺 Lung Cancer Prediction Using Machine Learning

This project explores the application of machine learning models to **predict lung cancer risk** using a dataset of lifestyle, clinical, and environmental variables. Conducted as a final project for the *IA650: Data Mining* course at Clarkson University, it demonstrates a full data science workflow from preprocessing to evaluation.

---

## 📊 Project Overview

- **Objective**: Predict pulmonary disease (a proxy for lung cancer) using ML models and identify key contributing factors.
- **Dataset**: 5,000 patients, 18 features
- **Target Variable**: `Pulmonary Disease` (binary: 0 = No, 1 = Yes)
- **Data Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/shantanugarg274/lung-cancer-prediction-dataset)

---

## 🧠 Key Techniques

- Data Cleaning & Encoding
- Chi-square Test for Association
- PCA for Dimensionality Reduction
- Variance Inflation Factor (VIF) to detect multicollinearity
- Train-test split and 5-fold cross-validation

---

## 🧪 Models Trained

| Model               | Accuracy | F1 Score (Disease Class) | AUC |
|--------------------|----------|---------------------------|-----|
| Logistic Regression | 86%      | 0.83                      | 0.90 |
| SVC (RBF Kernel)    | 86%      | 0.83                      | 0.90 |
| Decision Tree       | 85%      | 0.88                      | 0.86 |
| Random Forest       | 85%      | **0.88**                  | **0.87** |

✅ **Random Forest** had the highest F1 for identifying disease, making it suitable for clinical decision support.

---

## 📈 Feature Importance (Top 5)
- Smoking
- Breathing Issues
- Pollution Exposure
- Stress on Immune System
- Smoking Family History

---

## 📂 Project Structure

```
lung-cancer-prediction/
├── data/                # Raw dataset
├── notebooks/           # Jupyter analysis notebooks (to be added)
├── visuals/             # High-resolution figures (e.g., correlation matrix, VIF)
├── presentation/        # Report and PowerPoint slides
├── README.md
```

---

## 👥 Contributors

- **Beata Tatenda Moyo** – MS in Applied Data Science, Clarkson University
- **Smallman Jimu**

**Course**: IA650 – Data Mining (Spring 2025)  
**Instructor**: Dr. Sumona Mondal

---

## 📬 Contact

For questions or collaboration, feel free to reach out via LinkedIn or GitHub.
