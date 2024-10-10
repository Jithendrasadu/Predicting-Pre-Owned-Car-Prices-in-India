# Predicting Pre-Owned Car Prices in India

## Project Overview
This project aims to develop a predictive model for estimating the sale price of used vehicles in India using historical sales data. The model will assist businesses and consumers in making informed decisions regarding vehicle purchases and sales.

## Last Updated
May 9, 2023

## Business Question
Can historical data of past car sales in India be used to predict the sale price of a used vehicle? By creating a predictive model, businesses can assess potential inventory purchases, repair expenses, and provide consumers with fair value for trade-ins or purchases of used vehicles. 

## Business Case
The pre-owned car market in India was valued at $23 billion in FY 2021-22 and is projected to grow at a CAGR of 19.5% until FY 2026-27. The market remains largely unorganized, and a standardized tool for predicting pre-owned car prices is lacking. This project seeks to create a transparent tool for both buyers and sellers, enhancing the car buying process.

## Analytics Question
- What is the effect of various factors (kilometers driven, age of vehicle, owner type, etc.) on the price of a pre-owned car in India?
- To what extent do these variables affect the accuracy of the predictive model?

## Dataset Description
- The dataset comprises 2,237 observations sourced from Kaggle, including key predictors such as:
  - New Price
  - Model
  - Kilometers Driven
  - Age of Vehicle
  - Owner Type
  - Fuel Type
  - Vehicle Condition
  - Transmission Type

### Dataset Link
You can download the dataset from the following link: [Pre-Owned Car Prices Dataset](https://www.kaggle.com/datasets/ankits29/used-car-price-data).

## Descriptive Analytics
Descriptive analytics were conducted using R, including correlation matrices, histograms, and box plots. Key insights include:
- The selling price data shows an approximate normal distribution with mild skewness.
- Outliers were identified in various variables, indicating the need for further analysis.

## Modeling Methods
### Initial Model Specification
- Two Ordinary Least Squares (OLS) models were created:
  - **Fit Model**: Continuous variables only
  - **Full Model**: Includes categorical variables

### Model Candidates
- Standardization Model
- Principal Components Regression (PCR)
- Random Forest (non-parametric model)

### Cross-Validation Testing
K-Fold Cross Validation (K=10) was conducted to measure model accuracy, with the Random Forest model yielding the best RMSE (Root Mean Square Error) of 84,380 and a predictive accuracy of 86.7%.

## Analysis of Results
- The Random Forest model demonstrated the best predictive accuracy.
- Age of Vehicle and Original Price emerged as the most significant predictors.

## Conclusions
- Random Forest outperformed other models in predictive accuracy.
- Recommendations include conducting analyses on larger datasets and exploring non-linear models for improved accuracy.

## Challenges Faced
- Data preprocessing and transformation were challenging, particularly in filling missing values and handling zero values in the dataset.

## Future Work
- Conduct analysis with an expanded dataset.
- Explore non-linear modeling approaches.


