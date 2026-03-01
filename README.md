📌 Delhi PM2.5 Pollution Forecasting Using SARIMA

📖 Project Overview

This project builds a time-series forecasting model to predict future PM2.5 pollution levels in Delhi using historical air quality data. The objective is to analyze seasonal pollution patterns and develop a statistically robust forecasting model.

The analysis includes data preprocessing, stationarity testing, seasonal decomposition, baseline benchmarking, SARIMA modeling, and forecast evaluation.

📊 Dataset

Historical daily pollution data for Delhi

Variables include: PM2.5, PM10, NO2, SO2, CO, Ozone, AQI

Data aggregated to monthly frequency for stable seasonal modeling

🛠️ Methodology

1️⃣ Data Preprocessing

Created datetime index from Year, Month, Date columns

Sorted and validated time continuity

Aggregated daily PM2.5 into monthly averages


2️⃣ Exploratory Time Series Analysis

Seasonal Decomposition (Trend + Seasonality + Residuals)

Augmented Dickey-Fuller (ADF) Test for stationarity

Rolling mean visualization


3️⃣ Baseline Models

Naive forecast (last value persistence)

Seasonal naive forecast (same month previous year)


4️⃣ Model Development

ARIMA modeling

Seasonal ARIMA (SARIMA)

Final selected model:

SARIMA(1,0,0)(0,1,0,12)

5️⃣ Model Evaluation

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

Residual diagnostics

📈 Results

SARIMA outperformed baseline and simple ARIMA models

Successfully captured yearly pollution seasonality

Generated 6-month forward forecast

Included confidence intervals to quantify uncertainty

🔮 Future Forecast

The model predicts PM2.5 levels for the next six months, reflecting seasonal variation and historical trend behavior.

📷 Visualizations

Time series decomposition

Train-test split

Forecast vs Actual comparison

Forecast with confidence intervals

(See /images folder)

🧠 Key Learnings

Importance of stationarity testing before differencing

Avoiding over-parameterization in small datasets

Proper benchmarking using baseline models

Seasonal modeling considerations with limited cycles

Practical implementation of SARIMA

🛠️ Tools & Libraries

Python

Pandas

NumPy

Matplotlib

Statsmodels

Scikit-learn
