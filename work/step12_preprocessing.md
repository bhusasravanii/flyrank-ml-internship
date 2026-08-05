# Step 12: Data Preprocessing

## Feature Types Identified

### Numerical Features
29 numerical columns were identified.

Examples:
- search_volume
- competition
- cpc
- word_count
- impressions_90d
- clicks_90d
- engagement_rate
- trend_pct

### Categorical Features
12 categorical columns were identified.

Examples:
- competition_level
- content_type
- main_intent
- provider_used
- model_used
- trend_direction

## Missing Value Handling

Numerical columns:
- Missing values handled using median imputation.

Categorical columns:
- Missing values handled using most frequent value imputation.

## Encoding

Categorical variables are converted into numerical values using One Hot Encoding.

## Preprocessing Pipeline

A ColumnTransformer pipeline was created to apply different transformations to numerical and categorical features before model training.