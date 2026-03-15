# FinMark Sales Forecasting Model with Data Visualization

## Project Overview

This project is part of the **MO-IT134 Machine Learning course Milestone 2 requirement**. The objective is to extend the predictive modeling work from Milestone 1 and implement a **time series forecasting model** that predicts FinMark Corporation’s future sales performance.

Using historical transaction data, the model analyzes trends and patterns in sales activity and generates a **six-month sales forecast**. Data visualization techniques are also applied to clearly present sales trends, smoothed patterns, and projected outcomes.

The goal of this project is to support **data-driven decision making** by helping the organization anticipate future demand and plan business operations more effectively.

---

# Dataset Description

The forecasting model uses the cleaned datasets prepared in Milestone 1.

## Customers Dataset
Contains information about customer companies including:
- Company ID
- Company Profit
- Customer attributes used in the predictive model

## Products Dataset
Includes product-related information such as:
- Product ID
- Product Price
- Product category information

## Transactions Dataset
Contains transaction-level sales data including:
- Transaction ID
- Company ID
- Product ID
- Transaction Date
- Quantity purchased
- Total Cost

These datasets were **cleaned, validated, and integrated during Milestone 1** to ensure consistency and accuracy before applying forecasting techniques.

---

# Methodology

The forecasting workflow follows several key steps:

## 1. Data Preparation
- Load cleaned datasets
- Convert transaction dates into datetime format
- Aggregate transactions to produce **monthly sales values**

## 2. Time Series Construction
Monthly sales data is created by grouping transaction data by month and calculating the total revenue for each period.

## 3. Trend Smoothing Techniques
To better understand sales behavior, smoothing techniques were applied:

- **Moving Average (3-month window)** to reduce short-term fluctuations
- **Simple Exponential Smoothing (SES)** to emphasize recent observations

These techniques help reveal the underlying trend in the sales data.

## 4. Forecasting Model
The final forecasting model used is **Holt’s Exponential Smoothing (Trend Model)**.

This model captures:
- Long-term trends in sales
- Gradual increases or decreases in revenue over time

Using this model, the system generates **a six-month forecast of future sales**.

---

# Data Visualizations

Several visualizations were created to communicate insights clearly:

## Monthly Sales Trend
Shows the actual monthly revenue trend over time.

## Moving Average Smoothing
Highlights the overall direction of sales by reducing random fluctuations.

## Simple Exponential Smoothing
Provides smoothed values that give more weight to recent data.

## Holt Trend Forecast
Shows projected sales values for the next six months.

These visualizations help stakeholders easily understand patterns, trends, and projected business performance.

---

# Forecast Output

The forecasting model generates predicted sales values for the **next six months**, helping FinMark anticipate future demand.

The forecast results are visualized using charts that display:
- Historical sales data
- Smoothed trend patterns
- Projected future sales

These insights can help support decisions related to:
- Business planning
- Inventory management
- Marketing strategies
- Resource allocation

---

# Technologies Used

The project was implemented using the following tools:

- Python
- Pandas – Data manipulation and preprocessing
- Matplotlib – Data visualization
- Seaborn – Statistical visualization
- Statsmodels – Time series forecasting models
- Jupyter Notebook – Development environment

---

# Repository Structure

MO-IT134 Milestone 2 Forecasting Project
│
├── Milestone 2.ipynb
│   Main notebook containing the forecasting model and visualizations
│
├── customers_cleaned.csv
│   Cleaned customer dataset
│
├── products_cleaned.csv
│   Cleaned product dataset
│
├── transactions_cleaned.csv
│   Cleaned transaction dataset
│
└── README.md
    Project documentation

    
---

# Conclusion

This project demonstrates how **time series analysis and forecasting techniques** can be used to analyze historical sales data and generate meaningful future predictions.

By applying smoothing techniques and Holt’s forecasting model, the project provides **a structured approach to predicting FinMark’s future sales performance**, supported by clear and informative visualizations.

The results of this analysis can help the organization make **more informed strategic decisions** based on projected trends.
