# 🛍️ Retail Analytics & AI-Powered Sales Forecasting System

An end-to-end Retail Analytics and Machine Learning solution developed as a major project for the Unlox Academy Workshop. This system includes automated data cleaning, Exploratory Data Analysis (EDA), RFM customer segmentation, Random Forest time-series sales forecasting, dynamic Power BI integration, and a multi-page interactive Streamlit dashboard.

---

## 📌 Project Overview & Key Features

- **Data Engineering & Cleaning:** Automated scripts to handle missing values, correct data types, standardise dates, and engineer new metrics (e.g., total sales, revenue after discounts).
- **Exploratory Data Analysis (EDA):** Deep analytical insights into revenue trends, regional performance, top product categories, and rating distributions.
- **RFM Customer Segmentation:** K-Means Clustering model applied on Recency, Frequency, and Monetary (RFM) values to identify key customer and store profiles.
- **AI Sales Forecasting:** Time-series prediction model built with `RandomForestRegressor` to forecast future store revenue.
- **Interactive Multi-Page Streamlit App:** Clean UI with custom CSS styling and modular pages (`Sales Analysis`, `Store Analysis`, `Product Analysis`, `Forecasting`, `Segmentation`).
- **Power BI Integration:** Dedicated `.pbix` reporting dashboard for business users.

---

## 📂 Project Structure

```text
Retail Analytics System/
│
├── assets/                  # Custom CSS styling & media assets
│   ├── style.css
│   └── logo.png
│
├── dashboard/               # Multi-page Streamlit Application
│   ├── app.py               # Main entry script (Home Page)
│   └── pages/               # Sub-pages for interactive navigation
│       ├── 1_Sales_Analysis.py
│       ├── 2_Store_Analysis.py
│       ├── 3_Product_Analysis.py
│       ├── 4_Forecasting.py
│       └── 5_Segmentation.py
│
├── data/                    # Datasets folder
│   ├── raw/                 # Unprocessed raw sales data
│   └── processed/           # Cleaned and processed CSV datasets
│
├── database/                # SQL Database scripts
│   └── retail_analytics.sql # Schema & table creation scripts
│
├── models/                  # Saved Machine Learning models
│   └── sales_forecast.pkl
│
├── powerbi/                 # Power BI Dashboard file & documentation
│   └── Retail_Analytics.pbix
│
├── python/                  # Core Python modules
│   ├── data_cleaning.py
│   ├── eda.py
│   ├── segmentation.py
│   └── forecasting.py
│
├── requirements.txt         # Project dependencies
└── README.md                # Project documentation
