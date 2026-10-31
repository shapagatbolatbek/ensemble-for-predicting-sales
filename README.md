# Adaptive Ensemble for Daily Sales and Revenue Forecasting (M5)

Code and results for the paper *Development of a Time-Series Forecasting Model for Predicting Sales and Revenue Using Machine Learning Methods* (Shapagat Bolatbek, Symbat Salim, Astana IT University).

The notebook compares seven forecasting models (SNaive, ETS, SARIMAX, Prophet, LightGBM, LSTM, CNN-LSTM) and three ways of combining them (equal weights, per-series selection and an adaptive ensemble) on 70 store–department series from the M5 Walmart dataset, for daily unit sales and revenue.

## Files

| File | Contents |
|---|---|
| `sales_revenue_ensemble_M5.ipynb` | Full experiment, executed in Google Colab, with all outputs |
| `outputs/results_tables.xlsx` | Accuracy tables (overall, per window, DM tests, categories, states, weights, event days) |
| `outputs/latex_results.tex` | Table rows and plot coordinates used in the paper |
| `outputs/*.png` | Figures produced by the notebook |
| `requirements.txt` | Python packages |

## How to run

Open the notebook in Google Colab, select a GPU runtime and choose *Runtime → Run all*. The notebook downloads the M5 data itself (the data are not stored in this repository), saves intermediate results to Google Drive so an interrupted run can resume, and writes all tables and figures to `outputs/`.

## Data

M5 Forecasting – Accuracy competition data (Walmart), https://www.kaggle.com/competitions/m5-forecasting-accuracy. The notebook downloads identical copies of the files from a public mirror.
