# 🛍️ Customer Shopping Behavior Analysis

An end-to-end **Data Analytics** project that analyzes customer shopping behavior using **Python, PostgreSQL, SQL, Power BI, and DAX**. The project uncovers customer purchasing patterns, revenue trends, product performance, and customer segmentation through an interactive business intelligence dashboard.

## 📊 Project Overview

This project analyzes **3,900 retail transactions** across multiple product categories to generate actionable business insights. The complete workflow includes data cleaning, feature engineering, SQL analysis, DAX measure creation, and dashboard development in Power BI.

### Objectives

* Analyze customer spending behavior
* Identify high-performing products
* Segment customers based on purchase history
* Compare subscription and non-subscription customers
* Build an interactive Power BI dashboard for decision-making

## 🛠️ Tech Stack

| Technology | Purpose                             |
| ---------- | ----------------------------------- |
| Python     | Data Cleaning & Feature Engineering |
| Pandas     | Data Manipulation                   |
| PostgreSQL | Database Management                 |
| SQL        | Business Analysis                   |
| Power BI   | Interactive Dashboard               |
| DAX        | KPI & Revenue Measures              |

## 📁 Dataset Information

| Feature        | Value |
| -------------- | ----: |
| Total Records  | 3,900 |
| Total Columns  |    18 |
| Missing Values |    37 |

### Dataset Features

* Customer demographics (Age, Gender, Location)
* Product information (Item, Category, Color, Size)
* Purchase details (Amount, Season, Shipping Type)
* Shopping behavior (Discounts, Subscription, Previous Purchases)
* Customer feedback (Review Rating)

## ⚙️ Data Preparation

The dataset was preprocessed using **Python (Pandas)**.

### Data Cleaning

* Imported and explored the dataset
* Handled missing values in `review_rating`
* Standardized column names using `snake_case`
* Removed redundant attributes
* Validated data consistency

### Feature Engineering

* Created **Age Group**
* Created **Customer Segment** (New, Returning, Loyal)
* Prepared the cleaned dataset for PostgreSQL

## 🗄️ SQL Business Analysis

The following business questions were solved using SQL:

* Revenue by Gender
* High-Spending Discount Users
* Top Rated Products
* Shipping Type Comparison
* Subscriber vs Non-Subscriber Revenue
* Discount-Dependent Products
* Customer Segmentation
* Top Products by Category
* Repeat Buyers & Subscriptions
* Revenue by Age Group

## 📈 Power BI Dashboard

### Dashboard Features

* KPI Cards (Total Customers, Average Purchase Amount, Average Review Rating)
* Revenue by Product Category
* Sales by Category
* Subscription Distribution
* Revenue by Age Group
* Sales by Age Group
* **Highest Revenue Products** (Top 5)
* Interactive Filters (Gender, Category, Subscription Status, Shipping Type)

> **Dashboard Preview:** Add a screenshot in the `images` folder and update the path below.

`![Dashboard](images/dashboard.png)`

## 📐 DAX Measures

```DAX
Total Customers =
COUNT('public customer'[customer_id])

Average Purchase Amount =
AVERAGE('public customer'[purchase_amount])

Average Review Rating =
AVERAGE('public customer'[review_rating])

Total Revenue =
SUM('public customer'[purchase_amount])
```

## 💡 Key Insights

* Clothing generated the highest overall revenue.
* Young Adult customers contributed the largest share of revenue.
* Loyal customers represented the largest customer segment.
* Express shipping customers showed a slightly higher average purchase value.
* The **Top 5 Products** contributed significantly to total revenue.

## 🚀 Business Recommendations

* Implement customer loyalty programs to increase retention.
* Promote subscription benefits to improve recurring purchases.
* Prioritize marketing for the highest revenue products.
* Optimize discount strategies to balance revenue and profitability.
* Target high-value customer age groups with personalized campaigns.

## 📂 Project Structure

```text
Customer-Shopping-Behavior-Analysis/
│
├── data/
│   └── customer_shopping.csv
│
├── python/
│   └── data_cleaning.ipynb
│
├── sql/
│   └── business_queries.sql
│
├── powerbi/
│   └── customer_shopping_analysis.pbix
│
├── images/
│   └── dashboard.png
│
└── README.md
```

## 🎯 Project Outcome

This project demonstrates a complete **Data Analytics workflow** by combining Python for data preprocessing, PostgreSQL and SQL for business analysis, DAX for KPI calculations, and Power BI for interactive dashboard development. The final dashboard enables stakeholders to explore customer behavior and make data-driven business decisions.

## 👨‍💻 Author

**Sri Krishna Kowshik Nalliboina**

M.Sc. Computer Science | Data Analytics & Power BI Portfolio Project
