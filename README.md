# ⚡ US Electricity Generation Forecasting & Energy Transition Analysis

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Statsmodels](https://img.shields.io/badge/SARIMA-Econometrics-orange)
![XGBoost](https://img.shields.io/badge/XGBoost-Machine%20Learning-red)
![Prophet](https://img.shields.io/badge/Prophet-Forecasting-purple)

---

# Project Overview

This project analyzes the evolution of the U.S. electricity generation sector using the **EIA-923 Monthly Generation and Fuel Consumption database** from **2015 to 2024**.

The project combines:

- Data Engineering
- Exploratory Data Analysis
- Econometrics
- Time-Series Forecasting
- Machine Learning
- Energy Economics

The objectives are:

- Analyze the U.S. energy transition
- Study structural changes in electricity generation
- Forecast electricity generation
- Compare forecasting methodologies
- Evaluate forecasting performance

---

# Dataset

### Source

- U.S. Energy Information Administration (EIA)
- EIA-923 Monthly Generation and Fuel Consumption Data

### Period

January 2015 – December 2024

### Frequency

Monthly

### Observations

- 1.67 million observations after transformation
- 120 monthly observations for forecasting analysis

---

# Methodology

## Data Engineering

- Data extraction
- Cleaning and transformation
- Monthly aggregation
- Feature engineering

## Statistical Analysis

- Descriptive statistics
- Market share analysis
- Concentration analysis (HHI)
- Compound annual growth rates (CAGR)

## Econometric Analysis

- Augmented Dickey-Fuller tests
- Seasonal differencing
- ACF/PACF analysis
- Structural break analysis

## Forecasting Models

- SARIMA
- Prophet
- XGBoost

---

# Forecasting Results

| Model | MAE | RMSE | NRMSE |
|---|---:|---:|---:|
| XGBoost | 4.81M | 6.21M | **3.98%** |
| SARIMA | 4.79M | 6.28M | 4.03% |
| Prophet | 7.24M | 8.39M | 5.38% |

### Key Finding

Machine learning (XGBoost) slightly outperformed classical econometric methods, while SARIMA remained highly competitive.

---

# Energy Transition Results

| Fuel | CAGR |
|---|---:|
| Solar | +27.5% |
| Wind | +10.1% |
| Natural Gas | +3.9% |
| Nuclear | -0.2% |
| Hydro | -0.3% |
| Coal | -7.8% |

---

# Structural Break Analysis

A two-sample statistical test identified a significant structural change after 2020:

| Statistic | Value |
|---|---:|
| t-statistic | -5.72 |
| p-value | 8.68e-08 |

This indicates a statistically significant change in the U.S. electricity generation regime.

---



# Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Statsmodels
- Prophet
- XGBoost
- SciPy

---

# Repository Structure

```text
EIA923-Energy-Forecasting/

├── data/
├── notebooks/
├── figures/
├── results/
├── README.md
└── requirements.txt
```

---

# Key Findings

- Natural gas became the dominant electricity source.
- Coal experienced a structural decline.
- Solar generation exhibited exponential growth.
- The U.S. electricity portfolio remained moderately concentrated.
- Structural changes occurred after 2020.
- XGBoost achieved the highest forecasting accuracy.

---

# Author

Panagiotis Karampoulis
