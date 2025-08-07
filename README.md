# 🩺 Diabetes Prediction using Machine Learning

This project uses multiple machine learning models to predict whether a person is likely to be diabetic based on health indicators such as glucose level, BMI, blood pressure, and more.

---

## 📌 Project Overview

- **Dataset**: [Pima Indians Diabetes Dataset](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
- **Goal**: Predict diabetes (binary classification)
- **Tech Stack**: Python, Pandas, Scikit-learn, XGBoost, Matplotlib, Seaborn, Streamlit

---

## 🔍 Features Used
- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI
- Diabetes Pedigree Function
- Age

---

## ✅ Models Implemented
| Model                 | Accuracy | AUC Score | CV Accuracy |
|----------------------|----------|-----------|--------------|
| Logistic Regression  | ~78%     | ~0.83     | ~75%         |
| Random Forest        | ~81%     | ~0.88     | ~83%         |
| XGBoost              | ~79%     | ~0.85     | ~80%         |
| Decision Tree (Tuned)| ~78%     | ~0.84     | ~78%         |

---

## 🔧 Techniques Used

- Data cleaning (NaN handling, outlier treatment using IQR)
- Feature scaling (`StandardScaler`)
- Class balancing with **SMOTE**
- Hyperparameter tuning using **RandomizedSearchCV**
- Model evaluation using **accuracy**, **AUC score**, **confusion matrix**, **ROC curve**
- Best model exported using `joblib`

---

## 📊 Visualizations

- Histograms & Boxplots (Before/After outlier handling)
- Correlation Heatmap
- Confusion Matrices for all models
- ROC Curve Comparison

---

## 🚀 Streamlit App

You can interact with the trained model using the deployed Streamlit app:
```bash
streamlit run app.py
