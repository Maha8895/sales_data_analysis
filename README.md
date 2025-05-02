**About the Project:**

The main objective of the Project is to preprocess , analyze and visualize the Walmart sales data to uncover actionable insights. Performed extensive data cleaning and transformation using python libraries Pandas and Numpy. Used PostgreSQL for advanced querying and structured problem-solving techniques to address business challenges And developed an interactive Tableau dashboard to visualize performance patterns and strategic opportunities.

**About the Data:**

The project's data was obtained from the Kaggle Walmart Sales Dataset . It encompasses sales transactions from 100 Walmart branches situated in various cities. The data contains 11 columns and 10000 rows.
Column	Description	Data Type
invoice_id	Invoice of the sales made	Int64
branch	Branch at which the transactions were made	object
city	The location of the branch	object
category	The type of the product	object
unit_price	The price of each product	object
quantity	No.of.products sold	object
date	The date on which the purchase was made	object
time	The time at which the purchase was made	object
payment_method	Mode of payment	object
rating	Rating given by customers	Float64
Profit_margin	Profit made on sale	Float64

**Project Steps:**

**1.	Tools Used: Visual Studio Code (VS Code), PostgreSQL and Tableau.**

•	Jupyter Notebook v2025.3.0, Python 3.13
•	SQL Database: pgAdmin 4
•	Python Libraries: pandas, numpy, sqlalchemy, psycopg2
•	Tableau Public 2024.3.0
•	Kaggle API Key (for data downloading)

**2.	Data Exploration:**
   
•	Conducted an initial data exploration to understand data distribution, column names, data types, and to identify potential issues like duplicates, NULL values.
•	Used functions like .info(), .describe(), and .head() to get a quick overview of the data structure and statistics.
4.	 Data Wrangling:
•	Identified and removed duplicate entries to avoid skewed results.
•	Dropped rows and columns with missing values, which are insignificant.
•	Ensured columns that have consistent data types (e.g., date as datetime, price as float).
•	Used .replace() to handle and format currency values for analysis.
•	Converted the columns to lowercase to avoid inconsistencies.
•	Checked for any remaining inconsistencies and verified the cleaned data.
5.	 Feature Engineering:
•	Created new columns like total_amount for each transaction by multiplying unit_price by quantity and adding this as a new column.
•	Extracted weekday from date column and hour from time column.
•	Adding this calculated field will streamline further SQL analysis and aggregation tasks.
6.	Loaded Data into PostgreSQL:
•	Connections: Connected to PostgreSQL using psycopg2,sqlalchemy and loaded the cleaned data into pgAdmin 4 database.
•	Table Creation: Set up tables in PostgreSQL using Python SQLAlchemy to automate table creation and data insertion processes..
•	Verification: Executed initial SQL queries to verify that the data was loaded accurately.
7.	SQL Analysis: Complex Queries and Business Problem Solving
Some of the critical business problems, such as:
•	Revenue trends across branches and categories.
•	Identifying best-selling product categories.
•	Sales performance by time, city, and payment method.
•	Analyzing peak sales periods and customer buying patterns.
•	Profit margin analysis by branch and category.

8.	Tableau Dashboard:

Developed Tableau Dashboard to visualize some of the Key performance Indicators (KPI’s) as,
•	The Profit vs Rating dual-axis chart in Tableau shows how profitability relates to customer satisfaction. An interactive parameter allows users to switch views by top N cities. This enables dynamic analysis to identify patterns between profit and rating across different cities. 
•	The heat map chart shows the busiest day of the week for each branch based on the number of transactions. This is done by fixed LOD function. An interactive parameter allows users to select the number of top branches to display.
•	Sales trends over the years, segmented by product categories. It helps identify growth patterns and compare category performance across different time periods.
•	Built using Tableau Public and packaged as a `.twbx` file for easy sharing.


![image](https://github.com/user-attachments/assets/606b5408-1fee-4f10-963f-de8cf5f380b3)
