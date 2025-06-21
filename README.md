# 📈 Additive Time Series Sales Forecasting Model

Welcome to this Additive Time Series Forecasting project! This Python code demonstrates how to build and evaluate a linear regression model with seasonal effects to predict sales over time.

## 🚀 Project Overview

This project uses historical sales data (vente_maillots_de_bain.csv) to forecast future sales by capturing both trend and seasonality:

Trend is modeled as a continuous index of time.
Seasonality is captured using monthly dummy variables (one-hot encoded month names).
The model is trained on 75% of the data and tested on the remaining 25%.
Model performance is evaluated with Mean Absolute Error (MAE) on both train and test sets.
Results are visualized with the predicted vs actual sales and a 95% confidence interval for test predictions.
#### 🧩 How It Works

DataPreparation class:
Loads the CSV, converts dates, creates month dummies, and splits data into training/testing sets.
Additif class:
Builds a linear regression model with sklearn and fits an OLS model with statsmodels to get confidence intervals. Prints training/testing MAE and plots predictions.
#### 📊 Visual Output
<img width="910" alt="Screenshot 2024-12-20 at 15 12 32" src="https://github.com/user-attachments/assets/9c272d61-79cb-4b41-9c4e-9a2dd83da2cd" />
You get a clear graph showing:

Original sales data (blue dots for train, red dots for test)
Fitted and forecasted sales (blue and red lines)
95% confidence intervals shaded in red for test forecasts
This visualization helps to understand how well the model captures the underlying trends and seasonality.

#### ⚙️ How to Run

Make sure you have the required packages installed:
pip install numpy pandas scikit-learn statsmodels matplotlib
Place the dataset vente_maillots_de_bain.csv in the same folder as the script.
Run the script.
Enjoy the output and visualize your sales forecasting!
#### 🔍 Use Cases

Forecasting sales for seasonal products like swimwear 🩱
Understanding the impact of time and seasonal patterns on business metrics
Learning additive models for time series in Python
