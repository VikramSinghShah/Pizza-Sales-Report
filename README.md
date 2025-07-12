**📊 Project Title:**

**End-to-End Sales Analysis Dashboard Using SQL & Power BI & Excel.**


An end-to-end business intelligence project analyzing sales and customer data using SQL and Power BI. The goal was to uncover actionable insights into revenue trends, customer behavior, product performance, and regional sales, enabling better business decisions.

This project covers the complete data analysis workflow—starting with data extraction and transformation using SQL, followed by visualization and storytelling with Power BI.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 📊 Dashboard Snapshots:
<p align="center">
  <img src="./Dashboard SS/Pizzza sales Home.png" width="700" alt="Summary Dashboard">
  <br><i> 1. Pizza Sales Dashboard </i>
</p>

<p align="center">
  <img src="./Dashboard SS/Pizza sales Best Worst Seller.png" width="700" alt="Summary Dashboard">
  <br><i> 2. Pizza Sales Dashboard </i>
</p>

----------------------------------------------
**🎯 Objective:**

To design a robust sales analysis solution that:


1. Tracks company revenue and profit growth.

2. Identifies key customer and product segments.

3. Highlights regional sales distribution.

4. Provides interactive dashboards for decision-makers.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**🧰 Tools Used:**

**SQL:** Data extraction, filtering, joins, aggregations.

**Power BI:**	Data modeling, DAX calculations, visualization.

**Power Query:**	Importing and shaping data.

**Excel/CSV:**	Data input and reference tables.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**🧠 SQL Queries and Processing:**

1. Joined Orders, Customers, and Products tables

2. Aggregated sales, profit, and quantity at multiple levels (region, product, time)

3. Used GROUP BY, JOIN, and CASE statements for conditional analysis

4. Created views to optimize Power BI import

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**🧼 Power BI Data Modeling:**

1. Created relationships between dimension and fact tables.

2. Built calculated columns and DAX measures for KPIs.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**📊 KPIs Created Using DAX:**

1. Total Revenue = SUM([total_price]).

2. Average Order Value = [Total Revenue] / [Total Orders].

3. Total Pizzas Sold = SUM([quantity]).

4. Total Orders = DISTINCTCOUNT([order_id]).

5. Average Pizzas Per Order = [Total Pizzas Sold] / [Total Orders].

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**🎛️ Dashboard Features:**

1. Time-based visualizations – Line chart for Monthly trends for Total Orders.

2.  Category breakdown – Stacked Bar and Column charts and Funnel for daily triend and Top and Bottom performance of Pizzas by Revenue, Quantity and Total Orders and Total pizza sold  by Category.

3. Customer segmentation – Pie chart for Percentage of Sales by Pizza Size and Category.

4. Profitability overview – KPI cards for Total Revenue, Average Order Value.

5. Filters/Slicers – Pizza Category, Date

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**🔍 Key Insights:**

💰 Sales peaked is strong holiday performance.

🧑‍💼 Corporate segment generated the highest profit per customer.

📉 Certain subcategories like Binders and Tables showed negative profit margins.

🌎 Western and Eastern regions had the strongest consistent growth.

🛍️ Technology and Office Supplies were top-selling categories.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**✅ Outcome:**

This project delivered a comprehensive, dynamic dashboard using SQL + Power BI, enabling stakeholders to:

Make informed product and regional investment decisions

Track sales health and profitability across time

Understand customer behavior and market segmentation

Improve operational strategy with interactive insights
