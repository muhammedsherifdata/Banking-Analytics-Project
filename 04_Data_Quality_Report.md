# Data Quality Report

## Objective

A data quality assessment was performed after importing the banking dataset into SQL Server.

The purpose was to verify that the data could be safely used for analytical purposes before building business logic and reports.

---

# 1. Customer Data Validation

The Customers table contains approximately 60,000 customer records.

Validation checks included:

- NULL customer IDs
- Duplicate customer IDs
- Data type validation
- Basic value inspection

### Result

Customer identifiers were successfully validated.

---

# 2. Account Data Validation

The Accounts table was validated against the Customers and Branches tables.

Checks included:

- Valid customer references
- Valid branch references
- NULL account IDs
- Duplicate account IDs

### Result

The account relationships were validated successfully.

---

# 3. Loan Data Validation

The Loans table was checked against:

- Customers
- Branches

Loan payment records were also validated against the Loans table.

### Result

Loan-to-customer, loan-to-branch, and loan-to-payment relationships were validated.

---

# 4. Card Data Validation

Cards were validated against Customers and Accounts.

A business consistency check was performed to compare:

Cards.Customer_ID

with

Accounts.Customer_ID

for the associated Account_ID.

The following validation logic was used:

```sql
SELECT
    c.card_id,
    c.customer_id AS card_customer_id,
    a.account_id,
    a.customer_id AS account_customer_id
FROM cards c
JOIN accounts a
    ON c.account_id = a.account_id
WHERE c.customer_id <> a.customer_id;
