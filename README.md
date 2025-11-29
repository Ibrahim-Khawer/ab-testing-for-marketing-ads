A/B Testing for Marketing Ads
Project Overview

This project analyzes the performance of two marketing campaigns (“Ad” vs “PSA”) to determine which drives higher user conversion. Using real campaign data, the goal is to identify conversion differences across ad types, days of the week, and hours of the day, providing actionable insights for marketing strategy.

Dataset

Source: Marketing A/B campaign dataset (internal / Kaggle style)

Size: 588,101 user interactions

Columns:

user_id – unique user identifier

test_group – Ad vs PSA group

converted – 0/1 conversion indicator

total_ads – number of ads seen by the user

most_ads_day – day with most ad exposure

most_ads_hour – hour with most ad exposure

Key Steps

Data Cleaning

Removed unnecessary columns (Unnamed: 0)

Checked for duplicates and missing values

Verified column types

Exploratory Data Analysis (EDA)

Univariate analysis: Count plots & pie charts for categorical variables (test_group, converted, most_ads_day, most_ads_hour)

Numerical distribution: Histograms and boxplots for total_ads (with skew adjustment for outliers)

Bivariate Analysis

Conversion rates by test group, day, and hour

Crosstabs and bar charts to visualize patterns

Statistical Testing

Conversion differences by group: t-test / Mann-Whitney U test

Day and hour significance: Chi-square test

Key insight: Differences between Ad and PSA groups are statistically significant

Visualization

Bar charts for conversion rates by group

Hourly and daily conversion trends

Boxplots showing relationship between total_ads and conversion

Key Insights

Ad group has higher conversion rate than PSA group

Peak conversions occur on Tuesday and Wednesday, around 10 AM–2 PM

Users exposed to fewer than 50 ads convert at slightly higher rates; overexposure does not improve conversions

Statistical tests confirm that ad type, day, and hour affect conversion significantly
