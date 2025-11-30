# A/B Testing for Marketing Ads

## Business Problem

Marketing teams aim to optimize advertisement strategies to maximize user conversions. This project evaluates the effectiveness of two types of ads—commercial ads (**Ad**) and public service announcements (**PSA**)—to determine which drives higher conversion rates. By identifying statistically significant differences in user engagement, businesses can allocate advertising budgets more efficiently and improve campaign ROI.

## Project Details

- **Dataset**: [Marketing A/B Data](https://github.com/Ibrahim-Khawer/ab-testing-for-marketing-ads/blob/main/marketing_AB.csv) - 588,101 records
- **Tools & Libraries**: Python (**Pandas, NumPy, Seaborn, Matplotlib, statsmodels**)
- **Code**: [Click here to view notebook](https://github.com/Ibrahim-Khawer/ab-testing-for-marketing-ads/blob/main/AB_Testing_Marketing_Ads.ipynb)

## Data Preparation

- **Data Cleaning**: Removed unnecessary columns, checked for duplicates, ensured correct data types.
- **Exploratory Data Analysis (EDA)**:
  - Distribution of users across test groups
  - Overall conversion distribution
  - Conversion rates by group, day, and hour
  - Visualizations using bar charts and line plots

## Conversion Metrics

- **Conversion Rate (Ad vs PSA)**:
  - Ad: 2.55%
  - PSA: 1.79%
- **Absolute Lift**: 0.0077 → Ad group conversion higher by ~0.77 percentage points
- **Relative Lift**: 43% → Ad group performs 43% better relative to PSA

## Statistical Test

- **Two-Proportion Z-Test**: Z = 7.37, p < 0.000001 → statistically significant difference
- **Interpretation**: The Ad group truly performs better; difference is real, not random. You can confidently recommend running the Ad version.

## Key Findings

- Conversion rates vary by day of week (**Monday** and **Tuesday** highest) and hour of day (**4 PM** and **8 PM** peak).
- Users who saw more ads were more likely to convert, highlighting the importance of repeated exposure.

## Recommendations

1. Prioritize commercial ads over PSAs for higher conversions.
2. Optimize ad placements based on high-performing days and hours to maximize user engagement.
3. Repeated exposure to ads increases conversion likelihood; consider showing relevant ads multiple times per user.
