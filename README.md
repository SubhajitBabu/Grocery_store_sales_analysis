# grocery-store-sales-analysis
1. Project Title

Grocery Store Sales Data Analysis using MongoDB and Power BI

2. Project Overview

The Grocery Store Sales Data Analysis project focuses on analyzing grocery store transaction data to understand sales performance, customer behavior, product demand, discounts, store performance, and loyalty-program activity.

The project follows an end-to-end data analytics workflow. MongoDB was used for storing, cleaning, transforming, aggregating, and analyzing the transactional data. The processed data was then used in Power BI to develop an interactive dashboard containing KPIs and multiple visualizations.

The dashboard provides a centralized view of grocery store performance and allows users to analyze the business using filters such as transaction date, store, aisle, and product/item name.

3. Project Objectives

The main objectives of this project are:

To analyze grocery store transaction data.
To clean and prepare raw data using MongoDB.
To perform data transformation and aggregation.
To calculate important business KPIs.
To analyze sales across different stores and aisles.
To identify high-performing products.
To analyze product quantities sold.
To understand discount distribution.
To examine sales trends over time.
To analyze customer and loyalty-program activity.
To develop an interactive Power BI dashboard.
To generate meaningful business insights from transactional data.
4. Tools and Technologies
Tool	Purpose
MongoDB	Data storage, cleaning, transformation and analysis
MongoDB Compass	Database management and query execution
MongoDB Aggregation Pipeline	Aggregation and KPI calculations
Power BI	Interactive dashboard and data visualization
Power Query	Data preparation where required
DAX	KPI and analytical calculations in Power BI
5. Dataset Description

The dataset contains grocery store transaction-level information.

Main Fields
customer_id
store_name
transaction_date
aisle
product
quantity
unit_price
total_amount
discount_amount
final_amount
loyalty_points

These fields provide information about customers, products, stores, transactions, prices, discounts, and loyalty activity.

6. Data Structure

Each record represents a grocery store transaction.

For example, a transaction may contain:

Field	Description
Customer ID	Unique identifier of the customer
Store Name	Store where the transaction occurred
Transaction Date	Date of the transaction
Aisle	Product section/category
Product	Product purchased
Quantity	Number of units purchased
Unit Price	Price per unit
Total Amount	Sales amount before discount
Discount Amount	Discount provided
Final Amount	Amount after discount
Loyalty Points	Points earned by the customer
7. Data Cleaning

The raw data was first imported into MongoDB for data preparation.

The following cleaning activities were performed:

7.1 Missing Value Checking

The dataset was checked for missing or incomplete values in important fields such as:

Customer ID
Store Name
Product
Quantity
Unit Price
Transaction Date
Sales Amount

Missing or invalid values were handled appropriately before analysis.

7.2 Data Type Validation

Data types were checked to ensure that:

Quantity was treated as a numeric value.
Unit price was treated as a numeric value.
Sales amounts were numeric.
Discount amounts were numeric.
Transaction dates were treated as dates.
Customer IDs were consistently represented.
7.3 Text Standardization

Text fields such as store names, product names, and aisle names were reviewed to maintain consistency.

7.4 Duplicate and Invalid Records

The dataset was checked for duplicate or invalid transactions and unnecessary records were excluded from the analytical dataset where required.

7.5 Sales Validation

Sales-related values were checked to ensure that calculations such as total sales, discounts, and final sales were logically consistent.

8. Data Transformation

After cleaning, MongoDB was used to transform the data into an analysis-ready structure.

The transformation process included:

Selecting required fields.
Converting fields into appropriate data types.
Creating calculated values.
Grouping transactions.
Aggregating sales.
Aggregating quantities.
Counting transactions.
Counting unique customers.
Calculating discount totals.
Calculating loyalty-point metrics.

MongoDB aggregation pipelines were used to perform these operations efficiently.

9. Sales Calculations

The project uses several important sales calculations.

Gross Sales

Gross sales represent sales before discounts.

Formula:

Gross Sales = Sum of Total Amount

Discount

The total discount provided to customers is calculated as:

Total Discount = Sum of Discount Amount

Net Sales

Net sales represent the amount generated after discounts.

Formula:

Net Sales = Gross Sales - Total Discount

or, where available:

Net Sales = Sum of Final Amount

Average Order Value

Average Order Value measures the average amount generated per transaction.

Formula:

AOV = Net Sales / Total Transactions

10. KPI Analysis

The dashboard contains several important Key Performance Indicators.

10.1 Total Sales

Total Sales: 82.04K

This KPI represents the total net sales generated from the analyzed transactions.

10.2 Total Transactions

Total Transactions: approximately 2K

This represents the total number of transactions recorded in the dataset.

10.3 Total Customers

Total Customers: approximately 2K

This represents the number of customers included in the analyzed transaction data.

10.4 Total Quantity Sold

Total Quantity Sold: approximately 6K

