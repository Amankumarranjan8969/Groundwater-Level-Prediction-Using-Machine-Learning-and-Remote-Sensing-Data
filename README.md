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


### CatBoost Regressor

- Gradient boosting framework optimized for tabular data
- Captures complex nonlinear relationships effectively
- Robust performance on small datasets
- Reduces overfitting using ordered boosting
- Handles missing values efficiently
- Achieved the highest predictive accuracy in this study

## 📊 Model Performance

The performance of multiple ensemble machine learning models was evaluated for groundwater level prediction. Among all tested models, **CatBoost Regressor achieved the best predictive performance**, demonstrating its ability to capture complex nonlinear relationships within hydro-meteorological and remote sensing datasets.

| Model | R² Score | MAE | MSE | RMSE |
|---------|---------|---------|---------|---------|
| Random Forest | 0.6847 | 1.8414 | 5.1869 | 2.2775 |
| XGBoost | 0.6631 | 1.7954 | 5.5420 | 2.3541 |
| CatBoost | **0.8008** | **1.4531** | **3.2762** | **1.8100** |

### 🏆 Best Performing Model

**CatBoost Regressor**

- Highest R² Score: **0.8008**
- Lowest MAE: **1.4531**
- Lowest MSE: **3.2762**
- Lowest RMSE: **1.8100**

### 📈 Performance Summary

```text
CatBoost      ████████████████████ 0.8008
Random Forest █████████████████    0.6847
XGBoost       ████████████████     0.6631
```

### 🔍 Interpretation

- CatBoost achieved the highest predictive accuracy among all evaluated models.
- The model effectively captured nonlinear relationships between groundwater levels and environmental variables.
- Temporal lag features significantly improved forecasting performance by incorporating historical groundwater behavior.
- The results demonstrate the potential of combining machine learning, remote sensing, and hydro-meteorological data for groundwater forecasting and digital twin development.

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

Aman kumar ranjan

B.Tech Computer Science Engineering (Data science)

Machine Learning | Remote Sensing | Groundwater Analytics
