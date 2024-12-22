# SQL_pizzasales_complex_queries
The Pizza Sales Database Project is a robust SQL-based solution designed to manage and analyze pizza sales data effectively. 
This project involves creating a normalized database schema and executing complex queries to derive actionable insights into sales performance, orders.


## Features
- **Comprehensive Database Schema:** Structured around 4 core tables to handle pizzas, orders, and related details.
- **SQL Queries:** Includes a variety of queries to analyze sales, most popular pizzas, and daily sales performance.


## Technologies Used
- **SQL:** The core query language for managing the database and retrieving insights.
- **DBMS:** MySQL

## Schema Overview
The database consists of four main tables:

### `pizzas`
Stores details about each pizza available for sale.
- `pizza_id` 
- `pizza_type_id`
- `size`
- `price`

### `pizza_types`
Defines the different categories of pizzas (e.g., Veg, Non-Veg).
- `pizza_type_id` 
- `name`
- `category`
- `ingredients`

### `orders`
Contains records of customer orders.
- `order_id` (Primary Key, Not Null)
- `date`
- `time`

### `order_details`
Stores the details of the pizzas ordered, linked to the `orders` table.
- `order_detail_id` 
- `order_id` 
- `pizza_id` 
- `quantity`
