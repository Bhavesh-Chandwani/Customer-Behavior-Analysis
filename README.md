# 🛍️ Customer Shopping Behavior Analysis

## 📌 Business Problem
A retail company wants to understand customer shopping behavior to improve sales, customer satisfaction, and long-term loyalty.

The key objective:
> How can customer data be leveraged to identify trends, improve engagement, and optimize marketing strategies?

📄 Detailed Problem Statement: [Business Problem Document](./docs/Business_Problem.pdf)

---

## 📊 Project Overview
This project analyzes **3,900 customer transactions** to uncover insights into:
- Customer spending patterns
- Product preferences
- Discount behavior
- Subscription impact
- Customer segmentation

---

## 📁 Dataset Summary
- Total Records: 3,900  
- Features: 18  
- Includes:
  - Demographics (Age, Gender, Location)
  - Purchase Data (Item, Category, Amount)
  - Behavior (Discounts, Reviews, Frequency)

- Missing Values:
  - Review Rating (handled using median imputation)

---

## ⚙️ Project Workflow

### 1️⃣ Data Cleaning & Feature Engineering (Python)
- Data cleaning and preprocessing using Pandas
- Handled missing values in `review_rating`
- Standardized column names
- Created new features:
  - `age_group`
  - `purchase_frequency_days`
- Removed redundant columns (`promo_code_used`)
- Loaded clean data into PostgreSQL

---

### 2️⃣ Data Analysis (SQL)
Performed business-driven analysis:

- Revenue by gender
- High-spending discount users
- Top-rated products
- Shipping type impact
- Subscription vs non-subscription analysis
- Discount-dependent products
- Customer segmentation (New, Returning, Loyal)
- Top products per category
- Repeat buyers vs subscriptions
- Revenue by age group

📌 Example Insight:
- Male customers generated higher revenue than female customers :contentReference[oaicite:0]{index=0}  
- Express shipping users spend slightly more on average :contentReference[oaicite:1]{index=1}  

---

### 3️⃣ Data Visualization (Power BI)
Developed an interactive dashboard with:
- KPI Cards (Total Customers, Avg Purchase, Ratings)
- Revenue breakdown by category & age group
- Subscription distribution
- Sales trends

📊 Dashboard highlights (Page 7):
- Total Customers: ~3.9K  
- Avg Purchase: ~$59.76 :contentReference[oaicite:2]{index=2}  

---

### 4️⃣ Business Insights & Recommendations

- 🎯 Promote subscription benefits to increase retention
- 🔁 Reward repeat customers to build loyalty
- 💸 Optimize discount strategy to protect margins
- ⭐ Focus marketing on top-rated products
- 📦 Target high-value segments (young adults & express shipping users)

---

## 🛠️ Tech Stack
- Python (Pandas, NumPy)
- Sql Server
- Power BI
- Excel

---

## 📂 Project Structure
Customer-Shopping-Behavior-Analysis/
│
├── 📁 docs/
│   ├── Business_Problem.pdf
│   └── Final_Report.pdf
│
├── 📁 data/
│   ├── raw_data.xlsx
│   └── cleaned_data.csv
│
├── 📁 python/
│   └── data_cleaning_and_feature_engineering.py
│
├── 📁 sql/
│   ├── schema.sql
│   └── analysis_queries.sql
│
├── 📁 powerbi/
│   └── dashboard.pbix
│
├── 📁 presentation/
│   └── final_presentation.pptx
│
├── README.md
└── requirements.txt
