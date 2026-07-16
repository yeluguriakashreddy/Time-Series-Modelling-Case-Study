# German Electricity Demand Forecasting using Statistical, Machine Learning and Deep Learning Models

## Project Overview

This project develops and compares multiple forecasting techniques for predicting German electricity demand using publicly available electricity consumption data. The study evaluates classical statistical forecasting models, machine learning algorithms, and deep learning approaches to identify the most suitable forecasting model for operational electricity demand prediction.

The project follows a complete machine learning workflow including data preprocessing, exploratory data analysis, feature engineering, statistical modelling, machine learning, deep learning, model evaluation, and forecasting.

---

## Objectives

- Download and preprocess German electricity demand data.
- Perform exploratory data analysis (EDA).
- Test stationarity using statistical tests.
- Build benchmark forecasting models.
- Develop SARIMA and SARIMAX forecasting models.
- Incorporate temperature as an exogenous variable.
- Build feature-based machine learning models.
- Develop an LSTM neural network for forecasting.
- Compare forecasting accuracy using multiple evaluation metrics.
- Recommend the best model for operational forecasting.

---

## Dataset

### Electricity Demand Dataset

Source:
https://data.open-power-system-data.org/time_series/

Dataset Used:

time_series_60min_singleindex.csv

Country:

Germany (DE)

Time Period:

January 2015 – October 2020

Frequency:

Hourly

After preprocessing:

- Hourly data
- Daily aggregated data
- Weekly aggregated data

---

## Technologies Used

- Python 3
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels
- Scikit-learn
- TensorFlow / Keras
- Open-Meteo API

---

## Project Structure

```
German-Electricity-Forecasting/
│
├── data/
│   ├── time_series_60min_singleindex.csv
│   └── berlin_temperature.csv
│
├── notebooks/
│   └── Electricity_Demand_Forecasting.ipynb
│
├── figures/
│   ├── hourly_plot.png
│   ├── daily_plot.png
│   ├── weekly_plot.png
│   ├── benchmark_models.png
│   ├── sarima_forecast.png
│   ├── sarimax_forecast.png
│   ├── random_forest_forecast.png
│   ├── gradient_boosting_forecast.png
│   ├── lstm_forecast.png
│   └── model_comparison.png
│
├── results/
│   ├── benchmark_model_results.csv
│   ├── sarima_metrics.csv
│   ├── sarimax_metrics.csv
│   ├── random_forest_metrics.csv
│   ├── gradient_boosting_metrics.csv
│   ├── lstm_metrics.csv
│   └── Final_Model_Comparison.csv
│
├── report/
│   └── Electricity_Demand_Forecasting_Report.pdf
│
├── README.md
└── requirements.txt
```

---

## Project Workflow

### Part 1

Data Collection and Preprocessing

- Load hourly electricity demand data
- Data cleaning
- Missing value removal
- Convert timestamps
- Aggregate to daily and weekly frequency

---

### Part 2

Exploratory Data Analysis

- Hourly demand visualization
- Daily demand visualization
- Weekly demand visualization
- Histogram
- Boxplot
- Seasonal decomposition
- Rolling statistics
- ADF Test
- KPSS Test
- Autocorrelation analysis

---

### Part 3

Benchmark Forecast Models

- Mean Forecast
- Naïve Forecast
- Seasonal Naïve Forecast
- Drift Forecast

---

### Part 4

SARIMA Model

- Grid Search using AIC
- Residual diagnostics
- Forecast generation
- Confidence intervals

---

### Part 5

SARIMAX Model

Additional explanatory variables:

- Weekly Mean Temperature
- Heating Degree Days (HDD)
- Cooling Degree Days (CDD)

---

### Part 6

Machine Learning Models

- Random Forest Regressor
- Gradient Boosting Regressor

---

### Part 7

Deep Learning Model

Long Short-Term Memory (LSTM)

Workflow:

- Data normalization
- Sequence generation
- Model training
- Hyperparameter tuning
- Forecast generation

---

## Evaluation Metrics

The models are evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Percentage Error (MAPE)
- Coefficient of Determination (R²)

---

## Models Implemented

- Mean Forecast
- Naïve Forecast
- Seasonal Naïve Forecast
- Drift Forecast
- SARIMA
- SARIMAX
- Random Forest
- Gradient Boosting
- LSTM Neural Network

---

## Results Summary

The forecasting models were compared using MAE, RMSE, MAPE, and R².

Among all evaluated models, the Gradient Boosting model achieved the best overall forecasting performance by producing the lowest prediction errors and the highest coefficient of determination. Random Forest also demonstrated strong predictive capability, while the SARIMA model outperformed the benchmark statistical models. The SARIMAX model incorporated temperature information but did not consistently improve forecasting accuracy for this implementation. The LSTM model successfully learned temporal patterns but required considerably more computational resources and model tuning.

---

## How to Run

### Clone Repository

```bash
git clone https://github.com/yeluguriakashreddy/Time-Series-Modelling-Case-Study.git
```

### Install Packages

```bash
pip install -r requirements.txt
```

### Open Notebook

```
Google Colab

or

Jupyter Notebook
```

### Run All Cells

Execute the notebook sequentially.

---

## Output

The project generates:

- Exploratory plots
- Forecast plots
- Residual analysis
- Feature importance plots
- LSTM predictions
- Model comparison charts
- Performance metrics
- Final report

---

## Future Improvements

Possible future enhancements include:

- Transformer-based forecasting models
- Temporal Fusion Transformer (TFT)
- XGBoost
- LightGBM
- Prophet
- Additional weather variables
- Holiday effects
- Renewable energy generation
- Bayesian hyperparameter optimization

---
