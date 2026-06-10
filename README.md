##  Project Description
# Time-Series-Analysis-and-Forecasting-for-a-comapny-
This project aims to analyze and forecast the closing price time series of a company  **Eurocycles (ECYCL)** stock, listed on the Tunis Stock Exchange.


### Key Steps:

1. **Data Collection** – Web scraping with Selenium from `ilboursa.com`
2. **Exploratory Analysis** – Visualization, seasonal decomposition, stationarity tests
3. **Modeling** – ARIMA(1,1,0) and SARIMA(5,1,0,5)
4. **Evaluation** – Model comparison (RMSE, MAE, MAPE)
5. **Forecasting** – 50 business day projection

## 📊 Key Results

| Model                        | RMSE    | MAE     | MAPE   |
|------------------------------|---------|---------|--------|
| **ARIMA(1,1,0)**             | 0.2849  | 0.1690  | 1.11%  |
| SARIMA(5,1,0,5)              | 0.3077  | 0.1967  | 1.30%  |

👉 The **ARIMA(1,1,0)** model is selected as the best, with a mean absolute percentage error of only **1.11%**.

## 📈 Key Visualizations

| Price Evolution | Decomposition |
|-----------------|---------------|
| ![](images/evolution_cours.png) | ![](images/decomposition.png) |

| ACF/PACF | ARIMA Prediction |
|----------|------------------|
| ![](images/acf_pacf.png) | ![](images/prediction_arima.png) |

| Model Comparison | 50-Day Forecast |
|------------------|-----------------|
| ![](images/comparaison_modeles.png) | ![](images/forecast_50.png) |

## 🛠️ Technologies Used

- **Python**
- **Pandas, NumPy** – Data manipulation and calculations
- **Matplotlib, Seaborn** – Visualization
- **Statsmodels** – ARIMA/SARIMA modeling
- **Scikit-learn** – Evaluation metrics
- **Selenium** – Web scraping
- **PMDARIMA** – Automatic model optimization
