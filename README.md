
🛍️ Customer Shopping Behavior Analysis

📄 Overview:
This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories.
The goal is to uncover insights into spending patterns, customer segments, product preferences, and subscription trends to guide strategic business decisions.

📊 Dataset Summary
Rows: 3,900
Columns: 18
Key Features:
Customer demographics: Age, Gender, Location, Subscription Status
Purchase details: Item Purchased, Category, Purchase Amount, Season, Size, Color
Shopping behavior: Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type
Missing Data: 37 missing values in the Review Rating column

🧰 Tools & Technologies
Task	Tool
Data Loading & Cleaning	Python (Jupyter Notebook, Pandas)
Database & Queries	MySQL
Visualization	Power BI


⚙️ Project Steps
1. Data Preparation (Python)
Imported dataset using pandas
Checked structure with df.info() and summary stats with df.describe()
Handled missing values in Review Rating using median values by category
Renamed columns to snake_case for better readability
Created new features:
age_group — grouped customer ages
purchase_frequency_days — derived from purchase timestamps
Removed redundant columns (promo_code_used) after consistency checks
Loaded cleaned data into MySQL for structured analysis


2. SQL Analysis (MySQL)
Performed SQL queries to answer business questions:
Revenue by Gender – Compare revenue between male and female customers
High-Spending Discount Users – Identify discount users spending above the average
Top 5 Products by Rating – Find highest-rated products
Shipping Type Comparison – Compare average spend for Standard vs Express shipping
Subscribers vs Non-Subscribers – Analyze spending and total revenue
Discount-Dependent Products – Find products most purchased on discount
Customer Segmentation – Classify customers as New, Returning, or Loyal
Top 3 Products per Category – Identify most purchased items in each category
Repeat Buyers & Subscriptions – Check if frequent buyers are more likely to subscribe
Revenue by Age Group – Evaluate contribution by different age groups


3. Power BI Dashboard
Created an interactive Power BI dashboard with:
KPIs: Total Revenue, Avg Purchase Value, Discount Usage Rate
Visuals: Bar charts, line charts, and pie charts for key metrics
Filters for gender, age group, category, and season
Insights on customer segments and top-performing products


📈 Results & Insights
Loyal and subscribed customers drive a major share of total revenue
Discounted purchases still generate strong sales volume
Express shipping customers show higher average spending
Younger age groups show higher purchase frequency but lower average ticket size



