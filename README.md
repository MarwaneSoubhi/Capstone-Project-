# Video Game Sales Prediction Project
Project Overview
This project focuses on analyzing and modeling video game sales using a dataset that includes global sales figures, critic and user scores, genres, platforms, and release years. The primary objective was to build a regression model capable of predicting the global sales of a video game based on its characteristics.

Problem Statement
Can we predict the global sales of a video game using available metadata such as critic/user scores, genre, platform, and release year?

Dataset Description
The dataset used is the "Video Game Sales as at 22 Dec 2016" CSV file. It contains information on over 16,000 video games, including:

Sales data across North America, Europe, Japan, and other regions

Global sales

Game metadata such as genre, platform, year of release

Critic and user scores from Metacritic

Data Cleaning & Preparation
Removed rows with missing target values (Global_Sales) and key features (Genre, Year_of_Release)

Converted user scores from string to numeric, handling 'tbd' as missing

Applied one-hot encoding on categorical features (Genre, Platform)

Selected relevant numerical and encoded features for modeling

Exploratory Data Analysis (EDA)
The dataset was especially suitable for EDA, allowing us to identify trends such as:

Sales by genre and by region

Distribution of global sales (right-skewed)

Correlation between critic/user scores and sales

Models Tested
We implemented and compared several regression models:

Linear Regression

Ridge Regression (with GridSearchCV)

Random Forest Regressor (with hyperparameter tuning)


Model Evaluation
All models were evaluated using:

MAE (Mean Absolute Error)

RMSE (Root Mean Squared Error)

R² (coefficient of determination)

The best model, Random Forest with GridSearchCV, achieved:

MAE: 0.65

RMSE: 1.46

R²: 0.22

Conclusion
Although several regression models were tested and optimized, the results suggest that this dataset is more suitable for exploratory data analysis rather than predictive modeling. Many influential factors in video game sales are not captured in the dataset (e.g., marketing, release timing, franchise power). However, the project effectively demonstrates the full machine learning workflow: from data cleaning and EDA to feature engineering, model training, tuning, and evaluation.
