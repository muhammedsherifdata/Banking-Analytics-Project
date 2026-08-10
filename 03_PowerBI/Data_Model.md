
# Power BI Data Model

## Model Overview

The Power BI data model was designed to connect the banking entities and support analytical reporting across customers, accounts, transactions, cards, loans, branches, and support operations.

## Main Tables

### Customers

Contains customer demographic and profile information.

### Accounts

Contains customer bank accounts and account balances.

### Transactions

Contains financial transaction activity.

### Cards

Contains customer card information.

### Card Transactions

Contains transactions performed using bank cards.

### Loans

Contains customer loan information and loan performance attributes.

### Loan Payments

Contains loan repayment transactions.

### Branches

Contains branch information and locations.

### Employees

Contains employee and branch information.

### Support Tickets

Contains customer support cases and satisfaction information.

---

## Key Relationships

Examples of important relationships include:

- Customers → Accounts
- Customers → Cards
- Accounts → Transactions
- Accounts → Branches
- Cards → Accounts
- Loans → Customers
- Loan Payments → Loans
- Employees → Branches
- Support Tickets → Customers

---

## Date Dimension

A dedicated `DimDate` table was created for time intelligence calculations.

The Date Dimension supports:

- YoY analysis
- Monthly trends
- Previous Year calculations
- Sparkline trends
