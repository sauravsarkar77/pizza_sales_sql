MySQL Project   -  🍕 Pizza Hut Sales Analysis.
This project demonstrates a complete end-to-end sales analysis workflow for Pizza Hut using MySQL. It showcases database design, SQL querying, and business insights derived from a real-world dataset downloaded from GitHub.

🚀 Project Overview
- Objective: Analyze Pizza Hut’s sales performance by building a relational database and running SQL queries to answer key business questions.
- Tools Used:
- 🧮 Excel → Data cleaning & transformation
- 🗄️ MySQL → Database creation, schema design, queries
- 📊 SQL Queries → Business insights & performance analysis

🔧 Process Breakdown
1. 📂 Data Preparation
- Downloaded dataset from GitHub.
- Cleaned raw data in Excel.
- Removed duplicates & null values.
- Standardized formats (dates, product names, time).
- Applied formulas for derived metrics.
- 
2. 🗄️ Database Creation
- Designed and created a Pizza Hut Sales Database in MySQL.
- Structured into four interconnected tables.
a. order_details : contains (order_details, order_id, pizza_id, quantity) 
b. orders        : contains (order_id, order_date, order_time)
c. pizza_types   : contains (pizza_type_id, name, category, ingredients)
d. pizzas        : contains (pizza_id, pizza_type_id, size, price)
-
3. 🔗 Relationships
- orders ↔ order_details → Linked via order_id
- order_details ↔ pizzas → Linked via pizza_id
- pizzas ↔ pizza_types → Linked via pizza_type_id
- This relational structure ensures normalized data and efficient querying.
-
4. 🧮 SQL Queries & Insights :
Ran 13 business-focused SQL queries to extract insights, including:
- Retrieve the total number of orders placed.
- Calculate the total revenue generated from pizza sales.
- Identify the highest-priced pizza.
- Identify the most common pizza size ordered.
- List the top 5 most ordered pizza types along with their quantities.
- Join the necessary tables to find the total quantity of each pizza category ordered.
- Determine the distribution of orders by hour of the day.
- Join relevant tables to find the category-wise distribution of pizzas.
- Group the orders by date and calculate the average number of pizzas ordered per day.
- Determine the top 3 most ordered pizza types based on revenue.
- Calculate the percentage contribution of each pizza type to total revenue.
- Analyze the cumulative revenue generated over time.
- Determine the top 3 most ordered pizza types based on revenue for each pizza category.

📈 Key Insights
- Revenue Drivers: Large-sized pizzas contributed the highest share of revenue.
- Customer Behavior: Peak orders occurred during evening hours.
- Top Performers: The Thai Chicken Pizza, The Bbq Chicken Pizza & The California Chicken Pizza categories dominated both order volume and revenue.
- Category Contribution: Each pizza category’s percentage share was calculated to identify strategic focus areas.
