# bike-rental-forecast-project
Time series analysis and forecasting of daily bike rental demand in Washington, D.C.
# 🚴‍♂️ Bike Rental Demand Forecasting using Time Series Models

This project involves a comprehensive time series analysis and forecasting of daily bike rental demand using the `bike_sharing_daily` dataset from the `timetk` package in R. The dataset includes daily bike rentals in Washington, D.C. along with corresponding weather and seasonal variables.

## 📌 Project Overview

The goal of this project is to:

- Explore and visualize the time series characteristics of the dataset.
- Clean and smooth the data to reveal underlying patterns.
- Decompose and test the stationarity of the time series.
- Fit ARIMA models (manual and auto) to generate forecasts.
- Evaluate model performance and forecast daily rental demand.

## 🛠️ Tools and Technologies

- **R**
- **RStudio**
- `timetk`, `forecast`, `lubridate`, `ggplot2`, `TTR`, `tseries`, and other supporting libraries

## 📈 Project Steps

### 1. Data Loading & Exploration
- Loaded the built-in `bike_sharing_daily` dataset using the `timetk` package.
- Explored seasonality, trend, weather correlations, and summary statistics.

### 2. Interactive Visualization
- Used `plot_time_series()` for interactive time plots.
- Visualized seasonality and anomalies using `plot_seasonal_diagnostics()` and `plot_anomaly_diagnostics()`.

### 3. Data Cleaning & Smoothing
- Cleaned the data using `tsclean()` to remove outliers and fill missing values.
- Applied Simple Moving Average (SMA) and Exponential Smoothing for short-term forecasts.

### 4. Time Series Decomposition & Stationarity
- Decomposed the series using STL to isolate seasonal and trend components.
- Tested for stationarity using ADF test and differencing techniques.

### 5. ARIMA Modeling & Forecasting
- Built both manual and automatic ARIMA models.
- Compared models using AIC/BIC and residual diagnostics.
- Forecasted the next 25 days of bike rental demand with confidence intervals.

## 💡 Key Findings

- Strong seasonal trends: Rentals peak in summer and drop in winter.
- Temperature and “feeling temperature” show a strong positive correlation with rentals.
- Auto ARIMA selected an optimal model with well-behaved residuals and minimal AIC.
- Forecasts indicate continued seasonality and gradual growth trends in demand.

## 📁 Files in this Repository

- `Forecast-daily-bike-rental-demand-using-time-series-models.Rmd` — R Markdown script containing all code and analysis.
- `Forecast-daily-bike-rental-demand-using-time-series-models.html` — Knitted HTML report with results and visualizations.


## 📍 How to Run

1. Clone this repository or download the files.
2. Open the `.Rmd` file in **RStudio**.
3. Install required packages (`timetk`, `forecast`, `lubridate`, etc.).
4. Knit to HTML to view the full analysis.

## 👤 Author

vikashini balasubramanian

## 📄 License

This project is open-source and available under the MIT License.
