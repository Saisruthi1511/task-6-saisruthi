# Task 6: Sales Trend Analysis Using SQL Aggregations

##  Objective
Analyze monthly and yearly sales trends using SQL by creating a database, inserting sample sales data, and applying aggregation functions to uncover revenue patterns.

##  Tools Used
- SQL (MySQL / SQLite)
- Aggregate Functions: `SUM()`, `COUNT(DISTINCT)`, `AVG()`
- Time Functions: `YEAR()`, `MONTH()`
- String Functions: `CONCAT()`, `LPAD()`
- Clauses: `GROUP BY`, `ORDER BY`, `LIMIT`

##  Project Workflow

### 1. Database Creation
- Created a new database named **sales_trend_analysis**.

### 2. Table Creation
- Created a table called **online_sales** with columns:
  - `order_id` (Primary Key)
  - `order_date` (Date of purchase)
  - `amount` (Transaction amount)
  - `product_id` (Product identifier)

### 3. Data Insertion
- Inserted 18 realistic sales records covering different months and years.

### 4. Sales Trend Analysis
Executed the following SQL queries:
- Monthly Revenue and Order Volume
- Yearly Revenue Summary
- Top 3 Months by Revenue
- Average Order Amount per Month


##  Key Queries Explained

- **Monthly Revenue and Orders**:  
  Using `YEAR(order_date)`, `MONTH(order_date)`, `SUM(amount)`, `COUNT(DISTINCT order_id)`.

- **Yearly Revenue**:  
  Summarized total sales per year using `GROUP BY YEAR(order_date)`.

- **Top 3 Revenue Months**:  
  Used `CONCAT()`, `LPAD()`, and `ORDER BY` with `LIMIT 3`.

- **Average Order Value**:  
  Calculated monthly average using `AVG(amount)`.
## Files Included
- `task6_sales_trend_full.sql` — Full SQL script (database, table, data, queries)
- `task6_output_sample.csv` — (Optional) Example result table
- `README.md` — Project documentation

##  Key Learnings
- Mastered use of `GROUP BY`, `ORDER BY`, `LIMIT` for time-based analysis.
- Used `YEAR()` and `MONTH()` functions for time extraction.
- Aggregated total revenue, order volume, and average order values.
- Learned string manipulation (`CONCAT()`, `LPAD()`) for clean date formatting.
