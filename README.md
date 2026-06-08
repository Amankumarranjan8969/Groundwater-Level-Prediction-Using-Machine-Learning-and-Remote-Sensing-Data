# Groundwater-Level-Prediction-Using-Machine-Learning-and-Remote-Sensing-Data
Groundwater is one of the most important freshwater resources for agriculture, domestic consumption, and industrial activities. Accurate prediction of groundwater levels is essential for sustainable water resource management and drought mitigation.
Objectives
Predict monthly groundwater levels using machine learning techniques.
Analyze the influence of climatic and environmental factors on groundwater fluctuations.
Compare the performance of different machine learning models.
Identify the most important variables affecting groundwater levels.
Improve groundwater forecasting through temporal feature engineering.
Dataset Description

The dataset consists of monthly groundwater observations along with environmental and climatic variables.

Input Features
Feature	Description
Latitude	Location coordinate
ET_Mon	Monthly Evapotranspiration
RH_Mon	Monthly Relative Humidity
Wind_Mon	Monthly Wind Speed
NDVI_Mon	Normalized Difference Vegetation Index
NDMI_Mon	Normalized Difference Moisture Index
SM_100cm_Mon	Soil Moisture at 100 cm depth
GWL_lag_1	Groundwater Level of Previous Month
GWL_lag_2	Groundwater Level Two Months Earlier
Rain_lag_1	Rainfall of Previous Month
Rain_lag_2	Rainfall Two Months Earlier
Rain_roll3	Three-Month Rolling Average Rainfall
Temp_Avg	Average Monthly Temperature
Target Variable
GWL_Mon (Monthly Groundwater Level)
Feature Engineering

To improve prediction performance, temporal features were generated:

Groundwater Lag Features
GWL_lag_1
GWL_lag_2
Rainfall Lag Features
Rain_lag_1
Rain_lag_2
Rolling Statistics
Rain_roll3

These features help capture delayed groundwater responses to rainfall and seasonal hydrological processes.

Machine Learning Models
Random Forest Regressor

An ensemble learning method based on multiple decision trees that reduces overfitting and improves prediction stability.

XGBoost Regressor

A gradient boosting framework capable of capturing complex nonlinear relationships between environmental variables and groundwater levels.

Data Preprocessing

The following preprocessing steps were performed:

Missing value handling using median imputation.
Feature selection and cleaning.
Lag feature generation.
Rolling statistic generation.
Train-test splitting.
Model training and evaluation.
Evaluation Metrics

The following metrics were used:

R² Score
Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
Results
Random Forest
R² Score: 0.4067
MAE: 2.3655
MSE: 9.7597
RMSE: 3.1241
XGBoost
R² Score: 0.4134
Interpretation

Groundwater systems are highly nonlinear and influenced by numerous unobserved factors such as local pumping activities, geological heterogeneity, recharge variability, and human interventions. Despite these complexities, the models successfully captured a significant portion of groundwater variability.

Explainable AI (SHAP Analysis)

SHAP (SHapley Additive exPlanations) was used to understand feature importance and model behavior.

Benefits:

Improved model interpretability.
Identification of key groundwater drivers.
Enhanced trust and transparency in predictions.
Technologies Used
Python
Pandas
NumPy
Scikit-Learn
XGBoost
SHAP
Matplotlib
Seaborn
Jupyter Notebook
Project Workflow

Data Collection
↓
Data Cleaning
↓
Missing Value Treatment
↓
Feature Engineering
↓
Lag Feature Creation
↓
Model Training
↓
Model Evaluation
↓
SHAP Analysis
↓
Groundwater Prediction

Limitations
Small dataset size (289 samples).
Limited spatial coverage.
Absence of pumping and recharge records.
Groundwater behavior influenced by factors not included in the dataset.
Future Improvements
Integration of satellite-derived rainfall products.
Addition of geological and aquifer characteristics.
Incorporation of groundwater abstraction data.
Deep Learning based forecasting models.
Physics-Informed Neural Networks (PINNs).
Real-time groundwater monitoring dashboard.
Conclusion

This project demonstrates the feasibility of predicting groundwater levels using machine learning and remote sensing data. By combining climatic variables, vegetation indices, soil moisture information, and historical groundwater observations, the developed models provide useful insights into groundwater dynamics and support sustainable water resource management.
