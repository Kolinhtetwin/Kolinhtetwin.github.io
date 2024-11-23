---
title: "Exploring Sales and Customer Insights with Tableau"
date: 2023-11-20
draft: false
links:
  - icon: fab fa-github
    url: https://github.com/Kolinhtetwin/MedScan-Insight
author: "Lin Htet Win"
tags:
  - Tableau
  - Data Visualization
  - Interactive Dashboards
  - Storytelling
  - SQL
  - Flask
badges:
 - Tableau Public
 - Data Visualization
 - Interactive Dashboards
 - Storytelling

image: /projects/sales_dashboard/sales_dashboard title picture.jpg
description: "A web application designed to predict the disease with symptoms."
toc: 
---

In today’s data-driven world, businesses thrive on visual analytics to make informed 
decisions. I'm thrilled to showcase two dynamic dashboards (view [here](https://public.tableau.com/views/Sales_Dashboard_17322898738320/SalesDashboard?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)) that I created during my 
Tableau learning journey with **Data with Baraa**. These dashboards provide comprehensive 
insights into sales performance and customer metrics, empowering businesses to make 
data-driven decisions. Let's explore the specifics of these projects and discover 
how you can leverage these insights.

<hr>

### Project Overview
The primary goal of these dashboards was to analyze and track performance in 2023 
compared to 2022. This project features two key dashboards: Sales Analysis and 
Customer Analysis, aiming to deliver a view of:
- Sales Trends (via the Sales Dashboard)
- Customer Behavior and Profitability (via the Customer Dashboard)

#### Sales Analysis Dashboard

The Sales Analysis dashboard includes several essential components:
- **Total Sales**: Displays the total sales amount with a percentage change compared to the previous year.
- **Total Profit**: Shows the total profit earned and its year-over-year growth.
- **Total Quantity**: Indicates the total quantity of items sold.
- **Sales by Subcategory**: A bar chart that breaks down sales by different product subcategories.
- **Sales Trends**: A line chart illustrating sales trends over time, highlighting peaks and troughs.

#### Customer Analysis Dashboard

The Customer Analysis dashboard features:
- **Total Customers**: Displays the total number of customers and the percentage change from the previous year.
- **Total Sales Per Customer**: Shows the average sales amount per customer and its year-over-year growth.
- **Total Orders**: Indicates the total number of orders and their growth compared to the previous year.
- **Customer Distribution by Number of Orders**: A bar chart showing how many customers made one, two, or more orders.
- **Top 10 Customers by Profit**: A table listing the top 10 customers by profit, including their last order date, profit, sales, and number of orders.

<hr>

### Key Insights
#### Sales Analysis Dashboard Insights
![Sales Dashboard](/projects/sales_dashboard/Sales_dashboard.png)

One of the key insights from the Sales Dashboard is the achievement of $733K in total sales, a 20.4% increase from 2022, demonstrating the success of the sales strategy and strong market presence. Over the year, sales trends show clear fluctuations, with identifiable high and low-performing months. These patterns offer valuable opportunities to plan marketing campaigns and optimize inventory. The subcategory breakdown highlights phones and chairs as top-performing categories, underscoring their importance for driving growth. Conversely, categories such as labels and envelopes continue to underperform, signaling the need for strategic adjustments.

#### Customer Analysis Dashboard Insights
![Customer Dashboard](/projects/sales_dashboard/Customer_dashboard.png)

The Customer Dashboard shows an 8.6% increase in total customers and a 28.3% rise in total orders, reflecting successful customer acquisition and growing engagement. However, a deeper analysis of order frequency per customer shows the potential to further grow average order frequency through targeted campaigns like subscription services or bundle offers. The top 10 customers contribute significantly to both profit and sales. Creating exclusive programs or providing personalized service for these customers could strengthen loyalty and further increase their contribution.

<hr>

### Technical Details
To create these dashboards, I used data provided by Data with Baraa, including transaction details from the past three years. I leveraged Tableau's powerful data blending capabilities to combine multiple data sources and used calculated fields to derive key metrics such as year-over-year growth and profit margins. Interactive elements like filters allow users to drill down into specific time periods and product categories.

<hr>

### Interactive Elements
The dashboards are designed with user interactivity in mind:
- **Filters**: Enable users to refine data by year, region, or category.
- **Tooltips**: Provide additional context on hover, making it easier to understand data points.
- **Color Coding**: Highlights trends, anomalies, and areas requiring attention, improving decision-making efficiency.


<hr>

### Conclusion
In conclusion, these sales and customer analysis dashboards serve as powerful tools for visualizing key business metrics and uncovering actionable insights. I hope you find them as valuable as I do in making data-driven decisions. Feel free to explore the interactive dashboards yourself [here](https://public.tableau.com/views/Sales_Dashboard_17322898738320/SalesDashboard?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link). If you have any questions or feedback, please leave a comment or reach out to me directly.
