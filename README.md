# Superstore Sales & Business Performance Analytics using Excel

## Project Overview

This project focuses on performing end-to-end sales and profitability analysis on a retail Superstore dataset using Microsoft Excel. The objective was to transform raw transactional data into meaningful business insights through data cleaning, feature engineering, exploratory analysis, dashboard development, and business reporting.

---

# Project Lifecycle

## 1. Business Understanding

### Problem Statement

Retail businesses generate large volumes of transactional data, but raw data alone does not provide actionable insights.

The goal of this project was to:

* Analyze sales and profitability performance.
* Identify top-performing regions and categories.
* Understand customer segment contribution.
* Detect loss-making products and transactions.
* Build an executive dashboard for decision-making.

---

## 2. Data Collection

### Dataset

Superstore Retail Dataset

### Dataset Size

* Records: 9,986
* Original Columns: 21

### Original Features

* Row ID
* Order ID
* Order Date
* Ship Date
* Ship Mode
* Customer ID
* Customer Name
* Segment
* Country
* City
* State
* Postal Code
* Region
* Product ID
* Category
* Sub-Category
* Product Name
* Sales
* Quantity
* Discount
* Profit

---

## 3. Data Cleaning

The raw dataset was validated and prepared for analysis.

### Activities Performed

#### Missing Value Check

Verified all columns for null or missing values.

#### Duplicate Check

Checked for duplicate records to maintain data integrity.

#### Date Validation

Verified Order Date and Ship Date formats.

#### Data Type Validation

Validated numeric and categorical fields.

---

## 4. Feature Engineering

To enhance business analysis, four additional columns were created.

### Shipping Days

Measures delivery duration between order placement and shipment.

Formula:

```excel
=Ship Date - Order Date
```

Purpose:

* Analyze delivery efficiency.
* Support logistics performance evaluation.

---

### Profit Margin

Measures profitability percentage of each transaction.

Formula:

```excel
=(Profit/Sales)*100
```

Purpose:

* Identify profitable and low-margin orders.
* Compare profitability across products.

---

### Profit Flag

Classifies transactions as Profit or Loss.

Formula:

```excel
=IF(Profit>0,"Profit","Loss")
```

Purpose:

* Separate profitable and loss-making transactions.

---

### Revenue Band

Categorizes transactions into revenue groups.

Formula:

```excel
=IF(Sales<100,"Low",
IF(Sales<500,"Medium",
"High"))
```

Purpose:

* Segment sales transactions by revenue contribution.

---

## 5. Final Dataset Structure

### Total Columns: 25

1. Row ID
2. Order ID
3. Order Date
4. Ship Date
5. Ship Mode
6. Customer ID
7. Customer Name
8. Segment
9. Country
10. City
11. State
12. Postal Code
13. Region
14. Product ID
15. Category
16. Sub-Category
17. Product Name
18. Sales
19. Quantity
20. Discount
21. Profit
22. Shipping Days
23. Profit Margin
24. Profit Flag
25. Revenue Band

---

# 6. Exploratory Data Analysis

Multiple Pivot Tables were created to analyze business performance.

---

## Regional Performance Analysis

### Metrics

* Sum of Sales
* Sum of Profit

### Objective

Identify best and worst-performing regions.

### Result

* West Region generated highest sales.
* West Region generated highest profit.
* South Region generated lowest sales.

---

## Category Performance Analysis

### Metrics

* Sum of Sales
* Sum of Profit

### Objective

Evaluate category-level profitability.

### Result

* Technology was the highest-profit category.
* Furniture generated the lowest profit.

---

## Customer Segment Analysis

### Metrics

* Sum of Sales
* Sum of Profit

### Objective

Understand customer contribution.

### Result

* Consumer segment generated the highest revenue.
* Corporate segment ranked second.
* Home Office segment contributed the least revenue.

---

## Profit vs Loss Analysis

### Metrics

* Count of Orders

### Objective

Identify percentage of loss-making transactions.

### Result

* Profit Orders: 8,116
* Loss Orders: 1,870
* Loss Transaction Rate: 18.7%

---

## Product Analysis

### Top Revenue Generating Products

Analyzed products contributing highest sales revenue.

Result:

* Canon imageCLASS 2200 Advanced Copier emerged as the highest-selling product.

---

### Loss-Making Product Analysis

Analyzed products contributing negative profit.

Objective:

* Identify pricing issues.
* Evaluate discount impact.
* Support profitability improvement.

---

# 7. Dashboard Development

A dedicated executive dashboard worksheet was created.

---

## Dashboard Metrics

### Total Sales

$2.30 Million

### Total Profit

$286 Thousand

### Total Orders

9,986

### Overall Profit Margin

12.46%

---

## Dashboard Visualizations

### Sales & Profit by Region

Purpose:

Compare regional performance.

---

### Profit and Sales by Category

Purpose:

Identify profitable product categories.

---

### Sales by Segment

Purpose:

Understand customer segment contribution.

---

### Top 10 Products

Purpose:

Identify highest revenue-generating products.

---

### Top Loss-Making Products

Purpose:

Identify products negatively impacting profitability.

---

# 8. Business Insights

## Key Findings

### Regional Insights

* West region achieved highest sales and profit.
* South region recorded the lowest sales.

### Category Insights

* Technology generated strongest profitability.
* Furniture delivered lower profits despite significant sales.

### Customer Insights

* Consumer segment accounted for approximately 51% of total revenue.

### Product Insights

* Several products generated strong revenue but weak profitability.
* Multiple products consistently generated losses.

---

# 9. Recommendations

### Recommendation 1

Replicate successful sales strategies from the West region.

### Recommendation 2

Increase focus on Technology products.

### Recommendation 3

Review discounting policies for loss-making products.

### Recommendation 4

Improve Furniture category profitability.

### Recommendation 5

Monitor high-sales products with weak margins.

---

# 10. Project Outcome

Successfully transformed raw retail sales data into an executive business intelligence solution using Microsoft Excel.

The project enabled:

* Sales performance monitoring
* Profitability tracking
* Customer segment analysis
* Product performance evaluation
* Business decision support

---

# Tools Used

* Microsoft Excel
* Pivot Tables
* Pivot Charts
* Data Cleaning Techniques
* Feature Engineering
* Business Analysis
* Dashboard Development

---

# Skills Demonstrated

* Data Cleaning
* Data Transformation
* Exploratory Data Analysis (EDA)
* Business Intelligence
* Dashboard Development
* Data Visualization
* KPI Analysis
* Problem Solving
* Analytical Thinking
* Business Reporting
