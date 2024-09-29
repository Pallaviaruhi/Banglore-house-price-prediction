# House Price Prediction in Bangalore 🏠
This project focuses on predicting house prices in Bangalore based on features such as BHK, square footage, number of bathrooms, and location. Multiple regression algorithms were tested, with Linear Regression yielding the best results after hyperparameter tuning and cross-validation.

## Table of Contents
Project Overview

Dataset

Data Preprocessing

Modeling and Hyperparameter Tuning

Results

Installation

Usage

Future Work

### Project Overview
The goal of this project is to predict house prices in Bangalore using features such as BHK, square footage, bathrooms, and location. Several regression models were evaluated, including Linear Regression, Lasso Regression, and Decision Tree Regressor. Linear Regression performed the best, achieving an accuracy of 81.83% after hyperparameter tuning with GridSearchCV.

### Dataset :https://www.kaggle.com/amitabhajoy/bengaluru-house-price-data
The dataset includes the following features:

BHK (Number of bedrooms)

Square footage (Total area of the house)

Number of bathrooms

Location (categorical)

### Data Preprocessing
Steps taken for data preprocessing:

Data Cleaning: Handled missing values and removed outliers.

Feature Engineering: Applied one-hot encoding for categorical variables (location).

Scaling: Standardized the numerical features (BHK, square footage, bathrooms) to improve model performance.

### Modeling and Hyperparameter Tuning
Models evaluated: Linear Regression, Lasso Regression, and Decision Tree Regressor.

K-Fold Cross Validation was implemented (5-fold) with Linear Regression, achieving an average accuracy of 80%.

GridSearchCV was used for hyperparameter tuning to optimize model performance.

The final model, Linear Regression, achieved an accuracy of 81.83% on the test set.

### Results
Final Model: Linear Regression

Accuracy: 81.83%

K-Fold Cross Validation Accuracy (5-fold): ~80%

### Installation
Clone the repository:

git clone https://github.com/yourusername/house-price-prediction.git

Install dependencies:

pip install -r requirements.txt

### Usage
After installing dependencies, you can run the model using the following command:

python predict.py --input <input-data>

Example input:

json

{
  "BHK": 3,
  
  "SquareFootage": 1500,
  
  "Bathrooms": 2,
  
  "Location": "Indira Nagar"
}

### Future Work
Implement additional machine learning algorithms such as XGBoost or LightGBM.

Perform more advanced feature engineering, like adding geographical data for better predictions.

Explore UI/UX integration to build an interactive web interface.
