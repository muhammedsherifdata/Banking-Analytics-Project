# 🏦 Banking Analytics Project

## 📌 Project Overview

This project simulates a real-world banking analytics workflow using SQL Server and Power BI. The objective is not only to build dashboards, but also to demonstrate the complete analytical process followed by a Data Analyst in a production environment.

The project covers the full lifecycle of a data analytics solution, starting from raw CSV files, building a relational database, validating data quality, designing a semantic model, transforming data using Power Query, performing analytical calculations using DAX, and finally developing an interactive Power BI dashboard to support business decision-making.

---

## 🎯 Project Objectives

- Build a structured relational database in SQL Server.
- Validate data quality before analysis.
- Design a scalable analytical data model.
- Clean and transform data using Power Query.
- Develop business KPIs using DAX.
- Build an executive Power BI dashboard.
- Generate business insights and recommendations.

---

## 🛠 Tech Stack

- SQL Server
- SQL
- Power BI
- Power Query
- DAX
- Git & GitHub

---

## 📂 Project Structure

```

Banking-Analytics-Project

├── 01_Database
├── 02_SQL
├── 03_PowerBI
├── 04_Documentation
└── README.md

```

---

## 📊 Dataset

The dataset represents the operations of a retail bank including customers, accounts, transactions, cards, loans, branches, employees, and customer support activities.

Main entities:

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

---

## 🚧 Project Status

## 📈 Key Findings

Analysis of the full banking dataset (60K customers, 2M transactions, 65K cards, 22K loans) surfaced the following:

- **Churn risk:** 32.6% of customers (about 20K) fall in the high churn-risk group.
- **Loan quality:** about 10% of loans are defaulted or written off.
- **Loan repayment:** the overall loan repayment rate is 55.3%.

## 📊 Power BI Report

A 4-page interactive report built on a star-schema model with a Date dimension (active and inactive relationships, role-playing dimension). KPIs are built with DAX measures using time intelligence for customer growth, transaction performance, account balances and YoY/MoM trends.

<!-- Add your dashboard screenshots here, for example: -->
<!-- ![Dashboard page 1](03_PowerBI/screenshots/page1.png) -->

## 📚 Documentation

- `01_Project_Overview.md`: project scope and workflow
- `02_Business_Requirements.md`: business questions and KPI requirements
- `03_Data_Dictionary.md`: tables, columns and definitions
- `04_Data_Quality_Report.md`: validation and reconciliation checks and results
- `04_Documentation/`: supporting documents (add a link to your final report here)
