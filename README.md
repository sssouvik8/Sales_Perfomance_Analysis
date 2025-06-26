# 📊 Sales Performance Analysis Dashboard

## 📌 Project Overview
This project delivers an end-to-end sales performance dashboard using Power BI and SQL. It analyzes profitability, growth, regional sales, and budget utilization from five structured datasets. SQL is used to generate KPIs, which are visualized in Power BI with interactive filtering.

---

## 🛠 Tools & Technologies Used
- Power BI – Visual dashboard and data modeling
- SQL – KPI generation and aggregation
- CSV – Raw structured datasets

---

## 🔍 Key Insights

- 💰 **Total Sales and Total Profit** calculated using SQL
- 📈 **Year-over-Year Sales Growth** with % change logic using LAG
- 🧭 **Sales by Region** using JOIN and aggregation
- 🛒 **Budget Utilization by Product** – Shows which products over- or under-perform
- 🔎 Interactive filters for product, year, and region

---

## 📁 Files Included

| File/Folder | Description |
|-------------|-------------|
| `SQL_POWERBI_PROJECT.pbix` | Power BI report file |
| `SQL/SQL_Codes_With_Output.docx` | SQL queries with sample outputs |
| `Datasets/*.csv` | Raw datasets: sales, products, customers, budgets |
| `Screenshots/dashboard.png` | Final dashboard image |

---

## 🧾 SQL Summary

SQL queries were written to:
- Calculate total sales and profit
- Measure product-wise budget utilization
- Track sales growth by year (using CTE + LAG)
- Aggregate sales region-wise

Sample query:
```sql
SELECT SUM(Line_Total - Total_Unit_Cost) AS TotalProfit FROM Sales_Order;
