# customer-segmentation-rfm
Customer Segmentation and Retention Analysis using RFM and Cohort Analysis with Python, Pandas, and Seaborn.
Customer Segmentation and Retention Analysis using RFM and Cohort Analysis
Project Overview

This project focuses on analyzing customer purchasing behavior using RFM (Recency, Frequency, Monetary) Analysis and Cohort Analysis. The goal is to segment customers based on their transaction patterns and analyze customer retention trends over time.

By applying these analytical techniques, businesses can identify high-value customers, understand purchasing behavior, and develop strategies to improve customer retention and marketing effectiveness.

The analysis is performed using Python libraries such as Pandas, NumPy, Matplotlib, and Seaborn.

Dataset Description

The dataset used in this project is the Online Retail Dataset.

It contains transactional data from an online retail store.

Key Columns in Dataset
Column	Description
InvoiceNo	Unique invoice number
StockCode	Product code
Description	Product description
Quantity	Number of products purchased
InvoiceDate	Date and time of purchase
UnitPrice	Price of each product
CustomerID	Unique customer identifier
Country	Customer location
Data Preprocessing

Before performing analysis, the dataset was cleaned and processed.

Steps Performed

Removed missing values

Rows with missing CustomerID were removed.

Removed cancelled transactions

Invoice numbers starting with 'C' represent cancelled orders.

Converted data types

Converted InvoiceDate to datetime format.

Created Total Purchase Value

Total Price = Quantity × UnitPrice

Removed negative or invalid values

Negative quantities or prices were excluded.

Exploratory Data Analysis (EDA)

EDA was conducted to understand customer purchasing behavior.

Key Observations

Most customers come from United Kingdom.

Certain months show higher purchase activity, indicating seasonal trends.

Some customers purchase frequently with high spending, while others buy only once.

Visualization techniques used:

Distribution plots

Bar charts

Heatmaps

Time-series purchase trends

Libraries used:

Matplotlib

Seaborn

RFM Analysis

RFM stands for:

Recency (R) → How recently a customer made a purchase

Frequency (F) → How often a customer purchases

Monetary (M) → How much money a customer spends

RFM Calculation

Recency = Current Date – Last Purchase Date

Frequency = Number of purchases made by the customer

Monetary = Total amount spent by the customer

Each metric is scored using quantile-based ranking (1–5 scale).

Higher scores represent better customer engagement and value.

Customer Segmentation

Based on RFM scores, customers are grouped into segments such as:

Segment	Description
Champions	Recently purchased, frequent buyers, high spending
Loyal Customers	Frequent buyers with consistent purchases
Potential Loyalists	Recent customers with moderate purchases
At Risk	Customers who haven't purchased recently
Lost Customers	Customers inactive for a long time

These segments help businesses design targeted marketing campaigns.

Cohort Analysis

Cohort Analysis groups customers based on their first purchase date and tracks their purchasing behavior over time.

Cohort Definition

A cohort is a group of customers who made their first purchase in the same month.

Example:

Customers who first purchased in January 2011 belong to the January cohort.

Retention Rate Calculation

Retention measures how many customers return to make repeat purchases.

Retention Rate = (Customers Active in Period / Customers in First Cohort Month)

This is visualized using a cohort retention table and heatmap.

Cohort Visualization

Cohort heatmaps show:

Customer retention across months

Decline or growth in returning customers

Insights from cohort visualization:

Many customers purchase once and do not return

A smaller group of customers shows consistent repeat purchasing behavior

Tools and Libraries Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Jupyter Notebook

Key Business Insights
1. High-Value Customers

Customers classified as Champions and Loyal Customers generate a large portion of revenue.

Strategy:
Provide loyalty rewards and personalized offers.

2. At-Risk Customers

Customers who have not purchased recently but had good past purchase behavior.

Strategy:
Use email campaigns, discounts, or reminders to re-engage them.

3. One-Time Buyers

A large portion of customers purchase only once.

Strategy:
Offer follow-up promotions or recommendations to encourage repeat purchases.

4. Retention Trends

Cohort analysis shows retention decreases over time.

Strategy:
Improve customer experience, product recommendations, and loyalty programs.

Business Value of This Project

This solution helps businesses:

Identify high-value customers

Improve customer retention strategies

Understand customer purchase behavior

Optimize marketing campaigns

Increase customer lifetime value (CLV)

Conclusion

By combining RFM segmentation and Cohort Analysis, businesses gain deeper insights into customer behavior and retention patterns.
