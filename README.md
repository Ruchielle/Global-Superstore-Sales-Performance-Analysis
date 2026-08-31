## Global Superstore Sales Performance Analysis


## Table of Content 
 - [Projects Overview](#project-overview)
 - [Project Objective](#project-objective)
 - [Tools](#tools) 
 - [Data Workflow](#data-workflow) 
 - [Key Metrics](#key-metrics)
 - [Data Cleaning and Transformation](#data-cleaning-and-transformation)
 - [Exploratory Data Analysis](#eploratory-data-analysis)
 - [Key Insights and Visuals](#key-insights-and-visuals)
 - [Recommendations](#recommendation)
 - [Assumptions](#assumptions)
 - [Limitations](#limitations)
 - [Author](#author)


### Project Overview
 - This project solves a common business problem in a retail store understanding where a global company is making its money, which products and regions are driving growth, and where operational barriers are slowing things down. By analyzing four years of company sales records (from 2011 to 2014) for Global Superstore, this project turns raw, messy transactional data into a clear, interactive two page dashboard. This helps management see exactly which categories bring in the highest revenue, which regions perform best, and how shipping times impact operations so they can make smarter business decisions.


### Project Objectives
 
 - Import, clean, and prepare the Global Superstore dataset in Power BI using Power Query.  
 
 - Build calculated columns and measures to handle totals, profit margins, order rankings, and time based growth.  
 
 - Analyze sales and profit performance across different product categories, sub-categories, and geographic regions.  
 
 - Evaluate order sizes and shipping times to see how fulfillment speed affects operations.  
 
 - Design an interactive dashboard with filters for customer segments, product categories, and shipping modes.  


### Tools
 - Power Query
      - Used for cleaning the raw data, fixing data types, and standardizing text.  
 
 - DAX (Data Analysis Expressions)
      - Used for writing formulas, calculating totals, ranking products, and measuring time based growth.  
 
 - Power BI
      - Used for designing the visual layouts, and creating the interactive dashboard.  


### Exploratory Data Analysis
 
 - The analysis looked into several core questions:
 - Which product categories and sub categories bring in the most money and profit?
 - Which geographic regions have the highest sales volume?
 - How did yearly sales grow across categories from 2011 to 2014?
 - What is the breakdown of small, medium, and large orders?
 - How long does it take for orders to ship out to customers?

### Data Workflow

 - Source 
      - This Global Superstore retail dataset was downloaded from Kaggle dataset containing 51,289 rows and 21 columns, with key attributes including Order ID, Order Date, Ship Date, Ship Mode, Customer Name, Segment, State, Country, Region, Market, Product Name, Category, Sub-Category, Sales, Quantity, and Profit.

 - Ingestion
      - The raw data files were imported into Power query to check the row count, column count, and data structure before making any changes.  

 - Cleaning
      - Checked the overall row and column counts to ensure all data loaded correctly.  
      - Inspected important tracking fields like Order ID, Customer Name, and Product Name to check for duplicate entries or missing information.  
      - Cleaned up extra spaces in text fields and standardized values across regions, categories, and sub categories.  

 - Transformation
      - Converted date columns (Order Date and Ship Date) into proper date formats so time calculations would work.  
      - Converted financial and numerical values (Sales, Profit, and Quantity) into proper numbers.  
      - Created new calculated columns and measures to track order values, shipping delays, and customer sales totals.  
 
 - Analysis
      - Explored the data to answer key business questions regarding category revenue, regional performance, yearly sales trends, and order shipping durations.  

 - Output
      - A complete, two page interactive Power BI dashboard featuring summary cards, charts, maps, and filter slicers.  

### Key Metrics 
  
 - Total Sales 
      - Measures the total revenue generated from all sales in the dataset.
 
 - Total Profit 
      - Measures the total profit generated from the sales after accounting for the associated costs.
 
 - Average Sales Quantity 
      - Measures the average number of units sold per order or sales transaction.
 
 - Average Order Value (AOV) 
      - Measures the average sales revenue generated per order, showing how much customers typically spend in a single order.

 - Total Quantity Sold 
      - Measures the total number of units sold across all orders.
 
 - Distinct Customers 
      - Measures the number of unique customers who placed orders, counting each customer only once regardless of how many orders they made.
 
 - YTD Sales (Year to Date Sales) 
      - Measures the cumulative sales generated from the beginning of the current year up to the latest date in the selected context (such as January 1 to December 31 for a full year selection).
 
 - YoY Sales Growth (Year over Year Sales Growth) 
      - Measures the percentage increase or decrease in sales compared with the same period in the previous year (for example, comparing 2014 sales with corresponding 2013 sales).

 - Prior Year Sales 
      - Measures the sales generated during the corresponding period in the previous year to provide a baseline for comparing current performance.


### Data Cleaning and Transformation

 - Column Review
      - All 21 columns in the dataset were reviewed to make sure only relevant business fields were kept for the analysis.  

 - Data Type Corrections
      - Order Date and Ship Date were changed from text to proper date format.
      - Sales, Profit, and Quantity were changed to numeric formats so they could be added up and calculated properly.

 - Text Standardization
      - Extra spaces were removed from text entries, and names in the Region, Category, and Sub Category columns were cleaned up so they matched consistently.



### Key Insights and Visuals

 - Product and Category Performance
 
 - Sub-Category Sales
      - Technology brought in the highest total sales at $4.7M, followed by Furniture at $4.1M, and Office Supplies at $3.8M.  
 
 - Top-Selling Products
      - Apple Smartphones were the top-selling individual product at $87K in sales, followed by Cisco Smartphones at $76K.  
 
 - Profit Margin Contrast
      - Office Supplies had the highest profit margin at 5.86%, followed by Technology at 4.97%, and Furniture at 0.87%. This shows that a category with high sales doesn't always mean it keeps the most profit per dollar sold.  

 - Regional Sales Distribution
      - Regional Breakdown
      - The Central region generated $2.8M in sales, performing nearly double the South region ($1.6M), North region ($1.2M), and Oceania region ($1.1M). Central serves as the strongest performance standard.  

 - Sales Trends (2011–2014)
      - All three product categories grew steadily every single year from 2011 to 2014. Technology stayed in the lead and widened its sales gap over Furniture and Office Supplies by the end of 2014.  

 - Order Distribution by Sales 
      - Low: 33.04K orders (64.41%).  
      - Medium: 15.63K orders (30.48%).  
      - High: 2.62K orders (5.11%).  
      - Business Meaning: The business relies heavily on high volume sales coming from many smaller orders rather than a few massive purchases.  

 - Shipping Duration and Fulfillment
      - Shipping activity peaks heavily around Day 4 (58K units) and Day 5 (56K units). Very few orders ship out on Day 0 or Day 1, showing that fulfillment is concentrated around a 4 to 6 day window.  


### Recommendations
 - Speed Up Order Fulfillment
      - Because most orders ship around Day 4 and Day 5, the company can review its warehouse and processing steps to cut down on delays and ship orders faster.  
 - Protect High Margin Categories
      - While Technology brings in the most total revenue, Office Supplies gives the best profit return per dollar (5.86%). Focusing attention on these strong margins can improve overall financial return.  
 - Use Dashboard Filters for Deeper Reviews
      - Take advantage of the newly added filters for Customer Segments (Consumer, Corporate, Home Office), Product Categories, and Ship Modes during management meetings to answer specific questions on the fly.  

### Assumptions
 - Transactional records that loaded correctly without date errors were treated as valid retail sales events.
 - Orders were classified into High, Medium, and Low sales tiers based on set transaction thresholds.
 - Shipping delay was calculated simply by counting the number of calendar days between the order date and the shipping date.
 
### Limitations
 - The analysis is strictly limited to the four year timeframe (2011–2014) and the specific columns provided inside the Global Superstore dataset.  
 - External factors like local marketing campaigns, competitor pricing, and regional economic conditions were not part of the dataset.


### Author 