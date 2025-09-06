![SQL](https://img.shields.io/badge/SQL-SQLite-blue)
![Project](https://img.shields.io/badge/Project-Retail_Sales-orange)

# SQL_RetailSales_Project

 Retail Sales Analysis with SQL
 
## 📌 Project Overview

This project involves analyzing a retail sales dataset using SQL to generate meaningful business insights. The goal is to explore product performance, customer behavior, sales trends, and store-level contributions by writing SQL queries across multiple related tables.
________________________________________

 ## 📂 Repository Structure
- `queries.sql` → All SQL queries used in this project  
- `Sales_Analysis with SQL.pdf` → Report with insights  
- `Retail_sales.sqbpro` → SQLite project file (can be opened in DB Browser)
________________________________________  

 ## 🔍 Key Insights
- Store A generated the highest revenue in 2025  
- Smartphones and laptops were top sellers across all stores  
- Customer retention was highest in Q3 2025
________________________________________ 

| Table      | Description |
|------------|-------------|
| products   | Contains product information such as ID, name, category, and unit price. |
| customers  | Includes customer details like ID, name, and location. |
| sales      | Tracks each sale (product ID, customer ID, store ID, quantity, price, date). |
| stores     | Lists store information (store ID, name, and location). |

________________________________________ 

## 🧱 Dataset Description

The dataset simulates a retail environment and includes the following tables:
Table Name	Description
products	Contains product information such as ID, name, category, and unit price.
customers	Includes customer details like ID, name, and location.
sales	Tracks each sale, including product ID, customer ID, store ID, quantity, unit price, and date of sale.
stores	Lists store information such as store ID, store name, and location.

Source: Generated for learning purposes by ChatGPT.
________________________________________

## 💡 Project Scope

This project focuses on solving real-world analytical queries using SQL.

### 📊 Sales & Revenue Analysis

1.	What is the total revenue generated per product?
2.	Which store generated the highest revenue in 2025?
3.	Which month had the highest total sales across all stores?
4.	What is the average order value per store?
________________________________________
### 🛒 Product Insights

5.	Which are the top 5 best-selling products by quantity sold?
6.	List products that were never sold.
7.	Which products have a high price but low sales volume?
________________________________________
### 🧍‍♂️ Customer Behavior

8.	Which customer made the highest number of purchases?
9.	Which customer spent the most in total?
10.	Find customers who made purchases in every quarter of 2025.
________________________________________
### 🏪 Store Performance

11.	Which store had the most diverse product sales (sold the most different products)?
12.	Find the peak sales day for each store.
13.	Which store had the highest average order value?
________________________________________
### 📈 Trends & Comparisons

14.	Show monthly revenue trends over 2024–2025.
15.	Compare average revenue per store in 2024 vs 2025.
16.	What is the trend of total units sold per month?
________________________________________
### 🔎 Advanced Challenge

17.	Which products were consistently top-selling (in top 3) every month?
18.	Find products whose sales dropped 3 months in a row.
19.	Find customers who only purchased from one store
_______________________________________

## Sales & Revenue Analysis
```sql
SELECT product_id, SUM(quantity * unit_price) AS total_revenue
FROM sales
GROUP BY product_id
ORDER BY total_revenue DESC;
```
________________________________________






  
















