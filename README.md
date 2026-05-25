# Intraday-Market-Prediction-ML
## Overview
This project aims to predict the direction of end-of-day stock returns on the US equity market using intraday financial data.

The study was conducted as part of a Data Science & Financial Risk project at the University of Rennes.

## Objective
Predict the direction of returns between 2pm and 4pm using intraday returns observed between 9:30am and 2pm.

Target variable:
- -1 : significant decrease
- 0 : neutral movement
- 1 : significant increase

## Dataset
- ~843,000 observations
- 53 intraday return variables
- 5-minute frequency financial data

## Feature Engineering
Several categories of features were created:
- Momentum indicators
- Intraday structure
- Volatility measures
- Buyer/Seller pressure
- Trend indicators

## Models
### LightGBM
Gradient boosting model optimized for tabular financial data.

### Random Forest
Ensemble tree-based classifier robust to noisy market data.

### Stacking
Combination of LightGBM and Random Forest probabilities.

Optimal weights:
- 60% LightGBM
- 40% Random Forest

## Validation
- Stratified K-Fold Cross Validation (K=3)

## Results
- LightGBM accuracy: 0.4726
- Random Forest accuracy: 0.4713
- Stacking score: 0.4744
- Benchmark: 0.4174

The stacking approach successfully outperformed the benchmark.

## Tools & Libraries
- Python
- Pandas
- NumPy
- Scikit-learn
- LightGBM
- Machine Learning
- Financial Data Science

## Author
Inès Tapoayi
