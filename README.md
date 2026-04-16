# Egypt Inflation Forecasting using ARIMA, XGBoost, and Hybrid Modeling

This project analyzes and forecasts Egyptian inflation using monthly macroeconomic data from 1995 to 2024.

## Project overview

The workflow includes:

- Data collection and preprocessing
- Merging CPI, exchange rate, interest rate, and M2 money supply data
- Feature engineering
- Inflation rate calculation
- ARIMA modeling
- XGBoost modeling
- Hybrid ARIMA + XGBoost modeling
- Model comparison using evaluation metrics

## Dataset

The project uses monthly data for:

- Consumer Price Index (CPI)
- USD/EGP exchange rate
- Interest rate
- M2 money supply

Processed features also include dummy variables for major economic events such as:

- 2016 currency float
- COVID period
- Ukraine war period

## Repository structure

```text
.
├── notebooks/
│   └── main_analysis.ipynb
├── data/
│   ├── raw/
│   │   ├── cpi.csv
│   │   ├── exchange_rate.csv
│   │   ├── m2.csv
│   │   └── interest_rate.csv
│   └── processed/
│       └── combined_inflation_dataset.csv
├── results/
│   ├── arima_xgb_results.csv
│   └── model_comparison_metrics.csv
├── requirements.txt
├── .gitignore
└── README.md
