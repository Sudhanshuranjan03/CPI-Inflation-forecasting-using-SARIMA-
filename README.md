# Forecasting Inflation Rate of India using SARIMA


**Overview**

This project aims to forecast the inflation rate in India from January 2014 to January 2024 using time series analysis. The focus is on applying the Box-Jenkins (BJ) methodology to develop univariate models for accurate inflation forecasting, which can help policymakers and financial institutions make better decisions.

**Objective**

The primary objective of this study is to:

Analyze trends, seasonality, and autocorrelation in India’s inflation data.
Develop and compare time series models, such as ARIMA and SARIMA, to identify the best model for forecasting.
Generate out-of-sample forecasts for the inflation rate from February 2024 to August 2024.

**Data**

Data Source: Monthly inflation rates in India from January 2014 to January 2024.
Observations: 121 monthly observations.
Time Frame: 10 years (2014-2024).

**Methodology**

This project employs the Box-Jenkins (BJ) methodology for time series analysis and forecasting:

**Exploratory Data Analysis (EDA):
**
Time series plots, Autocorrelation Function (ACF), and Partial Autocorrelation Function (PACF) plots were used to identify trends and seasonal patterns.
Decomposition analysis helped understand the underlying components of the series, such as trend, seasonality, and residuals.
Stationarity Tests:

Augmented Dickey-Fuller (ADF) Test
Phillips-Perron (PP) Test
KPSS Test
These tests indicated that the original series was non-stationary, requiring differencing to achieve stationarity.

**Model Identification:**

Two models were developed: ARIMA(2,1,0) and SARIMA(2,1,0)(0,0,1)[12].
The SARIMA model included a seasonal component with annual seasonality, which aligned with the observed seasonal patterns in the data.
Model Evaluation:

Models were evaluated using Root Mean Square Error (RMSE) and Mean Absolute Percentage Error (MAPE).
SARIMA(2,1,0)(0,0,1)[12] outperformed ARIMA(2,1,0) with a lower RMSE (0.835) and MAPE (12.89%), making it the preferred model for forecasting.

**Forecasting:**

Out-of-sample forecasts were generated for the period from February 2024 to August 2024.
The forecast predicts a gradual increase in inflation, peaking in May 2024, followed by a decline.

**Results**

Best-Fit Model: SARIMA(2,1,0)(0,0,1)[12].
Performance:
RMSE: 0.835 for the SARIMA model.
MAPE: 12.89% for the SARIMA model.

**Forecast Highlights:**

Predicted inflation rate peak of approximately 6.18% in May 2024.
Gradual decline to a low of around 4.05% in July 2024.

Repository Structure

notebooks/: Jupyter notebooks with detailed analysis and model outputs.
results/: Forecasts and model performance metrics.
README.md: Overview and detailed information about the project.
