# laptop-price-prediction
## Table of Contents

1. [Assignment](#assignment)
2. [Data Exploration and Processing](#data-exploration-and-processing)
3. [Multicollinearity Check](#multicollinearity-check)
4. [Train/Val/Test Split](#trainvaltest-split)
5. [Classical Machine Learning](#classical-machine-learning)
6. [Deep Learning](#deep-learning)
7. [Feature Selection](#feature-selection)

## Assignment

The goal of this project is to build and train machine learning models to predict the price of laptops based on their attributes, with the objective of minimizing the Root Mean Squared Error (RMSE).

## Data Exploration and Processing

The dataset is explored, processed, and cleaned using various techniques:
- Concatenating training, validation, and test datasets
- Handling missing values and dropping unnecessary columns
- Transforming categorical variables into numerical format
- Feature engineering for specific columns (e.g., RAM size, screen size, resolution)
- Encoding categorical variables using one-hot encoding and creating dummy variables

## Multicollinearity Check

Multicollinearity is addressed through Variance Inflation Factor (VIF) analysis. Features with VIF scores above 20 are iteratively removed until multicollinearity is mitigated. The correlation matrix of the final dataset is visualized.

## Train/Val/Test Split

The dataset is split into training, validation, and test sets. The machine learning models expect the target variable in a specific shape, and the data is appropriately reshaped.

## Classical Machine Learning

Various classical machine learning models are implemented and evaluated, including Linear Regression, MLP Regressor, Decision Tree Regressor, Random Forest Regressor, Gradient Boosting Regressor, Extra Trees Regressor, and a Voting Regressor combining multiple models.

## Deep Learning

Artificial Neural Networks (ANN) are explored with both a base model and a complex model. The models are trained, and their performances are compared. The Voting Regressor from classical models is chosen as the official solution due to its superior performance on this dataset.

## Feature Selection

Feature selection is performed using f_regression and RandomForestRegressor for feature importance. Although feature selection hurts the performance for this task, the methods applied are presented. The RandomForestRegressor's feature importance is visualized, and the impact on model performance is assessed.

Feel free to explore the details of each section in the corresponding notebooks and adjust the parameters as needed. The primary focus is on creating a robust and accurate model for predicting laptop prices based on the provided attributes.
