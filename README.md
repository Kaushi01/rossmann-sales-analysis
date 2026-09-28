# Rossmann Sales Analysis & Forecasting

Analysis of Rossmann drugstore sales using Python and Power BI. I explored what drives daily sales (promotions, day of week, season, store type) and built an XGBoost model to forecast sales.

## Objective
Understand what drives store sales and build a model that forecasts them accurately.

## Key Findings
- **Promotions work:** promo days average 8.2K in sales vs 5.9K without, about a 39% lift.
- **Sundays:** only 33 shops open on Sundays, but they average 8.2K, the highest of any day (tied with Monday).
- **Store types:** type b shops sell the most (10.2K average), but there are only 17 of them. Type a has the most shops (602).
- **Assortment:** assortment b averages 8.6K, vs 7.3K for c and 6.6K for a.
- **Seasonality:** December is the busiest month (8.6K average) and Saturday is the weakest day (5.9K).
- **Model:** the forecast has a 9.0% error vs 20.9% for the baseline.

## Tools Used
- Python (pandas, NumPy, Matplotlib)
- XGBoost for forecasting
- Power BI for the dashboard
- Google Colab

## Files
- `01_rossmann_eda.ipynb`: data exploration, feature engineering and the forecasting model
- `rossmann_dashboard_powerbi.pdf`: Power BI dashboard with 4 pages (Sales Insights, Model Forecast, Store Insights, Seasonality Insights)

## Dataset
Rossmann Store Sales from Kaggle: https://www.kaggle.com/c/rossmann-store-sales/data
(The raw data is not included in this repo.)

## Business Recommendations
1. Plan promotions around slow days (Saturday) and peak season (December).
2. Test Sunday opening in more shops, since the current Sunday shops perform strongly.
3. Look into why type b shops outperform and whether that can be replicated.

## Author
Kaushiki Sharma
