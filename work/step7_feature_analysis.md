# Step 7: Feature Analysis

## Target Column
ctr

## Correlation Analysis

The numerical features were analyzed to understand their relationship with CTR.

### Top Positive Features
- engagement_rate: 0.0969
- scroll_rate: 0.0130
- clicks_90d: 0.0106

### Top Negative Features
- days_with_impressions: -0.1295
- word_count: -0.1186
- char_count: -0.1081
- avg_position: -0.0726

## Observation

The correlation values are generally low, which indicates that CTR is influenced by multiple features rather than a single factor.

## Potential Features for Modeling

- search_volume
- competition
- cpc
- content_type
- main_intent
- word_count
- impressions_90d
- clicks_90d
- engagement_rate
- avg_position
- trend_pct