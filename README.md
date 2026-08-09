# Customer_Shopping_Behavior_Analysis
End-to-end customer shopping behavior analysis using Python (EDA &amp; cleaning), SQL (business insights), and Power BI (interactive dashboard) on a 3,900+ record retail dataset covering demographics, purchases, discounts, and customer segmentation.
# Customer Shopping Behavior Analysis

## 📌 Overview
This project analyzes customer shopping behavior using a real-world retail dataset to uncover patterns in spending, product preferences, discounts, and customer loyalty. The workflow covers the complete data analytics lifecycle — from raw data to a polished presentation — using **Python**, **SQL**, and **Power BI**.

The goal is to identify actionable business insights such as which customer segments generate the most revenue, which products perform best, how discounts influence purchases, and how shipping preferences relate to spending.

## 📊 Dataset
- **Source:** Customer shopping behavior dataset (retail transactions)
- **Size:** ~3,900 customer records
- **Key fields:** Customer ID, Age, Gender, Item Purchased, Category, Purchase Amount, Location, Review Rating, Subscription Status, Shipping Type, Discount Applied, Previous Purchases, Payment Method, Frequency of Purchases

## 🧰 Tools & Technologies
- **Python (Pandas)** – data loading, cleaning, and exploratory data analysis (EDA)
- **SQL (PostgreSQL / MySQL / SQL Server / DBeaver)** – querying cleaned data for business insights
- **Power BI** – interactive dashboard for visualization
- **Gamma** – presentation (PPT) generation for stakeholder reporting

## 🔄 Project Workflow

### 1. Data Loading & Exploration
- Loaded the dataset into a Pandas DataFrame
- Reviewed structure, data types, and summary statistics using `.info()` and `.describe()`

### 2. Data Cleaning
- Identified and handled missing values (e.g., filled missing review ratings using category-wise median)
- Standardized column names (lowercase, underscores, renamed ambiguous fields)
- Removed redundant columns (e.g., `promo_code_used`, which duplicated `discount_applied`)

### 3. Feature Engineering
- Created an `age_group` column by binning customers into Young Adult, Adult, Middle-Age, and Senior segments
- Converted `frequency_of_purchases` (e.g., Weekly, Monthly) into a numeric `purchase_frequency_days` column for easier analysis

### 4. SQL Analysis
Cleaned data was queried using SQL to answer key business questions, including:
- Revenue by gender
- High-value customers who used discounts
- Top 5 highest-rated products
- Average spend by shipping type
- Revenue and spend by subscription status
- Discount rate by product category
- Customer segmentation (New / Returning / Loyal)
- Top 3 best-selling items per category
- Repeat buyer counts by subscription status
- Revenue by age group

### 5. Dashboard (Power BI)
An interactive Power BI dashboard was built to visualize:
- Revenue trends across demographics and categories
- Top-performing products
- Customer segmentation
- Discount and subscription impact on sales

### 6. Reporting & Presentation
- Key findings were compiled into a written report
- A summary presentation was created using **Gamma** to communicate insights to non-technical stakeholders

## 📈 Results & Key Insights
- Identified top revenue-generating customer segments by age and gender
- Highlighted best-performing products and categories
- Quantified the impact of discounts on purchase behavior
- Segmented customers into New, Returning, and Loyal groups based on purchase history
- Compared shipping preferences against average spend

## 🚀 How to Run This Project

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd customer-shopping-behavior-analysis
   ```

2. **Python EDA & Cleaning**
   - Install dependencies: `pip install pandas`
   - Open and run `Customer_Shopping_Behavior_Analysis.ipynb` in Jupyter Notebook

3. **SQL Analysis**
   - Load `customer_shopping_behavior.csv` into PostgreSQL, MySQL, or SQL Server (via DBeaver or your preferred client)
   - Run the queries in `customer_behavior.sql` against the imported table

4. **Power BI Dashboard**
   - Open `customer_behavior_dashboard.pbix` in Power BI Desktop
   - Refresh the data source if needed to explore the interactive visuals

## 📁 Repository Structure
```
├── customer_shopping_behavior.csv         # Raw dataset
├── Customer_Shopping_Behavior_Analysis.ipynb  # Data cleaning & EDA
├── customer_behavior.sql                  # SQL queries for insights
├── customer_behavior_dashboard.pbix       # Power BI dashboard
└── README.md                              # Project documentation
```

## 🙋 About
This project demonstrates a complete data analytics workflow — from raw data to business-ready insights — showcasing skills in Python, SQL, data visualization, and stakeholder communication.
