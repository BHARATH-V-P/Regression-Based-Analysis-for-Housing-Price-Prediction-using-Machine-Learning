# Regression-Based Analysis for Housing Price Prediction using Machine Learning

This project focuses on predicting housing prices using various machine learning models. The aim is to provide accurate predictions based on a comprehensive dataset and detailed feature engineering.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Developing an optimized house price prediction model using a very large dimensional dataset after its thorough evaluation and cleaning. Conducted elaborate EDA to evaluate feature variability for accurate 
classification predictions. Evaluated feature importance using permutation importance to reduce dimensionality. Performed feature engineering to understand its elaborate effect on the machine learning models 
such as Linear Regression, Random Forest Regressors, XGB Regressors, and MLP Regressors. Performed model stacking and improved overall model R2 score by 10%.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_GITHUB_USERNAME/Regression-Based-Analysis-for-Housing-Price-Prediction-using-Machine-Learning.git
2. Navigate to project directory:
   cd Regression-Based-Analysis-for-Housing-Price-Prediction-using-Machine-Learning
3. Install the dependencies:
   pip install -r requirements.txt

## Usage

1. Prepare your dataset: Place your dataset in the data/ directory. Ensure it is named housing prices-training set.csv or adjust the script accordingly.
2. Open the Jupyter Notebook:
   jupyter notebook "Regression-Based Analysis for Housing Price Prediction using Machine Learning.ipynb"
   The script will:
   -Preprocess the data
   -Perform feature engineering
   -Train and evaluate models
   -Save results in the results/ directory
3. Review the results:
   Evaluation Metrics: Found in results/evaluation_metrics.txt
   Predictions: Found in results/predictions.csv

## Features
-Data Preprocessing: Handles missing values, normalization, and encoding.
-Feature Engineering: Includes permutation importance and feature selection.
-Model Training: Utilizes Linear Regression, Random Forest Regressors, XGBoost Regressors, and MLP Regressors.
-Model Stacking: Combines models to enhance performance.
-Evaluation: Performance metrics and predictions are saved for review.

## Results
-Performance Improvement: R2 score improved by 10% through model stacking.
-Evaluation Metrics: Detailed in results/evaluation_metrics.txt.
-Predictions: Available in results/predictions.csv.

## Contributing
-Contributions are welcome! To contribute:

-Fork the repository
-Create a feature branch (git checkout -b feature-branch)
-Commit your changes (git commit -am 'Add new feature')
-Push to the branch (git push origin feature-branch)
-Create a new Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
