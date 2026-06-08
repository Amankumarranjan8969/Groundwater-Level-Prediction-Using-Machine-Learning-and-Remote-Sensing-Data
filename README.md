# 🌍 Groundwater Level Prediction using Machine Learning

> Predicting monthly groundwater levels using hydro-meteorological variables, remote sensing indices, and temporal feature engineering.

---

## 🚀 Project Overview

Groundwater is a critical freshwater resource for agriculture, industry, and domestic use. Accurate groundwater forecasting helps in sustainable water resource management and drought preparedness.

This project uses Machine Learning techniques along with Remote Sensing and Climate Data to predict monthly groundwater levels.

---

## 📊 Features Used

### Climate Variables
- Evapotranspiration (ET)
- Relative Humidity (RH)
- Wind Speed
- Average Temperature

### Remote Sensing Variables
- NDVI (Normalized Difference Vegetation Index)
- NDMI (Normalized Difference Moisture Index)

### Soil Variables
- Soil Moisture (100 cm depth)

### Temporal Features
- GWL_lag_1
- GWL_lag_2
- Rain_lag_1
- Rain_lag_2
- Rain_roll3

### Spatial Feature
- Latitude

### Target Variable
- GWL_Mon (Groundwater Level)

---

## 🔄 Project Workflow

```text
Data Collection
      ↓
Data Cleaning
      ↓
Missing Value Handling
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

## 🤖 Machine Learning Models

### Random Forest Regressor

- Ensemble-based learning algorithm
- Handles non-linear relationships effectively
- Provides feature importance scores

### XGBoost Regressor

- Gradient boosting framework
- High predictive performance
- Efficient handling of tabular datasets

---

## 📈 Model Performance

| Model | R² Score |
|---------|---------|
| Random Forest | 0.4067 |
| XGBoost | 0.4134 |

### Random Forest Metrics

| Metric | Value |
|---------|---------|
| MAE | 2.365 |
| MSE | 9.760 |
| RMSE | 3.124 |

---

## 🧠 Explainable AI

SHAP (SHapley Additive Explanations) was used to:

- Understand model predictions
- Identify influential features
- Improve model transparency
- Interpret groundwater drivers

---

## 🛠️ Technology Stack

```python
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
│   └── water2222222.ipynb
│
├── results/
│   ├── correlation_heatmap.png
│   ├── feature_importance.png
│   ├── shap_summary.png
│   └── actual_vs_predicted.png
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 📷 Results

### Correlation Analysis

![Correlation Heatmap](results/correlation_heatmap.png)

### Feature Importance

![Feature Importance](results/feature_importance.png)

### SHAP Summary Plot

![SHAP Summary](results/shap_summary.png)

### Actual vs Predicted Groundwater Levels

![Prediction Plot](results/actual_vs_predicted.png)

---

## ✨ Key Contributions

- Integrated Remote Sensing and Climate Variables
- Developed Lag-Based Temporal Features
- Compared Multiple Machine Learning Models
- Applied Explainable AI for Model Interpretation
- Built an End-to-End Groundwater Prediction Pipeline

---

## 🔮 Future Scope

- Physics-Informed Neural Networks (PINNs)
- LSTM-Based Time Series Forecasting
- Real-Time Groundwater Monitoring Dashboard
- Digital Twin for Groundwater Systems
- Integration of Additional Satellite Datasets

---

## 👨‍💻 Author

Ak R

B.Tech Computer Science Engineering

Machine Learning | Remote Sensing | Groundwater Analytics
