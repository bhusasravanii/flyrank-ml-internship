# Capstone Report — Machine Learning

- **Author:** Bhusa Sravani
- **Lane:** Machine Learning
- **Repo:** https://github.com/bhusasravanii/flyrank-ml-internship
- **Date:** 06-08-2026

# 0. Abstract

This project aims to predict the Click-Through Rate (CTR) of online content using historical content and performance features. The dataset was provided as part of the FlyRank ML Internship and contains approximately 30,000 content records. A Linear Regression model was developed after performing data cleaning, preprocessing, feature selection, and encoding. The baseline model achieved an MAE of 0.8009, an RMSE of 3.0220, and an R² score of 0.1215. The resulting model provides a baseline for estimating CTR and can support future optimization of content performance.

# 1. Problem Framing

The objective is to predict the CTR of a content page before publication or optimization.

Unit of analysis:
- Individual content page

Output:
- Predicted CTR value

Decision supported:
- Identify content likely to achieve higher engagement and prioritize optimization efforts.

Cost of incorrect prediction:
- High-performing content may be overlooked or low-performing content may receive unnecessary optimization.

Machine learning helps discover relationships between content attributes and CTR that are difficult to identify manually.

# 2. Data Safety

Dataset used:
- FlyRank ML Internship Dataset

Excluded columns:
- content_id
- client_id

Reason:
- Identifier columns do not contribute to prediction and may introduce bias.

Potential leakage:
- Label-derived features were reviewed carefully.
- No client-identifying information was included in the final model.

No personally identifiable information is present in the work directory.

# 3. Baseline

Baseline Model:
- Linear Regression

This provides an interpretable benchmark against which future models such as Random Forest, XGBoost, or Gradient Boosting can be compared.

# 4. Model / Analysis

Model:
- Linear Regression

Target:
- ctr

Features:
- Search volume
- Competition
- CPC
- Word count
- Character count
- Engagement metrics
- Performance metrics
- Trend-related features
- Content attributes

Categorical variables were encoded using One Hot Encoding.

Missing numerical values were imputed using the median.

Missing categorical values were imputed using the most frequent category.

# 5. Evaluation

Train/Test Split:
- Training: 24,000 rows
- Testing: 6,000 rows

Metrics

MAE:
0.8008683012800075

RMSE:
3.0219915606666947

R² Score:
0.12151269919632524

The model establishes a baseline for CTR prediction. While the predictive performance is modest, it provides a foundation for evaluating more advanced models.

# 6. Interpretation

The model indicates that search-related features, engagement metrics, and content characteristics influence CTR prediction.

The baseline Linear Regression model captures some relationships but leaves room for improvement through feature engineering and more advanced algorithms.

# 7. Recommendation

Recommended next steps:

- Experiment with Random Forest Regressor.
- Evaluate Gradient Boosting or XGBoost.
- Perform feature engineering.
- Apply feature selection techniques.
- Tune model hyperparameters.
- Compare multiple regression models using the same evaluation metrics.

# 8. Reproducibility

Environment:
- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook

Random Seed:
42

Project can be reproduced by:

1. Clone the repository.
2. Install dependencies.
3. Open the notebooks.
4. Run preprocessing.
5. Train the Linear Regression model.
6. Evaluate using MAE, RMSE, and R² Score.

# 9. Acknowledgments & Data Credit

This project was built using the FlyRank ML Internship Dataset.

Data Source:
https://flyrank.ai

Special thanks to FlyRank for providing the internship project and dataset for educational purposes.