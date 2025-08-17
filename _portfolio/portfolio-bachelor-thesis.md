---
title: "Power Consumption Forecasting for Industrial Systems"
excerpt: "Time series modeling of industrial power consumption using ARIMA, LSTM, and XGBoost.<br/><img src='/images/portfolio/bachelor_thesis.png'>"
collection: portfolio
date: 2024-07-31
---

## Overview
In my Bachelor's thesis at HTWG Konstanz, I developed and compared machine learning models for forecasting **industrial power consumption**. The work involved preprocessing production-related time series data, training multiple models, and evaluating them using standard error metrics.

The project was conducted using real-world production data provided by the industrial company [Fondium](https://fondium.eu/) in Singen, Germany, and focused on improving prediction accuracy for **energy management**.

## Methods & Tools
- **Data Processing:** Python (Pandas, NumPy, Scikit-learn, statsmodels)
- **Models:** ARIMA, LSTM (PyTorch), XGBoost
- **Evaluation Metrics:** MAE, RMSE, R²
- **Visualization:** Matplotlib, Seaborn
- **Environment:** PyCharm, Anaconda

## Results
- **XGBoost** and **LSTM** achieved the highest prediction accuracy (R² ≈ 0.95), with **XGBoost** being significantly faster in training.  
- An application scenario demonstrated potential weekly cost savings of around €309 through optimized production scheduling based on model forecasts.

### Model performance comparison on validation (10 splits) and test datasets:

| **Model**  | **MAE** (Val.) | **RMSE** (Val.) | **R²** (Val.) | **MAE** (Test) | **RMSE** (Test) | **R²** (Test) | **Training Time** |
|------------|----------------|-----------------|---------------|----------------|-----------------|---------------|-------------------|
| ARIMA      | 33.442         | 42.625          | 0.698         | 32.932         | 41.144          | 0.741         | 69.679 s          |
| LSTM       | 18.073         | 23.424          | 0.915         | **12.481**     | **16.353**      | **0.959**     | 35.371 s          |
| XGBoost    | **16.801**     | **21.657**      | **0.927**     | 13.436         | 18.032          | 0.950         | **0.520 s**       |

These results demonstrate that XGBoost offers an optimal balance between prediction performance and computational efficiency.

**Notes:** Due to confidentiality, the full thesis document is not publicly available.
