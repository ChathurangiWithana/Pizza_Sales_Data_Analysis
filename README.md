# Pizza_Sales_Data_Analysis

This Pizza Sales Analysis project demonstrates the power of SQL and Excel in transforming raw data into actionable business intelligence, driving informed decision-making for pizza restaurant operations.


## PROBLEM STATEMENT

To simulate a real-world business scenario, this project analyzes sales data from a hypothetical popular pizza restaurant. 
The goal is to uncover actionable insights into customer preferences, sales trends, and product performance to optimize sales and marketing strategies.
1.   KPI’s REQUIREMENT

     To gain insights into our business performance, we will calculate key metrics derived from our pizza sales data, including...


         •	Total Revenue  -  The sum of the total price of all pizza orders
     
         •	Average Order Value -  The average amount spent per order, calculated by dividing the total revenue by the total number of orders. 
     
         •	Total Pizzas Sold  -  The sum of the quantities of all pizzas sold.
     
         •	Total Orders   -  The total number of orders placed.
     
         •	Average Pizzas Per Order  -  The avarage number of pizzas sold per order, calculated by dividing the total number of pizzas sold by the total number of orders.

2. CHARTS REQUIREMENT

   To gain a deeper understanding of our pizza sales, we aim to visualize key trends and patterns. To achieve this, we will create charts;

       •	Daily trend for Total Orders  -  A bar chart that displays the daily trend of total orders over a specific time period. This chart will help us identify any patterns or fluctuations in order volumes on a daily basis.
       •	Hourly trend for Total Orders  -  A line chart that illustrates the hourly trend of total orders throughout the day. This chart will allow us to identify peak hours or periods of high order activity.
       •	Percentage of sales by pizza Category  -  A pie chart that shows the distribution of sales across different pizza categories. This chart will provide insights into the popularity of various pizza categories and their contribution to overall sales. 
       •	Percentage of sales by pizza Size  -  A pie chart that represents the percentage of sales attributed to different pizza sizes. This chart will help us understand customer preferences for pizza sizes and their impact on sales.
       •	Total pizzas sold by pizza Category  -  A funnel chart that presents the total number of pizzas sold for each pizza category. This chart will allow us to compare the sales performance of different pizza categories.
       •	Top 5 best sellers by total pizzas sold  -  A bar chart highlighting the top 5 best-selling pizzas based on the total number of pizzas sold. This chart will help us identify the most popular pizza options.
       •	Bottom 5 worst sellers by total pizzas sold  -  A bar chart showcasing the bottom 5 worst-selling pizzas based on the total number of pizzas sold. This chart will enable us to identify underperforming or less popular pizza options.


## SOFTWARE USED
   

  Microsoft 365/Excel:  Version 2406

  Microsoft SQL Server Manamgement Studio - v20.2

  MS SQL Server: 19.0

## DATASET

Source:  Kaggle

Format:  .CSV

The dataset contain information about pizza orders, including specifics about the pizza variants, quantities, prices, dates, times, and categorization details. The data spans a period of one year, from January 2015 to December 2015.

### DATA STRUCTURE 

pizza_sales.csv dataset

rows : 48620

columns : 14

     
    •	pizza_id : A unique identifier linking to a specific name of the pizza. (PK)
    •	order_id : unique identifier for all the orders made. (PK)
    •	total_orders: frequency of each order id
    •	pizza_name_id : Specifies the name of the specific pizza variant ordered.
    •	quantity : The number of units of a specific pizza variant ordered within an order.
    •	order_date : The date when the order was placed
    •	order_day : The day when the order was placed
    •	order_time : The time when the order was placed
    •	unit_price : The cost of a single unit of the specific pizza variant.
    •	total_price : The cost of all unit of the specific pizza variant.
    •	pizza_Regularize : Represents the size of the pizza (e.g., small, medium, large)
    •	pizza_category : Indicates the category of the pizza, such as vegetarian, non-vegetarian, etc.
    •	pizza_ingredients : Provides a list or description of the ingredients used in the pizza.
    •	pizza_name : Specifies the name of the specific pizza variant ordered.


## DATA TRANSFORMATION


Data Transformation: Total Orders

    Column: total_orders

    Calculation: =1/COUNTIF(B:B,[@[order_id]])

    Description: This column calculates the reciprocal of the frequency of each order ID within the dataset. Essentially, it represents the proportion of the total dataset accounted for by a single occurrence of that order ID. 

Data Transformation: Pizza Size
    
    Column: pizza_Regularize
    
    Description: Transformed the abbreviations in the "pizza_Regularize" column into descriptive names, enhancing comprehension and usability of the dataset. This modification improves clarity and facilitates easier interpretation of        the pizza sizes.

      S >> Small

      M >> Medium

      L  >> Large

      XL >> X-Large

      XXL >> XX-Large

#### Check out the [SQL Queries for Pizza Sales Data](https://github.com/ChathurangiWithana/Pizza_Sales_Data_Analysis/blob/main/SQL%20Queries%20for%20Pizza%20Sales%20Data)

## BUILDING THE DASHBOARD 

The dashboard provides a comprehensive overview of pizza sales performance, featuring key performance indicators such as total revenue, orders, average order value, and pizzas sold. It also includes visualizations of busiest days and times, sales trends, best-selling and worst-selling pizzas. This holistic approach empowers stakeholders with actionable insights to optimize operations, inform product strategies, and drive sales growth.

![dashboard screenshot](https://github.com/user-attachments/assets/b3d30917-88ec-4663-a2bb-6ca1387f8602)

## INSIGHTS







   
