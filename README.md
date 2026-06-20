# customer_behavior_analysis
End-to-end retail analytics project. Data cleaning in Python, 10 business SQL queries in PostgreSQL, and an interactive Power BI dashboard. Analyzes 3,900 transactions across customer segments, revenue trends, and discount behavior.

📌 Overview

This project follows the complete data analyst workflow — from raw data to business recommendations. The goal was to analyze customer shopping patterns and answer key business questions to guide strategic decisions around subscriptions, discounts, product positioning, and targeted marketing.


📂 Dataset

PropertyDetailRows3,900Columns18SourceRetail transactional datasetMissing Data37 null values in Review Rating column

Key Features:


Customer demographics — Age, Gender, Location, Subscription Status
Purchase details — Item, Category, Purchase Amount, Season, Size, Color
Behavior signals — Discount Applied, Frequency of Purchases, Shipping Type, Review Rating, Previous Purchases



🛠️ Tools & Technologies

LayerToolsData Cleaning & EDAPython (pandas, numpy), Jupyter NotebookDatabasePostgreSQL, pgAdminBusiness AnalysisSQL (CTEs, Window Functions, Aggregations, Subqueries)VisualizationPower BI, DAXReportingMS Word, Gamma (PPT)


🔄 Project Steps

1. Data Cleaning (Python)


Loaded dataset using pandas and explored structure via df.info() and df.describe()
Imputed 37 missing Review Rating values using category-wise median
Renamed all columns to snake_case for consistency
Engineered 2 new features: age_group (binned from Age) and purchase_frequency_days
Verified that discount_applied and promo_code_used were redundant — dropped promo_code_used
Exported cleaned DataFrame directly into PostgreSQL via Python


2. SQL Business Analysis (PostgreSQL)

Wrote 10 structured queries to answer real business questions:

#Question1Revenue by Gender2High-Spending Discount Users (above average spend)3Top 5 Products by Average Review Rating4Shipping Type Comparison (Standard vs Express)5Subscribers vs Non-Subscribers (spend & revenue)6Discount-Dependent Products (top 5 by discount rate)7Customer Segmentation (New / Returning / Loyal)8Top 3 Products per Category (Window Function)9Repeat Buyers & Subscription Correlation10Revenue by Age Group

3. Power BI Dashboard


Connected Power BI directly to PostgreSQL
Built 3 DAX measures: Number of Customers, Average Purchase Amount, Average Review Rating
Designed slicers for Subscription Status, Gender, Category, and Shipping Type
Created visuals: KPI cards, donut chart, bar charts by category and age group


4. Report & Presentation


Compiled findings into a structured project report
Built a presentation using Gamma summarizing the pipeline, insights, and recommendations
