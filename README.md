# Walmart-Sales-ML
# About the Project
This project analyzes the Walmart Weekly Sales dataset to support store-level operational planning. The main objective is to understand how sales behave during holiday vs. non-holiday weeks, and to identify the key factors (drivers) that explain weekly sales patterns across stores.

We begin with exploratory data analysis (EDA) to compare sales distributions in holiday and non-holiday periods and to rank stores based on their holiday uplift (i.e., how much average weekly sales increase during holiday weeks). Next, we apply machine learning (Random Forest / Logistic Regression) to:

forecast or classify weekly demand patterns, and
explain which variables contribute most to sales using feature importance (and optional interpretation tools).

The project produces actionable insights such as the most holiday-sensitive stores, the top drivers of weekly sales, and visual summaries that can help inform decisions on replenishment, staffing, and capacity planning during demand peaks.

# Team Member
[Nicolas Rojas Lopez](https://github.com/nicolasrojol)

# The Dataset
We use the Walmart Dataset (Weekly Sales) from Kaggle:

- Source: https://www.kaggle.com/datasets/yasserh/walmart-dataset
- Time period: weekly data from 2010 to 2012
- Unit of analysis: Store-week
Main variables:
- Store: store identifier (1–45)
- Date: week date
- Weekly_Sales: total weekly sales per store
- Holiday_Flag: 1 = holiday week, 0 = non-holiday week, Temperature, Fuel_Price, CPI, Unemployment: external/economic factors

# Methodology
1. Data Preparation
Convert Date to datetime, sort by store and date, check missing values
Create time features (e.g., month/week)
2. Holiday Impact Analysis
Compare average sales in holiday vs non-holiday weeks
Compute holiday uplift (%) and rank the most holiday-sensitive stores
Visualize results using bar charts/boxplots
3. Machine Learning Models
Random Forest Regression to model/forecast weekly sales and extract feature importance
Logistic Regression to classify high-demand week

# Key Outputs
1. Top stores with highest holiday uplift
2. Key drivers of weekly sales (overall and selected stores)
3. Forecast vs actual visualizations (selected stores)
