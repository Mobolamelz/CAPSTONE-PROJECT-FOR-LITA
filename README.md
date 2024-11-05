# CAPSTONE-PROJECT-FOR-LITA
### PROJECT TITLE: ECOMMERCE SALES ANALYSIS
### TABLE OF CONTENT
[PROJECT OVERVIEW](#project-overview)
[DATA COLLECTED](#data-collected)
[OBJECTIVE OF THIS PROJECT](#objective-of-this-project)
[KEY METRICS](#key-metrics)
[TOOLS & METHODS USED](tools-&-methods-used)

![IMG_3677](https://github.com/user-attachments/assets/aec85330-3d62-4c30-a977-ba4d75605af6)
### PROJECT OVERVIEW
This project conducts an in-depth analysis of sales Performance for a Retail Store encompassing various Regions, product types, quantity sold, Order ID, Customer ID, Order date, and unit prices. The primary objective is to derive actionable insights on retrieving each product category's total sales, find the number of sales transactions in each region, find the highest-selling product by total sales value, calculate total revenue per product, calculate monthly sales totals for the current year, find the top 5 customers by total purchase amount, calculate the percentage of total sales contributed by each region, identify products with no sales in the last quarter. The goal is to produce an interactive Power BI dashboard that highlights these findings.

### DATA COLLECTED
Order ID
Customer ID
Product
Region
Order Date
Quantity
Unit price

### OBJECTIVE OF THIS PROJECT
This project aims to address the following analyses:

Total Sales Revenue: Calculate the total sales revenue by multiplying the quantity by price per unit to understand the overall sales performance.
Sales Trends Over Time: Use the date columns to analyze sales trends over different months, to identify peak and periods of low sales.
Region Performance Comparison: Compare sales across different regions to determine which locations are performing better. This can help identify top-performing branches and those that may need additional support.
Product Performance: Determine which products generate the most revenue or are sold most frequently using the product column. This can help in managing inventory and marketing efforts.
Top-Selling Products: Identify which products are sold most frequently (unit sold) to maintain adequate stock levels of materials.
Slow-Moving Inventory: Spot products with low sales that may require special promotions.
Branch-Level Stock Analysis: Understand which branches sell particular products faster and require frequent restocking of material.

### KEY METRICS
Total Revenue: This represents the overall income generated from sales, calculated as the sum of the revenue column.
Total Units Sold: This denotes the cumulative number of units sold, obtained by summing the units sold column.
Sales Growth Rate: This measures the percentage increase in sales revenue over a specific period (e.g., month-over-month, year-over-year).
Sales Performance Over Time: This involves analyzing trends over different time frames (daily, weekly, monthly) to identify peak sales periods.

### TOOLS & METHODS USED
- Microsoft Excel [Download here](https://microsoft.com)
  1. for data cleaning
  2. Data visualization
  3. Analysis of data
  4. Calculation
  
The pivot table effectively summarizes total sales by product, region, and month, highlighting key trends. Additionally, Excel formulas are used to calculate average sales per product and total revenue by region, providing valuable insights into sales performance.

![IMG_3675](https://github.com/user-attachments/assets/a73b607f-0598-4898-9cfa-9b9dacdd88cd)
![IMG_3676](https://github.com/user-attachments/assets/82fb16ef-79df-4924-838a-615d3ba84ace)

- STRUCTURES QUERY LANGUAGE TOOL-SQL
SQL (Structured Query Language) was used to extract and analyze data from the retail store dataset.
Retrieve Total Sales for Each Product Category Use SUM(sales_amount) to calculate total sales.
Group by category to get totals for each unique category. Find the Number of Sales Transactions in Each Region
Use COUNT(*) to count all transactions. Group by region for totals by region.
Find the Highest-Selling Product by Total Sales Value Calculate total sales per product. Use ORDER BY
Calculate Total Revenue per Product Use SUM(sales_amount) and group by product_name.
Calculate Monthly Sales Totals for the Current Year Filter by current year using WHERE. Extract month with EXTRACT(MONTH FROM sale_date) and group by month.
Find the Top 5 Customers by Total Purchase Amount Sum sales by customer_id. Order by total in descending orde
Calculate the Percentage of Total Sales Contributed by Each Region First, calculate regional sales using SUM. Then divide by total sales using a subquery.

- Github for porfolio building

  ### SKILLS
  
![IMG_3674](https://github.com/user-attachments/assets/4ecee25c-7b04-4d4b-be36-90300e25ce28)
![IMG_3673](https://github.com/user-attachments/assets/ae5d5594-fcab-4c87-b036-66147d71027a)

### DATA PREPARATION AND CLEANING WITH POWER BI
Data Import: Import data from Excel
Data Cleaning: Ensure unique records by removing duplicates, excluding irrelevant data through row filtering, and replacing or removing missing values if necessary.
Data Transformation: Ensure consistency by changing data types (e.g date, number, text) and improving data structuring by merging columns.
Data Normalization: Establish relationships between tables by defining primary and foreign keys

### DATA MODELLING

Establish Relationships: Enable efficient querying and accurate visualizations by creating relationships between tables (one-to-many, many-to-many).
Build a Date Table: Create a Date table with columns like Year, Quarter, Month, Day, etc., and relate it to the main data for time-based calculations (e.g., year-to-date, month-to-date).
Use Star Schema or Snowflake Schema: Connect a sales fact table to dimension tables (e.g. Sales table linked to Product, Region, and Date tables).

### CALCULATION AND ANALYSIS WITH DAX (Data Analysis Expressions)
Creating Measures and Calculated Columns:
Measures: Empower dynamic calculations based on report filters (e.g. total revenue, total quantity, and transaction).
Calculated Columns: Utilize static calculations that don’t change based on report filters (e.g. Revenue, Day of week, Period of day).
FORMULA USED:
Revenue Calculation: Revenue = SUM(Sales[Quantity]) * SUM(Sales[Price per Unit])
Total revenue: SUM('Sales Fact'[Revenue])
Total of quantity: SUM('Sales Fact'[Quantity])
Total orders: COUNT('Sales Fact'[Orders ID])

### DATA VISUALIZATION

Bar/Column Charts: Effectively compare quantities across categories.
Line Charts: Clearly display trends over time.
Donut Charts: Provide insights into percentage distribution.
Tree Map: Offer detailed data views.
Using Slicers and Filters: Enhance user-driven filtering by adding slicers (e.g., Region)

![IMG_3672](https://github.com/user-attachments/assets/c6fa1fb1-f4a8-4544-bda6-a3fa5183e9ed)

### RECOMMENDATION
Focus on Region-specific strategies The best-selling Region should have a meeting to speak on how they make large sales and what they do differently
Optimize operations by time of day More hands-on deck on Tuesday and Thursday since there’s a higher purchase at that time
Promote top-selling Product Put in more Revenue in the top-selling pizza to generate more Revenue
Revamp, Promote or Remove the least-selling pizza A sort of promo to the least product to boost the revenue and review the product.
Day-of-the-week promotions A promo for Monday and Friday to boost sales or have a discount during those days.

