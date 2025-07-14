# Retail Orders Analysis Project (SQL + Python)
## Project Overview
This project presents an end-to-end data analytics pipeline that leverages SQL and Python (Pandas) to derive meaningful insights from a retail sales dataset (orders.csv). It covers the complete lifecycle: data cleaning, transformation, feature engineering, database integration, and answering critical business questions using complex SQL queries and Python logic.
The analysis helps stakeholders identify high-performing products, seasonal trends, regional preferences, and revenue growth patterns.

## Technologies Used
| Tool/Language      | Purpose                             |
| ------------------ | ----------------------------------- |
| Python (Pandas)    | Data cleaning, transformation       |
| Jupyter Notebook   | Exploratory data analysis           |
| SQL (T-SQL Syntax) | Business queries on structured data |
| SQL Server / MySQL | Backend storage & querying          |
| VS Code            | Development environment             |

## Project Structure
   orders.csv            # Original dataset
   
   orders.ipynb          # Jupyter Notebook (Python Analysis)
   
   SQLQuery.sql          # SQL queries for business problem solving
   
   README.md             # Project documentation

## Dataset Description
The dataset includes transactional data from a retail store and contains the following columns:

**order_id, order_date, ship_mode, segment, country, city, state, postal_code, region**

**Product information: category, sub_category, product_id**

**Financial data: quantity, discount, sale_price, profit**


## Work Done
## Data Processing with Python (orders.ipynb)
## 1. Data Loading & Inspection
   
   Loaded data from orders.csv
   
   Inspected using .info(), .describe(), and .head()
   
   Checked for missing values, data types, and duplicates


## 2. Data Cleaning
   
   Converted date columns to proper datetime format
   
   Dropped duplicates and irrelevant columns (if any)
   
   Handled null values (if present)


## 3. Feature Engineering
   
   Extracted year, month, and day from order_date
   
   Created additional columns like revenue = quantity * sale_price
   

## 4. Export for SQL
   
   Final cleaned dataset was exported or inserted into an SQL database using SQLAlchemy
   

## Business Queries with SQL (SQLQuery.sql)
The SQL file contains several insightful business queries written using T-SQL syntax. Here's what each does:

Q1: Top 10 Highest Revenue Generating Products

Q2: Top 5 Best-Selling Products by Region

Q3: Month-over-Month Sales Comparison (2022 vs 2023)

Q4: Highest Revenue Month per Category

Q5: Sub-Category with Highest Growth (2022 vs 2023)

## How to Run the Project
### Step 1: Clone the Repository
  git clone https://github.com/your-username/your-repo-name.git

### Step 2: Create a Virtual Environment and Install Dependencies
  pip install pandas sqlalchemy

### Step 3: Run Jupyter Notebook
  jupyter notebook orders.ipynb

### Step 4: Load Data into SQL Server / MySQL
  Use the SQL schema in SQLQuery.sql to create the table.
  Use SQLAlchemy in the notebook to insert data from DataFrame.
  
### Step 5: Run SQL Queries
  Run the queries inside any SQL interface (SSMS, MySQL Workbench, DBeaver)

## Key Insights

  Certain products consistently generate high revenue across all regions.
  
  Sales trends show noticeable seasonal patterns, especially around peak shopping months.
  
  Some sub-categories experienced exponential growth, indicating shifting customer preferences.
  
  
## Future Enhancements

  Add dashboards using Power BI or Tableau.

  Include automated email reports using Python.
  
  Build an API to serve analytics as a service.


## License
  This project is licensed under the MIT License.

## Acknowledgments
- **Data Source**: Kaggle’s Retail Orders Dataset
