# TASK-6 - Sales Trend Analysis Using Aggregations

## 🎯 Objective
The goal of this task is to analyze sales data over time using SQL aggregate functions. Specifically, we want to understand how revenue and order volume vary month by month, and identify trends such as peak months, average order values, and top-performing products.

## 🛠️ Tools Used
- **SQL (MySQL / PostgreSQL compatible)**
- **online_sales** table from the provided dataset

## 🧠 Concepts Applied

### 1. Extracting Time Components
We use `EXTRACT(YEAR FROM order_date)` and `EXTRACT(MONTH FROM order_date)` to break down the date into year and month for grouping purposes.

### 2. Aggregation Functions
- `SUM(amount)` is used to calculate total revenue.
- `COUNT(DISTINCT order_id)` gives us the number of unique orders (order volume).
- `AVG()` and `LAG()` are used in extended queries for deeper trend analysis.

### 3. Grouping and Sorting
Data is grouped by both year and month using `GROUP BY` to aggregate values over time. `ORDER BY` ensures the results are sorted chronologically.

### 4. Filtering and Limiting
Using `LIMIT` helps us retrieve specific insights like the **top 3 months by sales**. You can also add `WHERE` clauses for custom time ranges.

## 📈 Sample Insights You Can Get

- Which months generated the highest revenue?
- What is the average revenue per order each month?
- Which products are the top sellers?
- On which days do people order the most?

## 🧪 Extended Analysis (Optional)
Extra queries were added to deepen the analysis:
- Monthly average order value
- Month-over-month revenue growth
- Top-selling products
- Order distribution by weekdays

These provide actionable insights for business decisions like marketing campaigns or inventory planning.
