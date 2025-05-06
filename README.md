**About the Project:**

The main objective of the Project is to preprocess , analyze and visualize the Walmart sales data to uncover actionable insights. Performed extensive data cleaning and transformation using python libraries Pandas and Numpy. Used PostgreSQL for advanced querying and structured problem-solving techniques to address business challenges And developed an interactive Tableau dashboard to visualize performance patterns and strategic opportunities.

**About the Data:**

The project's data was obtained from the Kaggle Walmart Sales Dataset. It encompasses sales transactions from 100 Walmart branches situated in various cities. The data contains 11 columns and 10000 rows.

<img width="349" alt="image" src="https://github.com/user-attachments/assets/f89a279f-207b-4434-9b9f-73fbdc454920" />

**Project Steps:**

**1.	Tools Used: Visual Studio Code (VS Code), PostgreSQL and Tableau.**

•	Jupyter Notebook v2025.3.0, Python 3.13 <br/>
•	SQL Database: pgAdmin 4 <br/>
•	Python Libraries: pandas, numpy, sqlalchemy, psycopg2 <br/>
•	Tableau Public 2024.3.0 <br/>
•	Kaggle API Key (for data downloading) <br/>

**2.	Data Exploration:**
   
•	Conducted an initial data exploration to understand data distribution, column names, data types, and to identify potential issues like duplicates, NULL values <br/>
•	Used functions like .info(), .describe(), and .head() to get a quick overview of the data structure and statistics <br/>

**3.	 Data Wrangling:**

•	Identified and removed duplicate entries to avoid skewed results <br/>
•	Dropped rows and columns with missing values, which are insignificant <br/>
•	Ensured columns that have consistent data types (e.g., date as datetime, price as float) <br/>
•	Used .replace() to handle and format currency values for analysis <br/>
•	Converted the columns to lowercase to avoid inconsistencies <br/>
•	Checked for any remaining inconsistencies and verified the cleaned data <br/>

**4.	 Feature Engineering:**

•	Created new columns like total_amount for each transaction by multiplying unit_price by quantity and adding this as a new column <br/>
•	Extracted weekday from date column and hour from time column <br/>
•	Adding this calculated field will streamline further SQL analysis and aggregation tasks <br/>

**5.	Loaded Data into PostgreSQL:**

•	Connections: Connected to PostgreSQL using psycopg2,sqlalchemy and loaded the cleaned data into pgAdmin 4 database <br/>
•	Table Creation: Set up tables in PostgreSQL using Python SQLAlchemy to automate table creation and data insertion processes <br/>
•	Verification: Executed initial SQL queries to verify that the data was loaded accurately <br/>

**6.	SQL Analysis: Complex Queries and Business Problem Solving**

Some of the critical business problems, such as: <br/>
•	Revenue trends across branches and categories <br/>
•	Identifying best-selling product categories <br/>
•	Sales performance by time, city, and payment method <br/>
•	Analyzing peak sales periods and customer buying patterns <br/>
•	Profit margin analysis by branch and category <br/>

**7.	Tableau Dashboard:**

Developed Tableau Dashboard to visualize some of the Key performance Indicators (KPI’s) as, <br/>
•	The Profit vs Rating dual-axis chart in Tableau shows how profitability relates to customer satisfaction. An interactive parameter allows users to switch views by top N cities. This enables dynamic analysis to identify patterns between profit and rating across different cities <br/>
•	The heat map chart shows the busiest day of the week for each branch based on the number of transactions. This is done by fixed LOD function. An interactive parameter allows users to select the number of top branches to display <br/>
•	Sales trends over the years, segmented by product categories. It helps identify growth patterns and compare category performance across different time periods <br/>
•	Built using Tableau Public and packaged as a `.twbx` file for easy sharing <br/>


