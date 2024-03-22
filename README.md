# Meta-Learning for Time Series Forecasting in ATM Load Series

This repository contains the Jupyter notebooks and datasets used in our project focused on developing a meta-classifier for time series forecasting, specifically applied to ATM load predictions. Our approach consists of extracting significant features from time series data and constructing a meta-model that selects the optimal forecasting model based on those features.

## Project Overview

Our goal is to improve both the accuracy and efficiency of forecasting models for ATM load series by:
- Employing various methods for feature extraction from time series data.
- Developing a meta-classifier to determine the most suitable forecasting model based on extracted features.

## Quick Results Overview

Our methodology demonstrated a noticeable improvement in forecasting accuracy:
- Custom features significantly enhanced performance.
- The meta-classifier outperformed the best individual model in terms of average SMAPE by 0.1\% and was more accurate than the most commonly effective model by 8.4\%.

## How to Run the Code

### Step 1: Feature Extraction (`Feature_extraction.ipynb`)

1. Begin by running `Feature_extraction.ipynb`. This notebook is designed to extract and analyze features from time series data, employing various techniques including tsfresh and catch22, alongside our custom-developed methods.
2. The execution of this notebook results in the creation of several CSV files containing the extracted features for subsequent steps:
   - `All_features.csv`
   - `Tsfresh_relevant.csv`
   - `Catch22_features.csv`
   - `Ordinary_features.csv`
   - `Selected_features.csv`

### Step 2: Meta-Model Construction (`Meta-model.ipynb`)

1. Ensure the CSV files generated in Step 1 are located in the same directory as the `Meta-model.ipynb` notebook for easy access.
2. Proceed to run `Meta-model.ipynb`. This notebook focuses on constructing and evaluating the meta-model using the previously extracted features.

## Reproducibility

This project is structured to ensure easy reproducibility. By following the above instructions, any reviewer should be able to replicate all the code executions and analyses with minimal effort. The project is designed to run efficiently without requiring high computational resources.
