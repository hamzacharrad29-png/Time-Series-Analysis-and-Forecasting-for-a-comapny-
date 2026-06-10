# 📈 Time Series Analysis and Forecasting for Euro-Cycles (ECYCL)

## 📌 Project Overview

This project analyzes and forecasts the closing stock price of **Euro-Cycles (ECYCL)**, a company listed on the **Tunis Stock Exchange**.

The objective is to study historical stock price behavior, evaluate time-series forecasting models, and generate future price predictions using statistical techniques.

---

## 🚀 Project Workflow

### 1. Data Collection
- Scraped historical stock price data from **ilboursa.com** using **Selenium**.

### 2. Exploratory Data Analysis (EDA)
- Price trend visualization
- Seasonal decomposition
- Stationarity testing (ADF test)
- ACF and PACF analysis

### 3. Time Series Modeling
Two forecasting models were developed and compared:

- **ARIMA(1,1,0)**
- **SARIMA(5,1,0)(5,1,0)**

### 4. Model Evaluation
Models were evaluated using:

- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- MAPE (Mean Absolute Percentage Error)

### 5. Forecasting
- Generated a **50-business-day forecast** using the best-performing model.

---

## 📊 Model Performance

| Model | RMSE | MAE | MAPE |
|--------|--------|--------|--------|
| **ARIMA(1,1,0)** | **0.2849** | **0.1690** | **1.11%** |
| SARIMA(5,1,0)(5,1,0) | 0.3077 | 0.1967 | 1.30% |

###  Best Model

The **ARIMA(1,1,0)** model achieved the best performance with a **MAPE of only 1.11%**, making it the selected model for forecasting.

---

##  Visualizations

### Stock Price Evolution and Seasonal Decomposition

![Price Evolution and Decomposition]([images/price_evolution_and_decomposition.png](https://github.com/hamzacharrad29-png/Time-Series-Analysis-and-Forecasting-for-a-comapny-/blob/578a26c528d9a9df1240eaf316f7c5b175064d7f/price%20evolution%20and%20decomposition%20.png))

### ACF and PACF Analysis

![ACF PACF]([[images/acf_pacf.png](https://github.com/hamzacharrad29-png/Time-Series-Analysis-and-Forecasting-for-a-comapny-/blob/7bb67ae72cf56ae73f5e7f9c2cd0a6063bc51ab3/ACF%20PACF%20ARIMA%20.png)

### ARIMA Forecast vs Actual Values

![ARIMA Prediction]([images/arima_prediction.png](https://github.com/hamzacharrad29-png/Time-Series-Analysis-and-Forecasting-for-a-comapny-/blob/7bb67ae72cf56ae73f5e7f9c2cd0a6063bc51ab3/Arima%20prediction%20.png))

### 50-Day Forecast

![50-Day Forecast]([images/forecast_50_days.png](https://github.com/hamzacharrad29-png/Time-Series-Analysis-and-Forecasting-for-a-comapny-/blob/7bb67ae72cf56ae73f5e7f9c2cd0a6063bc51ab3/Prediction%20de%2050%20jours%20.png))



## 🛠️ Technologies and Libraries

- **Python**
- **Pandas** & **NumPy** – Data manipulation and numerical computations
- **Matplotlib** & **Seaborn** – Data visualization
- **Statsmodels** – ARIMA and SARIMA modeling
- **Scikit-learn** – Model evaluation metrics
- **Selenium** – Web scraping
- **pmdarima** – Automatic ARIMA model selection and optimization
