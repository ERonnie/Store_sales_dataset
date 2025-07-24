# Store Sales Dataset Analysis

## 📘 Overview

This repository contains an exploratory data analysis (EDA) of a daily store sales dataset. The dataset includes information on sales per store, along with indicators for promotions and holidays. The analysis focuses on understanding temporal sales patterns, comparing store performance, and evaluating the impact of external factors.

## 📂 Dataset Description

The dataset used is `store_sales.csv`, with the following columns:

- `date`: Date of the record
- `store`: Store ID
- `sales`: Total sales value for the store on that day
- `promo`: Indicates if a promotion was active (1 = yes, 0 = no)
- `holiday`: Indicates if the day was a holiday (1 = yes, 0 = no)

## 📊 Performed Analyses

### 🗓️ Sales Trend Over Time

- Computed **average daily sales per month** to visualize sales evolution.
- Identified periods of growth and decline throughout the year.

### 📆 Weekly Sales Pattern

- Calculated **average sales per day of the week**.
- Found that **Fridays and Saturdays** have the highest sales, while **Sundays and Mondays** tend to have the lowest.

### 💡 Promotion & Holiday Impact

- Compared **average sales on days with and without holidays**.
  - Holidays showed significantly higher sales.
- Assessed **sales behavior on promotion vs holidays**.
  - Promotional days tended to have slightly lower average sales.

### 🏬 Store Performance Comparison

- Ranked stores based on their **average daily sales**.
- Highlighted top-performing and low-performing stores.

### 📉 Time Series Decomposition

- Aggregated total daily sales across all stores.
- Applied **additive seasonal decomposition** to separate:
  - **Trend**: Overall direction of sales over time
  - **Seasonality**: Repeating weekly/monthly patterns
  - **Residual**: Unexplained noise or anomalies

## 📈 Key Insights

- **Holidays** drive a clear increase in daily sales.
- There is a strong **weekly pattern** in sales behavior.
- **Store performance varies** significantly, suggesting opportunities for targeted actions.
- The **decomposition reveals stable seasonal patterns** and highlights irregularities.
