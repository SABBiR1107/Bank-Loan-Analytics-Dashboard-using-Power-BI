🏦 Bank Loan Analytics Dashboard (Power BI)

📊 Project Overview
This project presents a complete Bank Loan Analytics Dashboard built using Power BI.  
The goal is to analyze loan performance, identify risk patterns, and understand customer behavior through interactive visualizations.

🧹 Data Cleaning & Transformation
Removed duplicate records using `id`
Handled missing values (emp_length, emp_title)
Converted data types (date, numeric, percentage)
Cleaned text columns (Trim, Proper case)

🆕 New Columns Created
Term_Months
Emp_Length_Years
Loan Status Group (Good / Bad Loan)
Income Band
DTI Band
Interest Rate Band
Loan Amount Band
Term Category
Payment Status
Issue Year / Month

📐 Key DAX Measures
Total Applications
Total Funded Amount
Total Received Amount
Recovery Rate
Default Rate
Good Loan %
Bad Loan %

📊 Dashboard Pages
🔹 Executive Summary
KPI cards
Monthly trends
Loan distribution
🔹 Loan Risk Analysis
Grade vs default
DTI & interest impact
🔹 Customer Profile
Income distribution
Employment analysis
🔹 Recovery Analysis
Payment vs loan
Recovery rate

🎛 Slicers
Global:
Issue Date, Loan Status, Grade, Purpose, State, Term
Page-specific:
Risk: DTI, Interest Rate
Customer: Income, Employment
Recovery: Payment dates

📈 Key Insights
83% loans are fully paid
14% loans are charged off
Higher DTI & interest rate increase risk
Debt consolidation is the top purpose

🛠 Tools
Power BI
DAX
Power Query

📁 Project Structure
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
│   ├── risk_analysis.png
│   ├── customer_profile.png
│   └── recovery_analysis.png
│
└── README.md
```
👨‍💻 Author
Ahsanur Rahman Sabbir  
Data Science & AI Enthusiast
