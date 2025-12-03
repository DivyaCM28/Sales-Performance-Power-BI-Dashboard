#Sales Performance Power BI Dashboard

**Interactive Data Analytics Report**

This repository contains a complete Power BI Sales Dashboard Project, designed to provide insights into sales performance, customer behavior, product trends, and profitability.
The dashboard is visually optimized using a dark theme, highlight colors, and KPI cards, giving a professional and modern analytics look suitable for portfolio and resume use.

**Project Overview**

This Power BI report analyzes end-to-end sales and customer data, enabling business users to:

Understand overall revenue, profit, and orders

Identify top-selling product lines

Track sales trends over time

Analyze country-wise and state-wise performance

Review customer insights such as quantity purchased and top buyers

Visualize profit distribution and year-over-year growth

**Datasets Used**

The dashboard is built using multiple data sources:

1. Orders Dataset
2. Customer Data
3. Customer Reviews
4. Customer Journey
5. Country/Region Data

**Key KPIs Displayed in Dashboard**

The dashboard highlights major business metrics:

Total Sales – 10M
Quantity Sold – 2.823K
AOV (Average Order Value) – 32.68K
% Orders Shipped – 93%
Total Profit – 9.80M

**Dashboard Visuals Included**

1. KPI Cards
Displays high-level performance metrics.

2. Sales Trend Over Time
Line chart representing sales growth across years.

3. Country-wise Sales Contribution
Bar chart with % contribution by each country.

4. State-Level Sales Tree Map
Shows the top performing states using a color-coded treemap.

5. Profit Distribution by Product Line
Donut chart showing contribution % of each category.

6. Funnel Chart – Top Product Categories
Highlights top-performing categories by profit.

7. Customer Analysis Table
A detailed table showing:

Sales, Quantity, Profit %, Product lines

**Power BI Features Used**

Custom KPI cards
DAX Measures
Conditional formatting
Drilldown using Date Hierarchy
Tree maps, Funnel charts, Donut charts
Slicers for Year, Region, and Product Line

**Tooltip customization**

Dark mode UI with highlighted borders

**Important DAX Measures**

Total Sales = SUM(Orders[Sales])  
Total Profit = SUM(Orders[Profit])  
Quantity Sold = SUM(Orders[Qty])  
AOV = DIVIDE([Total Sales], DISTINCTCOUNT(Orders[OrderLine]))  
% Orders Shipped = 
VAR shipped = CALCULATE(COUNT(Orders[Status]), Orders[Status] = "Shipped")
VAR totalOrders = COUNT(Orders[Status])
RETURN DIVIDE(shipped, totalOrders)

**Insights Delivered**

USA leads with highest sales contribution
Classic Cars and Motorcycles dominate product performance
Profit margin highest in Classic Cars at 41.44%

Few states contribute heavily (CA, MA, NY)

Customer segments show strong repeat purchase behavior
