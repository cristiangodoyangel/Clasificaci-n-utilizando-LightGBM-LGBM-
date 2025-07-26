# 🏦 Loan Prediction Classifier - LightGBM

Este proyecto implementa un pipeline completo de Machine Learning utilizando **LightGBM (LGBM)** para predecir si un solicitante será aprobado o rechazado para un préstamo, basado en características personales y financieras.

---

## 📌 Objetivo

Predecir la variable `Loan_Status` (Aprobado / No aprobado) a partir de variables como ingresos, historial crediticio, educación y condiciones del préstamo.

---

## 🗂️ Dataset

- **Nombre:** Loan Prediction Dataset  
- **Fuente:** [Kaggle - Loan Prediction Problem](https://www.kaggle.com/)
- **Columnas clave:**
  - `ApplicantIncome`, `CoapplicantIncome`
  - `LoanAmount`, `Loan_Amount_Term`
  - `Credit_History`, `Education`, `Self_Employed`, etc.

---

## ⚙️ Tecnologías y Librerías

- Python 3.x
- Pandas
- Seaborn & Matplotlib
- Scikit-learn
- LightGBM
- GridSearchCV

---

## 🧠 Pipeline Desarrollado

### 1. **Carga y Exploración de Datos**
- Análisis estructural 
- Detección de nulos y outliers

### 2. **EDA - Análisis Exploratorio**
- Histogramas, gráficos de barras, dispersión y correlación
- Insights relevantes de distribución y relación entre variables

### 3. **Preprocesamiento**
- Imputación de valores nulos
- One-Hot Encoding para variables categóricas
- Escalado con `StandardScaler`
- División `train/test` (80/20)

### 4. **Modelo**
- Entrenamiento inicial con `LGBMClassifier`
- Métricas: Accuracy, Precision, Recall, F1, ROC-AUC
- Optimización de hiperparámetros con `GridSearchCV`

---

## 📈 Resultados

- Buen rendimiento del modelo base
- Mejora tras optimización con GridSearchCV
- `Credit_History` e `Income` fueron variables determinantes

---

## 📌 Conclusiones

- LightGBM demostró ser rápido, robusto y eficiente para este tipo de problema tabular.
- El análisis previo (EDA y limpieza) fue clave para un modelo exitoso.
- Hay oportunidades para seguir mejorando el rendimiento con balanceo de clases y otras técnicas avanzadas.

---

## 📁 Estructura del proyecto

📦 loan-prediction-lightgbm
├── data/
│ └── train.csv
├── notebook/
│ └── loan_prediction_lgbm.ipynb
├── README.md
└── requirements.txt
