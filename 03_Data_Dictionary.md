# Data Dictionary

## Customers

| Column | Description |
|---|---|
| customer_id | Unique identifier for each customer |
| name | Customer name |
| gender | Customer gender |
| date_of_birth | Customer date of birth |
| city | Customer city |
| state | Customer state |
| phone | Customer phone number |
| email | Customer email address |
| occupation | Customer occupation |
| annual_income | Customer annual income |
| join_date | Date the customer joined the bank |
| credit_score | Customer credit score |

---

## Accounts

| Column | Description |
|---|---|
| account_id | Unique identifier for each account |
| customer_id | Customer who owns the account |
| branch_id | Branch associated with the account |
| account_type | Type of bank account |
| balance | Current account balance |
| open_date | Account opening date |
| status | Current account status |

---

## Transactions

| Column | Description |
|---|---|
| transaction_id | Unique transaction identifier |
| account_id | Account associated with the transaction |
| txn_date | Transaction date |
| txn_type | Type of transaction |
| amount | Transaction amount |
| channel | Channel used for the transaction |
| merchant_category | Merchant or transaction category |

---

## Branches

| Column | Description |
|---|---|
| branch_id | Unique branch identifier |
| branch_name | Branch name |
| city | Branch city |
| state | Branch state |
| opened_date | Branch opening date |
| ifsc_code | Branch IFSC code |

---

## Employees

| Column | Description |
|---|---|
| employee_id | Unique employee identifier |
| name | Employee name |
| branch_id | Employee branch |
| role | Employee role |
| hire_date | Employee hiring date |
| salary | Employee salary |

---

## Cards

| Column | Description |
|---|---|
| card_id | Unique card identifier |
| customer_id | Customer associated with the card |
| account_id | Account associated with the card |
| card_type | Type of card |
| issue_date | Card issue date |
| expiry_date | Card expiration date |
| credit_limit | Card credit limit |
| status | Card status |

---

## Card Transactions

| Column | Description |
|---|---|
| card_txn_id | Unique card transaction identifier |
| card_id | Card associated with the transaction |
| txn_date | Card transaction date |
| merchant_category | Merchant category |
| amount | Transaction amount |
| is_fraud | Fraud indicator |

---

## Loans

| Column | Description |
|---|---|
| loan_id | Unique loan identifier |
| customer_id | Customer who owns the loan |
| branch_id | Branch associated with the loan |
| loan_type | Type of loan |
| loan_amount | Original loan amount |
| interest_rate | Loan interest rate |
| term_months | Loan term |
| start_date | Loan start date |
| status | Loan status |

---

## Loan Payments

| Column | Description |
|---|---|
| payment_id | Unique payment identifier |
| loan_id | Loan associated with the payment |
| payment_date | Payment date |
| amount_paid | Total payment amount |
| principal_component | Principal portion of payment |
| interest_component | Interest portion of payment |
| late_payment_flag | Indicates whether payment was late |

---

## Support Tickets

| Column | Description |
|---|---|
| ticket_id | Unique ticket identifier |
| customer_id | Customer who submitted the ticket |
| issue_type | Type of customer issue |
| date_opened | Ticket opening date |
| date_resolved | Ticket resolution date |
| status | Ticket status |
| satisfaction_score | Customer satisfaction score |
