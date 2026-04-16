# Egypt Inflation Forecasting using ARIMA, XGBoost, and Hybrid Modeling

## Project Overview
This repository contains a graduation project focused on forecasting Egypt’s inflation using three modeling approaches:
- ARIMA (time-series baseline)
- XGBoost (machine-learning model)
- Hybrid ARIMA + XGBoost (residual learning)

## Dataset Description
The project combines monthly macroeconomic indicators (1995–2024), including:
- Consumer Price Index (CPI)
- USD/EGP exchange rate
- M2 money supply
- Interest rate

Raw datasets are standardized and merged into a processed inflation dataset used for modeling.

## Repository Structure
```text
.
├── README.md
├── requirements.txt
├── .gitignore
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
└── results/
    ├── arima_xgb_results.csv
    └── model_comparison_metrics.csv
```

## Main Notebook Location
- `notebooks/main_analysis.ipynb`

## Outputs
- `results/arima_xgb_results.csv`
- `results/model_comparison_metrics.csv`

## Methods Used
- ARIMA
- XGBoost
- Hybrid model (ARIMA + XGBoost residual correction)

## Evaluation Metrics
- RMSE
- MAE
- R²
- MAPE

## Requirements / Installation
```bash
python -m venv .venv
source .venv/bin/activate  # Windows CMD: .venv\Scripts\activate | PowerShell: .venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

## Notes
- Notebook paths use repository-relative locations.
- Raw inputs are loaded with basic column-name cleaning for robustness.
- Old experimental notebooks and legacy source files are kept under `archive_local_only/` and excluded via `.gitignore`.

## Author
Graduation project repository for inflation forecasting in Egypt.
