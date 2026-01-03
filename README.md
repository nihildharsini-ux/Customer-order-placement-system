Customer Order Placement System

Objective:
To create a servlet + JDBC application where customers place an order, and the servlet stores it in the database.

Description:
Customer enters name, item, and quantity through an HTML form.
Servlet stores the order in the database and prints an order summary.
Uses init() for DB connection and destroy() for cleanup.

HTML:
•	Form for entering name, item, quantity

Servlet:
1.init() → establish DB connection
2.service() →
3.Read parameters
4.Insert into orders table
5.Display confirmation
6.destroy() → close connection

Database:
CREATE DATABASE orderdb;

USE orderdb;

CREATE TABLE orders (
    order_id INT AUTO_INCREMENT PRIMARY KEY,
    customer_name VARCHAR(100),
    item_name VARCHAR(100),
    quantity INT
);


