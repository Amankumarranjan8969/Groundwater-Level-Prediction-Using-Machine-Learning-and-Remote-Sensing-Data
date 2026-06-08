# 🌍 Groundwater Level Prediction using Machine Learning

## 📌 Overview

This project predicts **monthly groundwater levels** using Machine Learning, Remote Sensing, and Hydro-Meteorological data. The model learns relationships between climate variables, vegetation indices, soil moisture, rainfall patterns, and historical groundwater observations to forecast groundwater fluctuations.

The project also incorporates **Explainable AI (SHAP)** to understand the factors driving groundwater level changes.

---

## 🚀 Features

- Groundwater Level Forecasting
- Temporal Feature Engineering using Lag Features
- Remote Sensing Data Integration
- Explainable AI using SHAP
- Comparative Machine Learning Analysis
- End-to-End Prediction Pipeline

---

## 📊 Dataset Features

### Input Variables

| Feature | Description |
|----------|-------------|
| Latitude | Geographic Coordinate |
| ET_Mon | Monthly Evapotranspiration |
| RH_Mon | Monthly Relative Humidity |
| Wind_Mon | Monthly Wind Speed |
| NDVI_Mon | Vegetation Index |
| NDMI_Mon | Moisture Index |
| SM_100cm_Mon | Soil Moisture at 100 cm Depth |
| GWL_lag_1 | Previous Month Groundwater Level |
| GWL_lag_2 | Groundwater Level Two Months Earlier |
| Rain_lag_1 | Previous Month Rainfall |
| Rain_lag_2 | Rainfall Two Months Earlier |
| Rain_roll3 | Three-Month Rolling Rainfall Average |
| Temp_Avg | Average Monthly Temperature |

### Target Variable

```text
GWL_Mon (Monthly Groundwater Level)
```

---

## ⚙️ Workflow

```text
Data Collection
        ↓
Data Cleaning
        ↓
Missing Value Treatment
        ↓
Feature Engineering
        ↓
Lag Feature Generation
        ↓
Model Training
        ↓
Model Evaluation
        ↓
SHAP Analysis
        ↓
Groundwater Prediction
```

---

## 🧠 Models Used

### Random Forest Regressor

An ensemble learning model that combines multiple decision trees to improve prediction stability and reduce overfitting.

### XGBoost Regressor

A gradient boosting model capable of capturing complex nonlinear relationships in groundwater systems.

---

## 📈 Results

| Model | R² Score |
|---------|---------|
| Random Forest | 0.4067 |
| XGBoost | 0.4134 |

### Random Forest Metrics

| Metric | Value |
|----------|----------|
| MAE | 2.365 |
| MSE | 9.760 |
| RMSE | 3.124 |

---

## 🔍 Explainable AI

SHAP (SHapley Additive Explanations) was used to:

- Interpret model predictions
- Identify influential groundwater drivers
- Improve transparency and trust in the model

---

## 🛠️ Technology Stack

```text
Python
Pandas
NumPy
Scikit-Learn
XGBoost
SHAP
Matplotlib
Seaborn
Jupyter Notebook
```

---

## 📂 Project Structure

```text
Groundwater-Level-Prediction/
│
├── data/
│
├── notebooks/
│   └── model_training.ipynb
│
├── models/
│   └── best_model.pkl
│
├── results/
│   ├── feature_importance.png
│   ├── shap_summary.png
│   └── prediction_plot.png
│
├── src/
│   ├── preprocessing.py
│   ├── train.py
│   └── predict.py
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 📷 Visualizations

### Feature Importance

![Feature Importance](results/feature_importance.png)

### SHAP Summary Plot

![SHAP Summary](results/shap_summary.png)

### Actual vs Predicted

![Prediction Plot](results/prediction_plot.png)

---

## 🎯 Key Contributions

- Developed groundwater prediction models using climatic and remote sensing variables.
- Created lag-based temporal features to capture groundwater memory effects.
- Applied explainable AI techniques for model interpretation.
- Evaluated and compared multiple machine learning approaches.

---

## 🔮 Future Improvements

- Physics-Informed Neural Networks (PINNs)
- LSTM-based Groundwater Forecasting
- Real-Time Monitoring Dashboard
- Satellite Data Expansion
- Digital Twin Groundwater System

---

## 👨‍💻 Author

Machine Learning project focused on sustainable groundwater resource management through data-driven modeling and explainable AI.
