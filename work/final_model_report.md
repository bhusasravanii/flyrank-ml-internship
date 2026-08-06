# Final Model Report

## Problem
Predict content CTR using content and performance features.

## Target Column
ctr

## Model Type
Regression

## Data Split
- Training samples: 24000
- Testing samples: 6000

## Preprocessing
- Numerical missing values handled using median imputation.
- Categorical missing values handled using most frequent imputation.
- Categorical features encoded using One Hot Encoding.

## Baseline Model
Linear Regression

## Features Used
- Search related features
- Content features
- Engagement features
- Performance metrics
- Trend features

## Evaluation Metrics

MAE:
0.8008683012800075

RMSE:
3.0219915606666947

R2 Score:
0.12151269919632524

## Conclusion

A regression model was successfully developed to predict CTR based on content characteristics and historical performance data. The baseline Linear Regression model achieved an MAE of 0.8009, an RMSE of 3.0220, and an R² score of 0.1215. These results provide a baseline that can be improved further by experimenting with more advanced regression models and additional feature engineering.