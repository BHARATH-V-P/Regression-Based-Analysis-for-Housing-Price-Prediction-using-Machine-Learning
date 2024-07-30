# Regression-Based Analysis for Housing Price Prediction using Machine Learning

This project focuses on predicting housing prices using various machine learning models. The aim is to provide accurate predictions based on a comprehensive dataset and detailed feature engineering.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Results](#results)
- [License](#license)

## Introduction

   Developing an optimized house price prediction model using a very large dimensional dataset after its thorough evaluation and cleaning. Conducted elaborate EDA to evaluate feature variability for accurate 
   regression predictions. Evaluated feature importance using permutation importance to reduce dimensionality. Performed feature engineering to understand its effect on machine learning models such as Linear 
   Regression, Random Forest Regressors, XGBoost Regressors, and MLP Regressors. Improved overall model R² score by 10% through model stacking.

## Installation

1. Clone the repository:
   git clone https://github.com/BHARATH11112222/Regression-Based-Analysis-for-Housing-Price-Prediction-using-Machine-Learning.git

2. Navigate to project directory:
   cd Regression-Based-Analysis-for-Housing-Price-Prediction-using-Machine-Learning
   
4. Install the dependencies:
   pip install -r requirements.txt


## Usage

1. Prepare your dataset: Place your dataset in the data/ directory. Ensure it is named housing_prices_training_set.csv or adjust the script accordingly.
2. Open the Jupyter Notebook:
   jupyter notebook "Regression-Based Analysis for Housing Price Prediction using Machine Learning.ipynb"
   The script will:
   -Preprocess the raw data
   -Train and evaluate models
   -Perform feature engineering
   -Perform Hyperparameter tuning
   -Evaluate different models based on specific preprocessing done prior to model training
   -Save results in the results/ directory
4. Review the results:
   Evaluation Metrics: Found in results/evaluation_metrics.txt
   Predictions: Found in results/predictions.csv


## Features
   -Data Preprocessing: Handles missing values, normalization, and encoding.
   -Feature Engineering: Includes permutation importance and feature selection.
   -Model Training: Utilizes Linear Regression, Random Forest Regressors, XGBoost Regressors, and MLP Regressors.
   -Model Stacking: Combines models to enhance performance.
   -Evaluation: Performance metrics and predictions are saved for review.


## Results
   Baseline Model Performance
   -------------------------------
   Linear Regression: R² = 0.930, RMSE = $23,158.28
   Random Forest Regressor: R² = 0.892, RMSE = $28,791.35
   XGBoost Regressor: R² = 0.910, RMSE = $26,231.67
   MLP Regressor: R² = 0.836, RMSE = $35,467.19
   
   Hyperparameter Tuned Models
   --------------------------------
   Random Forest Regressor (Tuned): R² = 0.884, RMSE = $29,859.67
   XGBoost Regressor (Tuned): R² = 0.895, RMSE = $28,426.23
   MLP Regressor (Tuned): R² = 0.931, RMSE = $23,007.31
   
   Feature Engineered Dataset-Based Models
   ----------------------------------------   
   Random Forest Regressor: R² = 0.879, RMSE = $30,426.10
   XGBoost Regressor: R² = 0.900, RMSE = $27,676.39
   MLP Regressor: R² = 0.880, RMSE = $30,304.47
   
   Advanced Models
   ------------------------------------------
   Voting Regressor: RMSE = $23,136.85, MAE = $14,196.87
   Stacking Regressor with RF Meta Model: RMSE = $32,355.92, MAE = $16,893.47
   For detailed metrics, refer to the evaluation_metrics.txt.
   
   -Performance Improvement: R2 score improved by 10% through model stacking.
   -Evaluation Metrics: Detailed in results/evaluation_metrics.txt.
   -Predictions: Available in results/predictions.csv.


## License

   This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
