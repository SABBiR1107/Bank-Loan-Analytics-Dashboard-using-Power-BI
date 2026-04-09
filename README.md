
# 🏦 Bank Loan Analytics Dashboard (Power BI)

## 📌 Project Overview

This project presents a **comprehensive Bank Loan Analytics Dashboard** built using Power BI.
It provides deep insights into loan performance, customer behavior, and financial risk to support **data-driven decision-making**.

### 🎯 Objectives

* Analyze overall loan performance
* Identify high-risk loans and default patterns
* Understand customer financial behavior
* Monitor repayment and recovery trends

---

## 📁 Project Structure

```
Bank-Loan-Analytics/
│
├── dataset/
│   └── financial_loan.csv
│
├── dashboard/
│   └── Bank_Loan_Dashboard.pbix
│
├── images/
│   ├── executive_summary.png
│   ├── loan_risk_analysis.png
│   ├── customer_profile.png
│   └── recovery_analysis.png
│
└── README.md
```

---

## 📊 Dataset Description

The dataset contains detailed **loan-level financial and customer data**.

### 🔹 Basic Information

* id
* member_id
* address_state
* application_type

### 🔹 Customer Information

* emp_length
* emp_title
* home_ownership
* annual_income

### 🔹 Loan Details

* loan_amount
* term
* int_rate
* installment
* purpose
* grade
* sub_grade

### 🔹 Financial Metrics

* dti (Debt-to-Income Ratio)
* total_acc

### 🔹 Payment Information

* loan_status
* total_payment
* issue_date
* last_payment_date
* next_payment_date
* last_credit_pull_date

---

## 🧹 Data Cleaning & Preparation

Data transformation was performed using **Power Query**:

* ✅ Removed duplicate records (`id`)
* ✅ Handled missing values:

  * `emp_length` → "Unknown"
  * `emp_title` → "Unknown"
* ✅ Converted data types:

  * Dates → Date format
  * Numeric → Whole/Decimal
* ✅ Cleaned text:

  * Trimmed spaces
  * Standardized format (Proper Case)

---

## 🆕 Feature Engineering (New Columns)

Created additional columns to enhance analysis:

* Term_Months
* Emp_Length_Years
* Loan Status Group *(Good Loan / Bad Loan)*
* Income Band
* DTI Band
* Interest Rate Band
* Loan Amount Band
* Term Category *(Short / Long)*
* Payment Status *(Recovered / Not Recovered)*
* Issue Year, Month, Year-Month

---

## 🧠 Data Modeling

* ⭐ Fact Table: **Loans**
* ⭐ Dimension Table: **DimDate**
* 🔗 Relationship: `issue_date` → Date Table
* ⏱ Enabled time-based analysis

---

## 📐 Key DAX Measures

### 📊 KPIs

* Total Applications
* Total Funded Amount
* Total Received Amount
* Recovery Rate
* Default Rate

### 📉 Risk Metrics

* Good Loan %
* Bad Loan %
* Charged-Off Amount

### 💰 Financial Metrics

* Outstanding Amount
* Average Loan Amount
* Average Installment

---

## 📊 Dashboard Pages

### 🔹 1. Executive Summary

* KPI Cards
* Loan Status Distribution
* Monthly Trends
* State & Purpose Analysis

### 🔹 2. Loan Quality & Risk

* Grade vs Loan Status
* Default Rate Analysis
* DTI & Interest Rate Impact

### 🔹 3. Customer Profile

* Income Distribution
* Employment Analysis
* Customer Segmentation

### 🔹 4. Recovery Analysis

* Payment vs Loan
* Recovery Rate
* Outstanding Loans

---

## 🎛 Filters & Slicers

### 🌍 Global Slicers

* Issue Date
* Loan Status
* Grade
* Purpose
* Address State
* Term

### 📌 Page-Specific Slicers

* **Risk Page** → DTI Band, Interest Rate Band
* **Customer Page** → Income Band, Employment Length
* **Recovery Page** → Payment Dates

---

## 📈 Key Insights

* 📌 ~83% of loans are fully paid
* ⚠️ ~14% of loans are charged off
* 📉 High DTI & interest rates increase default risk
* 💳 Debt consolidation is the most common loan purpose
* ⏳ 36-month loans are the most frequent

---

## 🎨 Dashboard Design

* Clean & modern UI
* Consistent color scheme:

  * 🟢 Green → Good Loans
  * 🔴 Red → Bad Loans
  * 🔵 Blue → Neutral Metrics
* Interactive and user-friendly filters

---

## 🛠 Tools & Technologies

* Power BI
* DAX
* Power Query

---

## 🚀 How to Use

1. Open `Bank_Loan_Dashboard.pbix` in Power BI Desktop
2. Load the dataset (`financial_loan.csv`)
3. Interact with slicers and filters
4. Explore insights across all dashboard pages

---

## 👨‍💻 Author

**Ahsanur Rahman Sabbir**
📊 Data Science | 🤖 AI & ML Enthusiast

---

## ⭐ Support

If you found this project useful:

👉 Give it a ⭐ on GitHub
👉 Share your feedback
👉 Connect on LinkedIn

---
