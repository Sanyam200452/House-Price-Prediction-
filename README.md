# House Price Prediction Project

## Overview

This project is part of a Kaggle competition focused on predicting house prices. The goal is to build a robust predictive model using a variety of techniques and data preprocessing methods. The final model utilizes a Voting Regressor that combines the predictions of multiple base models to enhance accuracy.

## Data Exploration and Visualization

Extensive data exploration was conducted to understand the underlying structure and characteristics of the dataset. Key steps included:

- **Graphical Analysis**: A range of plots, including histograms, KDE plots, and correlation heatmaps, were used to visualize the distributions of numerical and categorical variables, and to explore relationships between features.
- **Missing Data Analysis**: Detailed analysis of missing data was performed. Visualization techniques, such as bar plots and heatmaps, were employed to assess the extent and patterns of missingness, guiding the choice of imputation strategies.

## Data Cleaning and Preprocessing

Data preprocessing involved several critical steps:

- **Imputation**: Missing values were imputed using appropriate techniques, including mean, median, and mode imputation, based on the nature of the data. This ensured that the dataset was complete and ready for model training.
- **Feature Engineering**: New features were created to capture additional information that may enhance the model's predictive power. This included transformations, scaling, and encoding of categorical variables.

## Model Building

The core of the modeling process involved building a Voting Regressor, which aggregates the predictions of multiple strong base models on which grid search CV was applied to get the best hyperparameters:

- **Random Forest (RF)**: A robust ensemble learning method that combines multiple decision trees to improve predictive accuracy and control overfitting.
- **XGBoost (XGB)**: A powerful gradient boosting algorithm known for its efficiency and performance in predictive modeling tasks.
- **LightGBM (LGBM)**: A gradient boosting framework that uses tree-based learning algorithms, known for its speed and efficiency, particularly with large datasets.

## Model Evaluation and Selection

The models were evaluated using cross-validation and performance metrics, such as Mean Absolute Error (MAE) and Root Mean Square Error (RMSE). The Voting Regressor was chosen for its ability to leverage the strengths of individual models, providing a balanced and accurate prediction.

