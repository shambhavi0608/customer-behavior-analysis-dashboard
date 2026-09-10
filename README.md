📊 Customer Behavior Analysis Dashboard

An end-to-end Business Intelligence project analyzing retail customer shopping behavior using Excel, MySQL, Python, and Power BI.

🚀 Project Overview

Retail companies generate large volumes of customer transaction data, but converting that raw data into actionable insights is a real challenge. This project builds a complete analytics pipeline — from raw CSV to an interactive dashboard — to help a retail business understand customer demographics, spending patterns, discount behavior, and subscription trends.

🎯 Business Problem

A retail company wants to better understand its customers' shopping behavior to improve sales, customer satisfaction, and long-term loyalty. This project answers the overarching question:

How can the company leverage customer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?

🛠 Tech Stack
Microsoft Excel — Data quality checks (duplicates, missing values, outliers)
Python (Pandas, SQLAlchemy) — Data cleaning and loading
MySQL — Structured querying and business analysis
Power BI — Interactive dashboard and visualization
📂 Repository Structure
customer-behavior-analysis-dashboard/
│
├── Dataset/
│   ├── customer_shopping_behavior.csv
│   └── customer_shopping_behavior.xlsx
│
├── SQL/
│   └── queries.sql
│
├── PowerBI/
│   ├── Customer_Behavior_Dashboard.pbix
│   └── Dashboard_Screenshot.png
│
├── README.md
└── Interview_Preparation.md
🔄 Data Pipeline
Excel — Data Quality Check: Verified the raw dataset for duplicate Customer IDs, missing values (Review Rating), and outliers (Purchase Amount) before loading it downstream.
Python (Pandas): Loaded the CSV, cleaned column names into snake_case, imputed missing values category-wise, engineered new features (Age Group, Purchase Frequency in days), and removed a redundant column.
MySQL: Loaded the cleaned data into a MySQL database using SQLAlchemy, then wrote SQL queries to answer 10 business questions using subqueries, CTEs, CASE statements, and window functions.
Power BI: Connected to MySQL via ODBC, built DAX measures and a calculated Age Group column, and designed an interactive dashboard with KPI cards, bar charts, a donut chart, and slicers.
📌 SQL Concepts Used
Aggregate Functions (SUM, AVG, COUNT)
GROUP BY / ORDER BY
Subqueries
CASE Statements
Common Table Expressions (CTEs)
Window Functions (ROW_NUMBER, PARTITION BY)
✨ Key Dashboard Features
Executive KPI Cards (Number of Customers, Avg Purchase Amount, Avg Review Rating)
Revenue & Sales by Category
Revenue by Age Group
Subscription Status Breakdown
Interactive Slicers (Gender, Category, Shipping Type, Subscription Status)
📊 Business Insights
Subscribed customers make up only ~27% of the customer base but show different average spend patterns than non-subscribers.
Certain products maintain consistently high review ratings and can be positioned for premium pricing.
Express shipping customers spend more on average than Standard shipping customers.
The majority of the customer base falls into the "Loyal" segment (10+ previous purchases).
Middle-aged and Young Adult customer groups drive the highest share of total revenue.
🚀 Getting Started
Import Dataset/customer_shopping_behavior.csv into MySQL.
Run the queries in SQL/queries.sql to reproduce the analysis.
Open PowerBI/Customer_Behavior_Dashboard.pbix in Power BI Desktop to explore the interactive dashboard.
💼 Author

Shambhavi
