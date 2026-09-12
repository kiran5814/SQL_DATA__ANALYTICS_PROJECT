# Adventure Works Sales Analytics Dashboard

## Project Overview

This project presents a comprehensive **Sales Analytics Solution** built using **SQL Server, Power BI, Power Query, and DAX**. The solution transforms raw sales data into actionable business insights through interactive dashboards focused on executive performance, customer behavior, and product profitability.

The project follows a complete analytics workflow:

- Data Warehousing using SQL Server
- Data Exploration and Business Analysis using SQL
- Data Modeling using a Star Schema
- Data Transformation using Power Query
- KPI Development using DAX
- Interactive Dashboard Development using Power BI

---

## Business Problem

Organizations generate large volumes of transactional sales data but often lack a centralized analytics solution to answer critical business questions such as:

- How are sales performing over time?
- Which products generate the highest revenue and profit?
- Which customer segments drive business growth?
- What countries contribute most to revenue?
- Which product lines are most profitable?
- What is the overall business profitability?

This project addresses these questions through a scalable analytics framework and executive-level reporting dashboards.

---

## Technology Stack

| Tool | Purpose |
|--------|----------|
| SQL Server | Data Warehouse & Analytics |
| T-SQL | Data Exploration & Reporting |
| Power Query | Data Cleaning & Transformation |
| Power BI | Dashboard Development |
| DAX | KPI Calculations |
| GitHub | Version Control & Portfolio |

---

## Data Model

The project uses a dimensional model following data warehousing best practices.

### Fact Table

```text
fact_sales
```

### Dimension Tables

```text
dim_customers
dim_products
```

### Model Type

```text
Star Schema
```

---

## SQL Analytics Implementation

The SQL layer consists of multiple analytical modules:

### Database Exploration
- Database metadata analysis
- Table exploration
- Data quality validation

### Dimension Exploration
- Customer analysis
- Product analysis
- Geographic analysis

### Date Analysis
- Historical date range exploration
- Time intelligence preparation

### KPI Development
- Total Sales
- Total Orders
- Total Quantity Sold
- Average Order Value
- Profit
- Profit Margin %

### Advanced Analytics
- Ranking Analysis
- Change Over Time Analysis
- Cumulative Analysis
- Product Performance Analysis
- Customer Segmentation
- Part-to-Whole Analysis

### Reporting Layer
- Customer Reporting Views
- Product Reporting Views

---

# Dashboard Pages

## 1. Executive Sales Analysis

### Purpose

Provides an executive overview of overall business performance.

### KPIs

- Total Sales: **$29M**
- Total Orders: **28K**
- Total Quantity Sold: **60K**
- Average Order Value: **$1.06K**

### Analysis Included

- Monthly Sales Trend
- Revenue by Product Line
- Revenue by Gender
- Geographic Sales Distribution

### Key Insights

- Road products generate the highest revenue.
- Monthly sales show steady growth across the analysis period.
- Sales distribution is balanced between male and female customers.
- North America contributes the largest share of revenue.

---

## 2. Customer Analysis Dashboard

### Purpose

Provides customer-centric insights to understand purchasing behavior and customer value.

### KPIs

- Total Customers: **18K**
- Sales per Customer: **$1.59K**
- Average Order Value: **$1.06K**
- Total Sales: **$29M**

### Analysis Included

- Sales by Country
- Average Sales per Customer
- Customer Distribution by Gender
- Top Customers by Revenue
- Sales Trend by Gender

### Key Insights

- United States and Australia generate the highest customer revenue.
- Average customer spending varies significantly across countries.
- Revenue contribution is balanced across genders.
- A small percentage of customers contribute disproportionately to revenue.

---

## 3. Product Performance Analysis

### Purpose

Evaluates product profitability and category performance.

### KPIs

- Total Products: **271**
- Total Product Cost: **$18M**
- Profit: **$12M**
- Profit Margin: **39.81%**
- Total Sales: **$29M**

### Analysis Included

- Sales vs Profit by Category
- Product Line Performance
- Subcategory Performance
- Top Products by Profit

### Key Insights

- Bikes account for the majority of company revenue and profit.
- Road products outperform other product lines.
- Touring Bikes dominate subcategory sales.
- A small number of products generate the highest profitability.

---

## Key DAX Measures

### Total Sales

```DAX
Total Sales =
SUM(fact_sales[sales_amount])
```

### Total Orders

```DAX
Total Orders =
DISTINCTCOUNT(fact_sales[order_number])
```

### Average Order Value

```DAX
Average Order Value =
DIVIDE([Total Sales],[Total Orders])
```

### Profit

```DAX
Profit =
[Total Sales] - [Total Product Cost]
```

### Profit Margin %

```DAX
Profit Margin % =
DIVIDE([Profit],[Total Sales])
```

### Sales Per Customer

```DAX
Sales Per Customer =
DIVIDE(
    [Total Sales],
    DISTINCTCOUNT(dim_customers[customer_key])
)
```

---

## Business Value Delivered

This solution enables stakeholders to:

- Monitor business performance through KPIs
- Identify top-performing products
- Analyze customer purchasing patterns
- Track profitability across categories
- Evaluate regional sales performance
- Support strategic decision-making with data-driven insights

---



## Skills Demonstrated

- SQL Server
- T-SQL
- Data Warehousing
- Dimensional Modeling
- Data Cleaning
- Power Query
- DAX
- Data Visualization
- Business Intelligence
- KPI Development
- Customer Analytics
- Product Analytics
- Time Series Analysis
- Dashboard Design
- Git & GitHub

---

## Author

**Kiran**

Aspiring Data Analyst | SQL | Power BI | Excel | Data Visualization

GitHub: https://github.com/kiran5814

---

## Resume Project Title

**Sales Analytics Dashboard & Data Warehouse Solution | SQL Server, Power BI, DAX, Power Query**
## About Me

🎓 Aspiring **Data Analyst** and **Data Engineer** with a passion for turning data into actionable insights.

📊 Currently preparing for a career in Data Analytics and Data Engineering by building hands-on projects and strengthening my technical skills.

💻 Skilled in:

* SQL
* Python
* Power BI
* Microsoft Excel
* Data Visualization
* Data Cleaning & Transformation

🚀 As a fresher, I am focused on learning industry best practices in analytics, database management, ETL processes, and data engineering.

🌱 Currently learning:

* Advanced SQL
* Python for Data Analysis
* Data Engineering Fundamentals
* Cloud & Big Data Concepts

📈 Interested in:

* Data Analytics
* Business Intelligence
* Data Engineering
* Data Visualization
* Database Management

📫 Open to internships, entry-level opportunities, and collaborations in the data domain.

*"Data is not just numbers; it tells a story waiting to be discovered."*
