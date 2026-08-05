# Step 9: Data Cleaning and Preparation

## Missing Value Analysis

Missing values were checked across all columns.

Columns with missing values:

| Column | Missing Count |
|---|---:|
| provider_used | 21438 |
| word_count | 7699 |
| char_count | 7699 |
| word_count_tier | 7699 |
| char_count_tier | 7699 |
| model_used | 5733 |
| trend_pct | 3388 |
| competition_level | 2610 |
| search_volume | 2468 |
| cpc | 2468 |

## Duplicate Check

Duplicate rows found:

0

## Data Cleaning Plan

- Remove identifier columns:
  - content_id
  - client_id

- Handle numerical missing values using appropriate imputation methods.

- Handle categorical missing values by replacing them with a separate category such as "Unknown".

- Encode categorical variables before model training.

- Keep `ctr` as the target variable.