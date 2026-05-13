# Probabilistic Solar PV Power Forecasting with Machine Learning and Calibrated Prediction Intervals

This repository contains the implementation for my MS Thesis-I work on one-hour-ahead probabilistic solar PV power forecasting using the DKASC Site 13 dataset.

## Overview

The project develops a reproducible machine-learning pipeline for solar PV forecasting. The workflow includes data cleaning, hourly resampling, daylight filtering, timestamp-safe lag feature engineering, chronological train/validation/calibration/test splitting, XGBoost point forecasting, XGBoost quantile regression, non-crossing correction, and conformal calibration.

## Dataset

The dataset is obtained from the Desert Knowledge Australia Solar Centre (DKASC), Site 13 / DKA-M6-B-Phase. Raw data files are not included in this repository due to file size considerations. Please refer to the DKASC website to download the original data.

## Repository Structure

- `notebooks/`: Jupyter notebooks for EDA, preprocessing, feature engineering, modeling, and calibration.
- `results/figures/`: Selected figures used in the thesis report.
- `results/tables/`: Final metric summaries.
- `report/`: Thesis-I report PDF.
- `data/README.md`: Dataset source and download notes.

## Main Results

The XGBoost point model substantially improved over the persistence baseline. The conformalized XGBoost quantile interval improved test coverage from 78.60% to 80.77%, while increasing PINAW only slightly from 11.39% to 11.64% of rated capacity.

## Tools

Python, Jupyter Notebook, pandas, NumPy, scikit-learn, XGBoost, Matplotlib, and Git.
