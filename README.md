# task3_elevate_labs-
# 📊 Task 3: SQL for Data Analysis

## 🎯 Objective
Use SQL to analyze and extract meaningful insights from a relational database. This task demonstrates proficiency in SQL operations such as filtering, joining, aggregating, subqueries, views, and performance optimization.

---

## 🛠 Tools Used
- SQL Engine: MySQL / PostgreSQL / SQLite *(choose the one you used)*
- Text Editor: VSCode / Sublime / DB Browser *(optional)*
- Dataset: Ecommerce_SQL_Database *(or any alternative dataset)*

---

## 📄 Contents
- `elevate_labs_task-3(SQL Querries).sql`: Contains all SQL queries written for this task.
- `screenshots/`: Folder containing output screenshots of executed queries.
- `TASK_3_DATA_ANALYST.pdf`: Official task description (provided).

---

## ✅ Key Concepts Demonstrated

### 1. **Basic Queries**
- `SELECT`, `WHERE`, `ORDER BY`, `LIMIT`
  
### 2. **Aggregations**
- `SUM`, `AVG`, `COUNT`, `GROUP BY`, `HAVING`

### 3. **Joins**
- `INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`

### 4. **Subqueries**
- Used in `SELECT`, `WHERE`, and `FROM` clauses for nested logic.

### 5. **Views**
- Created views to simplify complex queries and reuse logic.

### 6. **Query Optimization**
- Added indexes to improve performance.
- Used `EXPLAIN` to analyze slow queries.

---

## 🔍 Sample Query Examples

```sql
-- Find total revenue per product
SELECT product_id, SUM(total_price) AS revenue
FROM orders
GROUP BY product_id
ORDER BY revenue DESC;
