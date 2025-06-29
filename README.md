 Task Overview

This task involves analyzing tabular data by applying aggregate functions like `SUM`, `COUNT`, and `AVG`, and categorizing results using `GROUP BY` and `HAVING`.

Objective

Use aggregate functions to summarize numeric data
Categorize data using `GROUP BY`
Filter grouped data with `HAVING`

SELECT category_id, COUNT(*) AS total_products
FROM Products
GROUP BY category_id;

SELECT order_id, SUM(quantity) AS total_items
FROM OrderItems
GROUP BY order_id;

SELECT customer_id, COUNT(*) AS total_orders
FROM Orders
GROUP BY customer_id
HAVING COUNT(*) > 1;

SELECT category_id, AVG(price) AS average_price
FROM Products
GROUP BY category_id;




