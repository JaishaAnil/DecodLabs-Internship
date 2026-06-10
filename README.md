# SQL Data Analysis Project

## 📌 Project Overview

This project was completed as part of the DecodeLabs Data Analytics Internship Program. The objective was to perform SQL-based data analysis on an e-commerce dataset and extract meaningful business insights using SQL queries.

## 🎯 Objectives

* Import and analyze a dataset using SQLite.
* Perform data retrieval using SELECT statements.
* Apply filtering and sorting techniques.
* Use aggregate functions such as COUNT(), SUM(), and AVG().
* Analyze trends using GROUP BY and ORDER BY clauses.

## 🛠️ Tools Used

* DB Browser for SQLite
* SQLite
* Microsoft Excel
* GitHub

## 📂 Dataset Information

The dataset contains order-related information, including:

* Order ID
* Date
* Customer ID
* Product
* Quantity
* Total Price
* Payment Method
* Order Status
* Referral Source
* Shipping Information

## 📊 SQL Queries Performed

### 1. Dataset Preview

```sql
SELECT * FROM "Dataset for Data Analytics (2)" LIMIT 10;
```

### 2. Total Number of Orders

```sql
SELECT COUNT(*) AS TotalOrders
FROM "Dataset for Data Analytics (2)";
```

### 3. Total Revenue

```sql
SELECT SUM(TotalPrice) AS TotalRevenue
FROM "Dataset for Data Analytics (2)";
```

### 4. Average Order Value

```sql
SELECT AVG(TotalPrice) AS AverageOrderValue
FROM "Dataset for Data Analytics (2)";
```

### 5. Orders by Payment Method

```sql
SELECT PaymentMethod, COUNT(*) AS Orders
FROM "Dataset for Data Analytics (2)"
GROUP BY PaymentMethod;
```

### 6. Orders by Status

```sql
SELECT OrderStatus, COUNT(*) AS Orders
FROM "Dataset for Data Analytics (2)"
GROUP BY OrderStatus;
```

### 7. Top Products by Revenue

```sql
SELECT Product,
SUM(TotalPrice) AS Revenue
FROM "Dataset for Data Analytics (2)"
GROUP BY Product
ORDER BY Revenue DESC
LIMIT 5;
```

## 🔍 Key Insights

* Calculated the total number of orders.
* Determined overall revenue generated.
* Identified the average order value.
* Analyzed customer payment preferences.
* Evaluated order status distribution.
* Identified top-performing products by revenue.

## ✅ Conclusion

This project provided hands-on experience with SQL data analysis techniques. By applying SQL queries and aggregation functions, valuable insights were extracted from the dataset. The project strengthened practical knowledge of database querying, data filtering, grouping, and business intelligence analysis.

## 👨‍💻 Internship Project

**Program:** DecodeLabs Data Analytics Internship
**Project:** SQL Data Analysis (Project 3)
