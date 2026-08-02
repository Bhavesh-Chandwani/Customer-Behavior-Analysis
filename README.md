# 🛍️ Customer Shopping Behavior Analysis
### End-to-End Customer Analytics Pipeline | Python • SQL Server • Power BI

<p align="left">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)

</p>

---

# 📌 Business Problem

Retail businesses collect large volumes of transactional and customer data but often struggle to convert it into actionable business intelligence.

The objective of this project is to build an end-to-end analytics solution that identifies customer purchasing patterns, evaluates the effectiveness of discount strategies, measures subscription impact, and segments customers based on buying behaviour.

The insights generated from this analysis help business stakeholders improve customer retention, optimize pricing strategies, and maximize long-term revenue growth.

---

# 🎯 Business Objectives

This project answers the following business questions:

- Which customer segments generate the highest revenue?
- Do discounts genuinely increase sales or unnecessarily reduce profit margins?
- How do subscription members differ from non-subscribers?
- Which product categories drive the majority of revenue?
- Which shipping methods contribute to higher order values?
- What customer characteristics influence repeat purchases?
- Which products consistently receive high customer ratings?
- How can marketing campaigns be better targeted using customer behaviour?

---

# 📊 Project Overview

This project demonstrates the complete analytics lifecycle—from raw data preparation to executive dashboard reporting.

The workflow includes:

- Data cleaning and preprocessing using Python
- Feature engineering for customer segmentation
- Loading cleaned data into SQL Server
- Business-driven analytical querying
- Interactive Power BI dashboard development
- Executive recommendations supported by data

Dataset Summary

| Metric | Value |
|---------|------:|
| Records | 3,900 |
| Features | 18 |
| Data Source | Retail Customer Transactions |
| Missing Values | Review Rating |
| Database | SQL Server |

---

# 🗂 Dataset Overview

The dataset contains information across multiple business dimensions.

### Customer Information

- Age
- Gender
- Location

### Transaction Information

- Product Category
- Purchased Item
- Purchase Amount
- Shipping Type
- Payment Method

### Customer Behaviour

- Discount Applied
- Promo Code
- Subscription Status
- Purchase Frequency
- Review Rating

---

# ⚙️ End-to-End Analytics Workflow

---

## 1️⃣ Data Cleaning & Feature Engineering (Python)

Python was used as the ETL layer to prepare production-ready data before loading it into SQL Server.

### Data Quality Improvements

- Removed redundant fields
- Standardized column names
- Fixed inconsistent formatting
- Validated data types
- Removed unnecessary attributes

### Missing Value Treatment

Only the **Review Rating** column contained missing values.

Instead of removing records or replacing values with the mean, **median imputation** was selected because review scores are susceptible to outliers. The median preserves the central tendency while minimizing the influence of extreme ratings.

### Feature Engineering

Additional business-friendly features were created to simplify downstream analysis.

| Feature | Business Purpose |
|----------|------------------|
| age_group | Customer demographic segmentation |
| purchase_frequency_days | Behavioural frequency analysis |
| Cleaned categorical fields | Improved SQL grouping and dashboard filtering |

### Data Loading

After preprocessing, the cleaned dataset was imported into SQL Server to support scalable SQL analysis and Power BI reporting.

---

## 2️⃣ Business Analytics using SQL

Rather than writing isolated SQL queries, the analysis was organized into business-focused analytical frameworks.

### Customer Segmentation

- Revenue by gender
- Revenue by age group
- New vs Returning vs Loyal customers
- High-value customer identification

Business Goal

Identify the customer groups contributing the highest revenue for targeted marketing.

---

### Revenue Optimization

- Revenue by product category
- Top-selling products
- Average purchase amount
- Highest revenue-generating segments

Business Goal

Determine which products and customer groups should receive increased marketing investment.

---

### Discount Effectiveness

- Discount usage analysis
- High-spending discount customers
- Discount-dependent products

Business Goal

Measure whether discounts increase revenue or unnecessarily reduce margins.

---

### Subscription Behaviour

- Subscribers vs non-subscribers
- Repeat purchase comparison
- Average order value comparison

Business Goal

Evaluate whether subscription programs improve customer retention and lifetime value.

---

### Product Performance

- Top-rated products
- Category-wise product rankings
- Customer review analysis

Business Goal

Identify products suitable for premium marketing campaigns.

---

### Logistics & Shipping Analysis

- Shipping type comparison
- Average purchase by shipping method

Business Goal

Understand whether faster delivery options encourage higher customer spending.

---

## 3️⃣ Interactive Power BI Dashboard

An executive-level dashboard was built to enable interactive exploration of customer behaviour.

### Dashboard Features

