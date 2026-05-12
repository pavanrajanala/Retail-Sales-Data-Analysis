# Retail Sales Data Analysis using SQL

## Project Overview
This project analyzes retail sales data using SQL to extract meaningful business insights.  
The project focuses on sales performance, customer behavior, product trends, and revenue analysis.

---

## Objectives
- Analyze retail sales performance
- Identify top-selling products
- Track monthly sales trends
- Understand customer purchase behavior
- Generate reports for business decision-making

---

## Tools & Technologies
- SQL
- MySQL / PostgreSQL / SQLite
- CSV Dataset

---

## Features
- Data cleaning and preprocessing
- Complex SQL queries
- Sales trend analysis
- Customer behavior analysis
- Revenue and product performance analysis

---

## SQL Concepts Used
- SELECT Statements
- WHERE Clause
- GROUP BY
- ORDER BY
- Aggregate Functions
- JOIN Operations
- Subqueries

---

## Project Structure

```bash
Retail-Sales-Data-Analysis/
│
├── dataset/
│   └── retail_sales.csv
│
├── sql_queries/
│   └── queries.sql
│
├── reports/
│   └── insights.txt
│
└── README.md
```

---

## Sample SQL Queries

### Total Revenue

```sql
SELECT SUM(Quantity * Price) AS TotalRevenue
FROM retail_sales;
```

### Top Selling Products

```sql
SELECT Product, SUM(Quantity) AS TotalSold
FROM retail_sales
GROUP BY Product
ORDER BY TotalSold DESC;
```

### Monthly Sales Trend

```sql
SELECT MONTH(OrderDate) AS Month,
       SUM(Quantity * Price) AS MonthlyRevenue
FROM retail_sales
GROUP BY MONTH(OrderDate)
ORDER BY Month;
```

---

## Key Insights
- Electronics products generated the highest revenue
- Laptop sales contributed significantly to total sales
- Monthly sales increased during seasonal periods
- Repeat customers improved overall business growth

---

## Future Improvements
- Create interactive dashboards using Power BI or Tableau
- Add Python-based data analysis
- Implement sales forecasting models

---

## Author
**Pavan Rajanala**
