# Power BI Dashboard

## Overview

The Power BI dashboard was developed to transform the banking database into an interactive analytical solution.

The dashboard provides insights into:

- Customer behavior
- Transaction activity
- Loan performance
- Financial performance
- Customer churn risk
- Banking products and services

The report consists of four analytical pages:

1. Executive Overview
2. Customer Analysis
3. Transaction Analysis
4. Loans Analysis

---

# Dashboard Pages

## 1. Executive Overview

The Executive Overview provides a high-level summary of the bank's financial and operational performance.

### Key KPIs

- Total Transaction Amount
- Total Transactions
- Total Customers
- Total Account Balance
- Average Transaction Amount

### Main Visualizations

- Transaction Amount by Transaction Type
- Transaction Amount by Branch
- Monthly Transaction Trend
- Transaction Amount by Channel

### Purpose

This page provides executives with a quick overview of the bank's overall performance and transaction activity.

---

## 2. Customer Analysis

The Customer Analysis page focuses on customer demographics, banking relationships, and customer risk.

### Key KPIs

- Total Customers
- New Customers
- Average Accounts per Customer
- Total Cards
- Total Loans

### Main Visualizations

- Customers by Occupation
- Card Type Distribution
- Customers by Age Group
- Customers with Highest Total Balance
- Customer Churn Risk

### Customer Churn Risk

Customers were categorized into different churn-risk levels based on their account activity and transaction behavior.

The analysis helps identify customers who may require retention actions.

### Purpose

This page helps the bank understand its customer base and identify potential retention opportunities.

---

## 3. Transaction Analysis

The Transaction Analysis page focuses on detailed transaction behavior.

### Key KPIs

- Deposit Amount
- Withdrawal Amount
- Transfer In Amount
- Transfer Out Amount
- Interest Credit Amount

Each KPI includes:

- Current value
- Year-over-Year (YoY) comparison
- Dynamic performance indicator
- Sparkline trend

### Main Visualizations

- Transfer In vs Transfer Out
- Deposit vs Withdrawal Activity
- Interest Credit Trend
- Transaction Type Contribution by Year

### Transaction Types

The analysis includes:

- Deposit
- Withdrawal
- Transfer In
- Transfer Out
- Interest Credit
- Fee Debit

### Purpose

This page helps analyze how money moves through the banking system and identify changes in transaction behavior over time.

---

## 4. Loans Analysis

The Loans Analysis page focuses on the bank's lending portfolio and repayment performance.

### Key KPIs

- Total Loans
- Total Loan Amount
- Outstanding Loan Balance
- Average Loan Amount
- Loan Repayment Rate

The KPIs include YoY comparisons and sparkline trends.

### Main Visualizations

- Loan Amount by Loan Type
- Loans by Status
- Loan Amount by Term
- Loan Amount Trend
- Loan Portfolio Analysis

### Loan Performance

The dashboard analyzes:

- Active loans
- Closed loans
- Defaulted loans
- Written-off loans
- Outstanding balances
- Repayment performance

### Purpose

This page helps evaluate the bank's lending portfolio, loan performance, and potential credit risks.

---

# Interactive Features

The dashboard supports interactive filtering and cross-filtering between visuals.

Users can explore the data by different dimensions such as:

- Date
- Customer
- Transaction Type
- Channel
- Branch
- Loan Type
- Loan Status
- Customer characteristics

---

# Time Intelligence

Time-based analysis was implemented using a dedicated Date Dimension.

The dashboard includes:

- Year-over-Year (YoY) analysis
- Previous Year calculations
- Monthly trends
- Sparkline trends

The Date Dimension is used to provide consistent time-based analysis across the dashboard.

---

# Data Model

The Power BI model follows a relational/star-schema-oriented structure.

Main entities include:

- Customers
- Accounts
- Transactions
- Cards
- Card Transactions
- Loans
- Loan Payments
- Branches
- Employees
- Support Tickets

The model connects transactional data with relevant dimensions to support analytical reporting.

---

# Tools Used

- Power BI
- DAX
- Power Query
- SQL Server
- Data Modeling