This represents the total number of product units purchased.

10.5 Total Discount

Total Discount: 8.85K

This represents the total value of discounts provided to customers.

10.6 Average Order Value

Average Order Value: 41.43

This indicates the average sales value generated per transaction.

10.7 Gross Sales

Gross Sales: 90.89K

This represents the sales value before discounts.

10.8 Net Sales

Net Sales: 82.04K

This represents the final sales value after applying discounts.

10.9 Total Loyalty Points

Total Loyalty Points: approximately 505K

This represents the total loyalty points earned through customer transactions.

10.10 Average Loyalty Points

Average Loyalty Points: 15.49

This represents the average loyalty points generated per relevant transaction/customer record, based on the dashboard calculation.

Note: KPI values are shown in abbreviated form in the dashboard, such as K for thousands.

11. Power BI Dashboard

The cleaned and transformed data was connected to Power BI to create an interactive Grocery Store Sales Dashboard.

The dashboard provides a consolidated view of:

Sales
Transactions
Customers
Quantity
Discounts
Average Order Value
Gross Sales
Net Sales
Loyalty Points
Product performance
Store performance
Aisle performance
Sales trends
12. Dashboard Filters

The dashboard contains interactive filters that allow users to analyze the data from different perspectives.

Transaction Date

Users can filter the dashboard based on transaction dates to analyze sales for a specific period.

Store

The store filter allows users to compare the performance of different grocery stores.

Aisle

Users can select an aisle to analyze sales and product performance within a specific section.

Product / Item Name

The product filter allows users to focus on individual products and analyze their sales and quantity.

These filters make the dashboard interactive and allow users to perform customized analysis without modifying the underlying dataset.

13. Dashboard Visualizations
13.1 Sales by Store

The Sales by Store chart compares the total sales generated by different grocery stores.

This visualization helps identify:

Highest-performing stores
Lowest-performing stores
Differences in store-level revenue
Store contribution to total sales

It can help management identify stores that are performing strongly and those that may require additional attention.

13.2 Sales by Aisle

The Sales by Aisle visualization compares sales across different aisles.

It helps identify:

High-performing aisles
Low-performing aisles
Customer demand across product sections
Areas contributing significantly to revenue

This information can support product placement, inventory planning, and promotional strategies.

13.3 Sales by Product

The Sales by Product chart displays sales performance at the product level.

This allows the business to identify:

Best-selling products
Products generating higher revenue
Lower-performing products
Products that may require promotional support

Product-level analysis can help with inventory management and product strategy.

13.4 Sales Trend

The Sales Trend visualization shows sales activity over time.

The trend analysis helps identify:

Changes in sales volume
Periods of higher sales
Periods of lower sales
Sales fluctuations
Overall sales patterns

Time-based analysis can help businesses understand purchasing patterns and plan future sales strategies.

13.5 Quantity by Product

The Quantity by Product chart compares the number of units sold for different products.

This is useful because a product can have:

High sales value but lower quantity, or
Lower sales value but very high quantity.

Quantity analysis therefore provides a different perspective from revenue analysis and helps identify products with strong customer demand.

13.6 Discount Analysis

The Discount Analysis visualization compares the discounts associated with different stores.

It helps management understand:

Which stores provide higher discounts
Where promotional activity is concentrated
The relationship between discounting and sales
The overall impact of discounts on revenue

Discount analysis can help businesses evaluate whether promotional strategies are being used effectively.

14. Business Analysis

The dashboard provides several important analytical perspectives.

Store Performance

Sales by store allows management to compare different locations and identify high- and low-performing stores.

Product Performance

Product-level sales and quantity analysis helps identify products with strong customer demand.

Customer Activity

Customer and transaction KPIs provide an overview of customer participation and purchasing activity.

Discount Performance

Discount analysis helps determine the extent to which promotional discounts are being used.

Loyalty Performance

Loyalty points provide an indication of customer engagement with the loyalty program.

Sales Trends

The sales trend provides a time-based view of business performance and helps identify changes in transaction activity.

15. Business Insights

Based on the dashboard, the analysis provides the following types of insights:

Overall sales performance can be monitored through the Net Sales and Gross Sales KPIs.
The difference between Gross Sales and Net Sales highlights the financial impact of discounts.
Store-level analysis helps identify which stores contribute more significantly to overall sales.
Aisle-level analysis provides information about which product sections generate higher revenue.
Product-level sales analysis helps identify high-performing products.
Quantity analysis provides insight into product demand independently of revenue.
The Average Order Value provides an indication of the average customer transaction value.
Discount analysis helps evaluate promotional activity across stores.
Loyalty-point analysis provides information about customer engagement with the loyalty program.
The sales trend visualization makes it easier to identify changes and fluctuations in sales activity over time.
16. MongoDB Analysis Workflow

The MongoDB workflow can be summarized as:

Raw Dataset

↓

