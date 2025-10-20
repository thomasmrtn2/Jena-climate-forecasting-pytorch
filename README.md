# Jena Climate Forecasting (PyTorch)

Forecasting next-day (24h) temperature using the Jena Climate dataset (hourly resolution).  
This repo contains a clean, notebook-first workflow with:
- chronological split (train/val/test),
- standardized features (train-only stats),
- LSTM forecaster with temporal pooling,
- persistence baseline for comparison,
- portfolio-ready plots and metrics.

## Results (Test)
- Baseline (persistence): MAE 2.369 °C, RMSE 3.080 °C  
- Model (LSTM): MAE 1.772 °C, RMSE 2.300 °C  
**Improvement:** ~25% MAE and ~25% RMSE vs baseline.

## Repo Structure
.
├── notebook/
│   └── Jenna_Climate.ipynb
├── src/                # optional Python modules
├── figures/            # exported plots
├── data/               # (ignored) put raw data here
├── requirements.txt
├── .gitignore
└── README.md

## How to run
1. Create a Python env and install deps:
   ```bash
   pip install -r requirements.txt

2. Download the Jena Climate dataset (CSV) into data/.

3. Open Jenna_Climate.ipynb and run all cells.
