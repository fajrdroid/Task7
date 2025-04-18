# Task 7 – Sales Summary with SQLite and Python

## Objective
Analyze basic sales data stored in a SQLite database using Python, SQL, and matplotlib.

--
##  Tools Used

- Python
- SQLite3 (built-in)
- Pandas
- Matplotlib

---

##  What I Did

- Connected to a SQLite database using Python.
- Ran an SQL query to get total quantity sold and total revenue per product.
- Loaded the result into a pandas DataFrame.
- Printed the result in the console.
- Visualized the revenue with a simple bar chart.

---

##  SQL Query Used

```sql
SELECT 
    product, 
    SUM(quantity) AS total_quantity, 
    SUM(quantity * price) AS revenue 
FROM sales 
GROUP BY product;
```