Import into MongoDB

↓

Data Validation

↓

Data Cleaning

↓

Data Type Conversion

↓

Data Transformation

↓

Aggregation Pipelines

↓

KPI Calculation

↓

Analysis-Ready Dataset

↓

Power BI

↓

Interactive Dashboard

17. Power BI Dashboard Workflow

The Power BI workflow consists of:

Step 1 – Data Connection

The prepared grocery store dataset was connected to Power BI.

Step 2 – Data Preparation

The imported data was reviewed and prepared for visualization.

Step 3 – KPI Creation

Measures were created for important metrics such as:

Total Sales
Transactions
Customers
Quantity
Discounts
AOV
Gross Sales
Net Sales
Loyalty Points
Step 4 – Visualization

Different charts were created to analyze:

Store sales
Aisle sales
Product sales
Sales trends
Product quantities
Discount distribution
Step 5 – Dashboard Design

The KPIs and charts were arranged into a single interactive dashboard.

Step 6 – Interactive Filtering

Slicers were added to allow users to dynamically filter the dashboard.

18. Dashboard Layout

The dashboard is organized into several sections.

Header

The top section contains the dashboard title:

Grocery Store Sales Dashboard

along with the tagline:

Better Food | Happier Customers | Stronger Communities

Filter Section

The filter section contains:

Transaction Date
Store
Aisle
Product/Item Name
KPI Section

The KPI cards provide a quick overview of:

Total Sales
Transactions
Customers
Quantity Sold
Discount
Average Order Value
Gross Sales
Net Sales
Loyalty Points
Average Loyalty Points
Analysis Section

The lower portion contains charts for:

Sales by Store
Sales by Aisle
Sales by Product
Sales Trend
Quantity by Product
Discount Analysis

This layout allows users to move from high-level KPIs to detailed analysis.

19. Key Performance Metrics
KPI	Purpose
Total Sales	Measures overall net sales
Transactions	Measures transaction volume
Customers	Measures customer count
Quantity Sold	Measures product units sold
Total Discount	Measures promotional discount value
AOV	Measures average transaction value
Gross Sales	Measures sales before discounts
Net Sales	Measures sales after discounts
Loyalty Points	Measures loyalty activity
Average Loyalty Points	Measures average loyalty engagement
20. Advantages of the Dashboard

The Power BI dashboard provides several benefits:

Centralized business reporting
Interactive analysis
Easy KPI monitoring
Store comparison
Product performance analysis
Sales trend analysis
Discount monitoring
Customer analysis
Loyalty-program analysis
Faster business decision-making

Instead of analyzing raw transaction records manually, users can obtain important information from a single interactive report.

21. Technical Skills Demonstrated

This project demonstrates practical knowledge of:

MongoDB
Database creation
Collection management
Data querying
Filtering
Projection
Aggregation
Grouping
Sorting
Data transformation
KPI calculation
Power BI
Data import
Data preparation
Data modeling
DAX measures
KPI cards
Slicers
Bar charts
Column charts
Line charts
Dashboard design
Interactive filtering
Business reporting
Data Analytics
Data cleaning
Exploratory analysis
KPI development
Trend analysis
Product analysis
Customer analysis
Sales analysis
Business insight generation
22. Project Challenges

Some of the key challenges involved in the project included:

Preparing raw transaction data for analysis.
Ensuring consistent data types.
Handling potentially missing or inconsistent values.
Creating meaningful KPI calculations.
Connecting database-level analysis with Power BI reporting.
Designing a dashboard that presents multiple business metrics without becoming difficult to interpret.
Selecting appropriate visualizations for different analytical requirements.
23. Project Outcome

The project successfully transformed raw grocery transaction data into an interactive business intelligence dashboard.

MongoDB was used to perform the backend data-processing and analytical tasks, while Power BI was used to present the results through interactive KPIs, charts, and filters.

The final dashboard provides management with a simple way to monitor sales, transactions, customers, products, quantity, discounts, and loyalty performance.


<img width="1090" height="606" alt="Screenshot 2026-09-20 171056" src="https://github.com/user-attachments/assets/8a99f0d7-d8b7-4ddb-933b-ea9c2e3fed5d" />



24. Conclusion

The Grocery Store Sales Data Analysis project demonstrates an end-to-end approach to data analytics using MongoDB and Power BI.

MongoDB was used for data storage, cleaning, transformation, aggregation, and KPI analysis, while Power BI was used to create an interactive business dashboard.

The dashboard enables users to analyze store performance, aisle sales, product performance, quantity sold, sales trends, discounts, customers, and loyalty activity. The use of interactive filters allows users to explore the data according to different dates, stores, aisles, and products.

Overall, the project demonstrates practical skills in database analysis, data cleaning, aggregation, KPI development, business intelligence, data visualization, and dashboard development, making it a strong portfolio project for a Data Analyst / Business Intelligence Analyst role.




