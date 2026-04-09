🏦 Bank Loan Analytics Dashboard (Power BI)
📁 Project Structure
```
Bank-Loan-Analytics/
│
├── dataset/
│   └── financial\_loan.csv
│
├── dashboard/
│   └── Bank\_Loan\_Dashboard.pbix
│
├── images/
│   ├── executive\_summary.png
│   ├── loan\_risk\_analysis.png
│   ├── customer\_profile.png
│   └── recovery\_analysis.png
│
└── README.md
```
---
📊 Project Overview
This project presents a complete Bank Loan Analytics Dashboard built using Power BI.
The main goal of this project is to:
Analyze loan performance
Identify high-risk loans
Understand customer behavior
Monitor payment and recovery trends
---
📁 Dataset Description
The dataset includes loan-level data with the following features:
🔹 Basic Information
id
member_id
address_state
application_type
🔹 Customer Information
emp_length
emp_title
home_ownership
annual_income
🔹 Loan Details
loan_amount
term
int_rate
installment
purpose
grade
sub_grade
🔹 Financial Metrics
dti
total_acc
🔹 Payment Information
loan_status
total_payment
issue_date
last_payment_date
next_payment_date
last_credit_pull_date
---
🧹 Data Cleaning & Preparation
Performed using Power Query:
Removed duplicate rows using `id`
Handled missing values:
emp_length → replaced with "Unknown"
emp_title → replaced with "Unknown"
Converted data types:
Dates → Date format
Numbers → Decimal/Whole number
Cleaned text (trim, proper case)
---
🆕 New Columns Created
The following new columns were created for better analysis:
Term_Months (converted from text to numeric)
Emp_Length_Years (numeric employment length)
Loan Status Group (Good Loan / Bad Loan)
Income Band (grouped income levels)
DTI Band (grouped debt-to-income ratio)
Interest Rate Band
Loan Amount Band
Term Category (Short / Long Term)
Payment Status (Recovered / Not Recovered)
Issue Year, Month, Year-Month
---
🧠 Data Modeling
Fact Table: Loans
Created Date Table (DimDate)
Linked using issue_date
Enabled time-based analysis
---
📐 Key DAX Measures
📊 KPIs
Total Applications
Total Funded Amount
Total Received Amount
Recovery Rate
Default Rate
📉 Risk Metrics
Good Loan %
Bad Loan %
Charged Off Amount
💰 Financial Metrics
Outstanding Amount
Average Loan Amount
Average Installment
---
📊 Dashboard Pages
🔹 1. Executive Summary
KPI Cards
Loan Status Distribution
Monthly Trends
State & Purpose Analysis
🔹 2. Loan Quality & Risk
Grade vs Loan Status
Default Rate Analysis
DTI & Interest Rate Impact
🔹 3. Customer Profile
Income Distribution
Employment Analysis
Customer Segmentation
🔹 4. Recovery Analysis
Payment vs Loan
Recovery Rate
Outstanding Loans
---
🎛 Slicers
Global Slicers:
Issue Date
Loan Status
Grade
Purpose
Address State
Term
Page-Specific:
Risk → DTI Band, Interest Rate Band
Customer → Income Band, Employment Length
Recovery → Payment Dates
---
📈 Key Insights
~83% loans are fully paid
~14% loans are charged off
High DTI and interest rate increase risk
Debt consolidation is the top loan purpose
36-month loans are most common
---
🎨 Dashboard Design
Clean and professional layout
Consistent color scheme:
Green → Good Loans
Red → Bad Loans
Blue → Neutral
Interactive slicers and filters
---
🛠 Tools Used
Power BI
DAX
Power Query
---
👨‍💻 Author
Ahsanur Rahman Sabbir  
Data Science | AI & ML Enthusiast
---
⭐ If you like this project, give it a star!
