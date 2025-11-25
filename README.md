# NeuralProphet + Optuna Time Series Forecasting Project

This repository contains a full project implementing NeuralProphet with Optuna hyperparameter optimization on a synthetic daily time series (>= 3 years).

**Local path to uploaded screenshots (provided in conversation):**
- /mnt/data/Screenshot 2025-11-21 123040.png
- /mnt/data/Screenshot 2025-11-21 122957.png
- /mnt/data/Screenshot 2025-11-21 123022.png

## Contents
- `neuralprophet_optuna_project.py` - Main production-ready script.
- `requirements.txt` - Python packages required.
- `REPORT.md` - Project report and analysis.
- `top5_hyperparams.csv` - (generated after running) top-5 hyperparameter results.
- `best_model_forecast.png` - (generated after running) forecast plot.
- `screenshots/` - Copies of the uploaded screenshots.

## How to run
1. Create and activate a virtual environment.
2. Install requirements:
   ```
   pip install -r requirements.txt
   ```
   If NeuralProphet complains about PyTorch, install a compatible torch build for your platform:
   ```
   pip install torch
   ```
3. Run:
   ```
   python neuralprophet_optuna_project.py
   ```

The script will:
- Generate a synthetic dataset (2017-01-01 to 2021-12-31).
- Run baseline evaluation and Optuna optimization (default 30 trials).
- Save `top5_hyperparams.csv` and `best_model_forecast.png` in the working directory.

