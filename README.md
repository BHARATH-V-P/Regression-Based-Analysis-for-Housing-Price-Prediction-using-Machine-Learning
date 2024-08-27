# Regression-Based Analysis for Housing Price Prediction using Machine Learning

The project explores how different models such as Random Forest Regressor,XGB Regressor, LGB Regressor, etc. perform under different processes of data preprocessing and model optimization. The objective of this project is to create an efficient prediction model using information such as location, size, type of house, amenities etc. This repository includes a well structured readme file, relevant data, results and a well-structured python notebook, making it a comprehensive resource for a strong regression analysis model.


## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Results](#results)
- [License](#license)

## Introduction

Housing prices are influenced by a variety of features, each contributing differently to the overall dataset. The distinct nature of these features adds complexity to accurately characterizing individual data records. This project focuses on predicting housing prices using a well structured dataset with 81 predictors to create an efficient model through neccessary hyperparameter optimization. Key processes such as data cleaning and evaluation followed by EDA ìs performed to gain a better insight into the information available in the dataset. Feature importances where assesed for different models using concepts of permutation importance which in turn aided in evaluating the effect of PCA and dimensionality reduction. Various machine learning models, including Linear Regression, Random Forest Regressors, XGBoost Regressors, and MLP Regressors, were employed to predict housing prices. Predictability improvement beyond hyperparameter optimization of individual models where achieved by using a tuned stacking regressor which saw a boost in the r2 score by 10%.
   

## Installation

1. Clone the repository:
   git clone https://github.com/BHARATH-V-P/Regression-Based-Analysis-for-Housing-Price-Prediction-using-Machine-Learning_2.git

2. Navigate to project directory:
   cd Regression-Based-Analysis-for-Housing-Price-Prediction-using-Machine-Learning
   
4. Install the dependencies:
   pip install -r requirements.txt


## Usage

1. Prepare your dataset: Place your dataset in the data/ directory. Ensure it is named housing_prices_training_set.csv or adjust the script accordingly.
2. Open the Jupyter Notebook:
   jupyter notebook "Regression-Based_Analysis_for_Housing_Price_Prediction_using_Machine_Learning_2_final.ipynb"
   The script will:
   -Data Preprocessing: Handles missing values, normalization and encoding of all predictors as needed.
   -Perform EDA neccessary for optimum model training. 
   -Feature Engineering: Includes permutation importance and feature selection.
   -Model Training: Utilizes Linear Regression, Random Forest Regressors, XGBoost Regressors, and MLP Regressors.
   -Model Stacking: Combines models to enhance performance.
   -Save results in the results/ directory
4. Review the results:
   Evaluation Metrics: Found in results/evaluation_metrics.txt
   Predictions: Found in results/predictions.csv


## Features
   -Preprocess the raw data though data cleaning and data exploration
   -Train and evaluate models based on specific metrics such as RMSE, Inverse RMSE(for normalized target variable) and MAE.
   -Perform feature engineering based on results drawn from permutation importance and feature selection.
   -Perform Hyperparameter tuning using Bayesian Optimization and Optuna Optimization
   -Perfornm Ensembling using Stacking Regressors and Voting Regressors. Further improving them by iterative hyperparameter tuning.
   -Evaluation: Performance metrics and predictions are saved for review.


# Results

## Model Performance Comparison

- **Voting Regressor**: 
  - RMSE: 0.1248 ($23,136.85)
  - MAE: $14,196.87
  - Best overall performance with superior accuracy in predicting average prices.

- **MLP Regressor**: 
  - RMSE: 0.1704 ($35,467.19)
  - MAE: $22,592.49
  - Highest error metrics, indicating lower accuracy compared to other models.

- **Stacking Regressor**: 
  - RMSE: 0.1373 ($32,355.92)
  - MAE: $16,893.47
  - Higher RMSE and MAE compared to MLP, showing less accuracy for expensive properties.

## Baseline Model Performance

- **Linear Regression**:
  - RMSE: 0.1312 ($23,158.28)
  - MAE: $15,061.21
  - R²: 0.9301 (Highest R² score, strong baseline performance.)

- **Random Forest Regressor**:
  - RMSE: 0.1466 ($28,791.35)
  - MAE: $17,469.71

- **XGBoost Regressor**:
  - RMSE: 0.1450 ($26,231.67)
  - MAE: $17,367.99
  - R²: 0.9103

- **MLP Regressor**:
  - RMSE: 0.1704 ($35,467.19)
  - MAE: $22,592.49
  - R²: 0.8360 (Lowest R² score among the models.)

## Hyperparameter Tuned Models

- **Random Forest Regressor (Tuned)**:
  - RMSE: 0.1479 ($29,859.67)
  - MAE: $17,373.43

- **XGBoost Regressor (Tuned)**:
  - RMSE: 0.1406 ($28,426.23)
  - MAE: $16,432.65

- **MLP Regressor (Tuned)**:
  - RMSE: 0.1286 ($23,007.31)
  - MAE: $15,549.03
  - Significant improvement, comparable to the baseline model.

## Feature Engineered Dataset-Based Models

- **Random Forest Regressor**:
  - RMSE: 0.1481 ($30,426.10)
  - MAE: $17,522.78

- **XGBoost Regressor**:
  - RMSE: 0.1482 ($27,676.39)
  - MAE: $17,223.00

- **MLP Regressor**:
  - RMSE: 0.1594 ($30,304.47)
  - MAE: $20,811.16
  - Performance deteriorated with feature engineering.

## Voting Regressor

- **Performance**:
  - RMSE: 0.1248 ($23,136.85)
  - MAE: $14,196.87
  - Balanced prediction capabilities.

## Stacking Regressor

- **Performance**:
  - RMSE: 0.1373 ($32,355.92)
  - MAE: $16,893.47
  - Higher error metrics compared to other models, indicating a need for further tuning or feature adjustments.



## License

   This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
