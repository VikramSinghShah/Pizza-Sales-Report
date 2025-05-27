**📊 Project Title:**

**End-to-End Sales Analysis Dashboard Using SQL & Power BI & Excel.**

An end-to-end business intelligence project analyzing sales and customer data from 2023 to 2025 using SQL and Power BI. The goal was to uncover actionable insights into revenue trends, customer behavior, product performance, and regional sales, enabling better business decisions.

This project covers the complete data analysis workflow—starting with data extraction and transformation using SQL, followed by visualization and storytelling with Power BI.

🎯 Objective
To design a robust sales analysis solution that:

Tracks company revenue and profit growth

Identifies key customer and product segments

Highlights regional sales distribution

Provides interactive dashboards for decision-makers

🧰 Tools Used
Tool	Purpose
SQL (MySQL)	Data extraction, filtering, joins, aggregations
Power BI	Data modeling, DAX calculations, visualization
Power Query	Importing and shaping data
Excel/CSV	Data input and reference tables

🗃️ Datasets Used
Orders Table – Order ID, Customer ID, Product ID, Order Date, Sales, Quantity, Profit

Products Table – Product ID, Name, Category, Subcategory, Unit Cost

Customers Table – Customer ID, Segment, Country, Region

Date Table – Generated in Power BI for time intelligence

🧠 SQL Queries and Processing
Joined Orders, Customers, and Products tables

Aggregated sales, profit, and quantity at multiple levels (region, product, time)

Used GROUP BY, JOIN, and CASE statements for conditional analysis

Created views to optimize Power BI import

Example SQL Snippet:
sql
Copy
Edit
SELECT 
    o.OrderDate,
    c.Region,
    p.Category,
    SUM(o.Sales) AS TotalSales,
    SUM(o.Profit) AS TotalProfit
FROM Orders o
JOIN Customers c ON o.CustomerID = c.CustomerID
JOIN Products p ON o.ProductID = p.ProductID
GROUP BY o.OrderDate, c.Region, p.Category;
🧼 Power BI Data Modeling
Loaded SQL views into Power BI

Created relationships between dimension and fact tables

Built calculated columns and DAX measures for KPIs

📊 KPIs Created Using DAX
KPI	DAX Description
Total Sales	SUM(Orders[Sales])
Total Profit	SUM(Orders[Profit])
Average Order Value	DIVIDE([Total Sales], DISTINCTCOUNT(Orders[Order ID]))
Profit Margin	DIVIDE([Total Profit], [Total Sales])
Monthly Growth	CALCULATE([Total Sales], DATESMTD('Date'[Date]))

🎛️ Dashboard Features
Time-based visualizations – Line chart for sales trend (monthly/quarterly)

Category breakdown – Bar charts for top categories and subcategories

Customer segmentation – Pie chart for segments (Retail, Corporate, Home Office)

Geographical sales – Map showing region/country-level performance

Profitability overview – KPI cards for profit margin and AOV

Filters/Slicers – Region, Segment, Category, Date

🔍 Key Insights
💰 Sales peaked in Q4 of each year—indicating strong holiday performance.

🧑‍💼 Corporate segment generated the highest profit per customer.

📉 Certain subcategories like Binders and Tables showed negative profit margins.

🌎 Western and Eastern regions had the strongest consistent growth.

🛍️ Technology and Office Supplies were top-selling categories.

✅ Outcome
This project delivered a comprehensive, dynamic dashboard using SQL + Power BI, enabling stakeholders to:

Make informed product and regional investment decisions

Track sales health and profitability across time

Understand customer behavior and market segmentation

Improve operational strategy with interactive insights
