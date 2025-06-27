# Predictive Maintenance of Ball Bearings using Machine Learning

This project implements a machine learning-based predictive maintenance system for ball bearings. Using sensor data from the IEEE PHM 2012 Data Challenge, the model predicts the Remaining Useful Life (RUL) of bearings to enable timely maintenance and prevent equipment failure.

---

## Project Objective

- Analyze vibration data from sensors monitoring ball bearings.
- Extract statistical and frequency-domain features.
- Train regression models to predict Remaining Useful Life (RUL).
- Evaluate model performance using RMSE and MAE.

---

## Dataset

The dataset is sourced from:

📂 **[IEEE PHM 2012 Data Challenge Dataset](https://github.com/wkzs111/phm-ieee-2012-data-challenge-dataset)**

It includes vibration signal data from bearings under test until failure, recorded with high-frequency sensors.

---

## Technologies & Libraries

- **Python 3.x**
- **NumPy** – for array processing
- **Pandas** – for data handling
- **Matplotlib & Seaborn** – for visualization
- **SciPy** – for FFT and signal processing
- **scikit-learn** – for ML models and metrics
- **joblib** – for model saving/loading
- **os / glob** – for file operations

---

## Workflow Overview

1. **Data Loading**  
   Load raw `.mat` or `.csv` vibration data.

2. **Feature Extraction**  
   Extract time-domain and frequency-domain features:
   - RMS, Kurtosis, Skewness, Crest Factor, etc.
   - FFT-based frequency power

3. **Data Labeling**  
   Label data with actual Remaining Useful Life (RUL) based on failure timeline.

4. **Model Training**  
   Use regression models (e.g., Linear Regression, SVR, Random Forest) to predict RUL.

5. **Model Evaluation**  
   Evaluate using RMSE, MAE, and visualization of predictions vs. ground truth.

6. **Prediction & Deployment**  
   Predict RUL on new sensor data for maintenance scheduling.

---