- Executive KPI Cards
- Revenue by Product Category
- Revenue by Age Group
- Subscription Distribution
- Customer Demographics
- Purchase Trends
- Interactive Filters & Slicers

### Key KPIs

| KPI | Value |
|------|------:|
| Total Customers | ~3.9K |
| Average Purchase | ~$59.76 |
| Customer Ratings | Interactive |
| Revenue by Category | Interactive |

---

# 💡 Key Business Insights

### Customer Behaviour

- Male customers generated slightly higher revenue than female customers.
- Young Adult customers represented one of the strongest revenue-driving segments.

### Subscription Analysis

- Subscription customers demonstrated stronger purchasing behaviour than non-members.

### Discount Analysis

- Certain products showed high dependence on discounts, suggesting potential margin erosion.

### Product Performance

- Highly rated products consistently generated stronger customer engagement.

### Shipping Analysis

- Express shipping customers exhibited a marginally higher average purchase value.

---

# 📈 Executive Recommendations

### 🎯 Strengthen Customer Retention

Expand subscription benefits and personalized loyalty rewards to improve repeat purchase rates.

**Suggested KPI**

- Customer Retention Rate
- Customer Lifetime Value (CLV)

---

### 💰 Optimize Discount Strategy

Replace blanket discounts with targeted promotions focused on high-value customer segments.

**Suggested KPI**

- Discount Redemption Rate
- Gross Margin
- Average Order Value

---

### 📦 Promote High-Performing Products

Increase marketing investment toward products with consistently high ratings and strong revenue performance.

**Suggested KPI**

- Product Conversion Rate
- Revenue per Product

---

### 🚚 Encourage Premium Shipping

Bundle express shipping incentives with premium products to increase average basket size.

**Suggested KPI**

- Average Order Value
- Express Shipping Adoption Rate

---

### 👥 Improve Customer Segmentation

Develop personalized campaigns using demographic and behavioural segments instead of generic promotions.

**Suggested KPI**

- Campaign Conversion Rate
- Repeat Purchase Rate

---

# 🛠 Technology Stack

| Tool | Purpose |
|------|---------|
| Python | Data Cleaning & Feature Engineering |
| Pandas | Data Manipulation |
| NumPy | Numerical Processing |
| SQL Server | Data Storage & Business Analysis |
| Power BI | Interactive Dashboard |
| Excel | Initial Data Exploration |

---

# 📂 Repository Structure

```text
customer_shopping_behavior_analysis/
├── 1. Business Problem Document.pdf
├── 2. Customer_Shopping_Behavior.csv
├── 3. Customer_Shopping_Behavior_Analysis.ipynb
├── 4. Customer_Shopping_Behavior_Analysis_SQL.sql
├── 5. Customer_Behavior_Dashboard.pbix
├── 6. Customer-Shopping-Behavior-Analysis.pptx
├── LICENSE
└── README.md
```


---

<details>

<summary><b>📌 Project Highlights</b></summary>

✔ End-to-End Analytics Project

✔ Python Data Cleaning & Feature Engineering

✔ SQL Business Analysis

✔ Interactive Power BI Dashboard

✔ Executive-Level Business Recommendations

✔ Customer Segmentation

✔ Revenue Optimization Analysis

✔ Discount Effectiveness Analysis

✔ Subscription Behaviour Analysis

✔ Retail Business Intelligence

</details>

---

# 📌 Conclusion

This project demonstrates the complete end-to-end data analytics lifecycle, transforming raw retail transaction data into actionable business insights that support strategic decision-making. By combining **Python** for data cleaning and feature engineering, **SQL Server** for business-driven analysis, and **Power BI** for interactive visualization, the project delivers a scalable analytics solution rather than isolated reports.

The analysis uncovered meaningful patterns in customer demographics, purchasing behaviour, subscription adoption, discount utilization, and product performance. These insights enable stakeholders to identify high-value customer segments, evaluate the effectiveness of promotional strategies, optimize product marketing, and improve customer retention initiatives.

Overall, the project illustrates how data can be leveraged to drive business outcomes through evidence-based decision-making. It highlights not only technical proficiency across the analytics stack but also the ability to translate data into strategic recommendations that can improve revenue growth, customer satisfaction, and long-term business performance.

---

## 📬 Connect With Me

<div align="center">

| Platform | Link |
|----------|------|
| 💼 LinkedIn | [Let's Connect](https://www.linkedin.com/in/bhavesh-chandwani) |
| 📧 Gmail | [bhavesh101714@gmail.com](mailto:bhavesh101714@gmail.com) |

</div>


---

# 👨‍💻 Author

### Bhavesh Chandwani

---

⭐ If you found this useful, feel free to connect and discuss data-driven strategies!
