# Kaggle-HousePricePredictions

This repository contains the solution to the Kaggle challenge "House Prices - Advanced Regression Techniques." 
"The goal of this competition is to predict the final price of residential homes in Ames, Iowa, using a dataset with 79 explanatory variables."

## Introduction

"Ask a home buyer to describe their dream house, and they probably won't begin with the height of the basement ceiling or the proximity to an east-west railroad. But this playground competition's dataset proves that much more influences price negotiations than the number of bedrooms or a white-picket fence."

## Dataset

The dataset consists of two main files:
- `train.csv`: Training dataset containing features and target variable (SalePrice).
- `test.csv`: Testing dataset containing features without the target variable.

## Approach

### 1. Data Preprocessing

The preprocessing steps include:
- Combining the training and testing datasets.
- Cleaning missing values in categorical and numerical features.
- Feature engineering to create new relevant features.
- Feature transformation using logarithmic and cosine transformations.
- Categorical encoding of features.
- Numeric scaling of features.
- Target transformation using logarithmic transformation.

### 2. Building Models

We experimented with several regression models including CatBoost, Bayesian Ridge, and LightGBM. The models were trained on the preprocessed data and evaluated using cross-validation.

### 3. Ensemble Model

We constructed an ensemble model using Bagging (Bootstrap Aggregation) with the best-performing individual models.

## Results

The ensemble model achieved a root mean squared error (RMSE) of 0.12154.

## Future Work

Future work could involve:
- Fine-tuning hyperparameters for better model performance.
- Exploring other ensemble techniques such as stacking.
- Feature selection to improve model interpretability and reduce complexity.
