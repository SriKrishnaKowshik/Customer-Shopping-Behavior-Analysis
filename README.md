# 🛍️ Customer Shopping Behavior Analysis

An end-to-end **Data Analytics** project that analyzes customer shopping behavior using **Python, PostgreSQL, SQL, and Power BI**. The project focuses on customer segmentation, revenue analysis, purchasing trends, and interactive business intelligence dashboards.

## 📊 Project Overview

This project analyzes **3,900 retail transactions** to uncover valuable business insights, including:

* Customer spending patterns
* Product category performance
* Customer segmentation
* Subscription behavior
* Revenue trends across demographic groups

The final output is an interactive **Power BI dashboard** supported by data cleaning in Python and business analysis using SQL.

## 🛠️ Tech Stack

* **Python** (Pandas)
* **PostgreSQL**
* **SQL**
* **Power BI**
* **DAX**

## 📁 Dataset

| Feature        |              Value |
| -------------- | -----------------: |
| Total Records  |              3,900 |
| Total Columns  |                 18 |
| Missing Values | 37 (Review Rating) |

### Key Attributes

* Customer demographics
* Product category & items
* Purchase amount
* Shipping type
* Discounts
* Subscription status
* Previous purchases
* Review ratings

## ⚙️ Data Preparation

Data preprocessing was performed using **Python (Pandas)**.

* Imported and explored the dataset
* Handled missing values using median imputation
* Standardized column names (snake_case)
* Created **Age Group**
* Created **Customer Segment** (New, Returning, Loyal)
* Loaded cleaned data into PostgreSQL

## 🗄️ SQL Business Analysis

The following business questions were answered using SQL:

* Revenue by gender
* High-spending discount users
* Top-rated products
* Shipping type comparison
* Subscribers vs non-subscribers
* Discount-dependent products
* Customer segmentation
* Top 3 products per category
* Repeat buyers & subscriptions
* Revenue by age group

## 📈 Power BI Dashboard

### Dashboard Features

* KPI Cards (Total Customers, Average Purchase Amount, Average Review Rating)
* Subscription Distribution
* Revenue by Product Category
* Sales by Category
* Revenue by Age Group
* Sales by Age Group
* **Highest Revenue Products** (Top 5)
* Interactive slicers for Gender, Category, Subscription Status, and Shipping Type

> **Add your dashboard screenshot here:** `images/dashboard.png`

## 📐 DAX Measures

```DAX
Total Customers = DISTINCTCOUNT(CustomerID)

Average Purchase Amount = AVERAGE(PurchaseAmount)

Average Review Rating = AVERAGE(ReviewRating)

Total Revenue = SUM(PurchaseAmount)
```

## 💡 Key Insights

* Clothing generated the highest revenue.
* Young Adult customers contributed the largest share of sales.
* Loyal customers represented the largest customer segment.
* Express shipping showed a slightly higher average purchase value.
* The Top 5 products accounted for a significant portion of total revenue.

## 🚀 Business Recommendations

* Introduce customer loyalty rewards.
* Promote subscription benefits.
* Highlight highest revenue products in campaigns.
* Optimize discount strategies for profitability.
* Target high-value customer segments with personalized marketing.

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

This project demonstrates the complete **Data Analytics workflow**—from data cleaning and feature engineering to SQL-based business analysis, DAX measure creation, and interactive dashboard development using Power BI.

---

**Author:** Sri Krishna Kowshik
