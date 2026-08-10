# Business Requirements

## Objective

The following business requirements define the analytical questions that the project aims to answer.

Each requirement will be translated into:

Business Question
→ Business Logic
→ SQL Analysis
→ Validation
→ Business Insight
→ Recommendation
→ Visualization

---

# Phase 1 — Customer Insights & Retention

## BR-01 — High-Value Customers

### Business Question

Identify the top 10% of customers based on their financial relationship with the bank.

### Business Objective

Support premium customer targeting, personalized offers, and customer relationship management.

### Key Metrics

- Annual Income
- Total Account Balance
- Customer Value Score
- Customer Rank

---

## BR-02 — Customer Retention & Churn Risk

### Business Question

Calculate the current customer churn rate.

For analytical purposes, a customer will be considered potentially churned if:

- Their accounts are inactive, or
- They have not performed a transaction during the last six months.

### Business Objective

Identify customers who may require retention campaigns.

### Key Metrics

- Total Customers
- Active Customers
- Potentially Churned Customers
- Churn Rate

---

## BR-03 — Customer Demographic Segmentation

### Business Question

Analyze the relationship between customer occupation, preferred card type, and average loan amount.

### Business Objective

Understand customer segments and identify differences in product adoption and borrowing behavior.

### Key Metrics

- Customer Count
- Card Type Distribution
- Average Loan Amount
- Occupation Distribution

Note: Statistical significance testing is outside the scope of the initial SQL analysis and may require a statistical analysis tool such as Python.

---

# Phase 2 — Financial Performance

## BR-04 — Transaction Volume & Trends

### Business Question

What is the monthly trend in total transaction volume?

Break the analysis down by:

- Transaction Type
- Transaction Channel

### Business Objective

Understand customer transaction behavior and identify changes in banking channel usage.

### Key Metrics

- Transaction Count
- Transaction Amount
- Deposit Volume
- Withdrawal Volume
- Channel Distribution

---

## BR-05 — Branch Performance

### Business Question

Which branches generate the highest financial activity through their linked accounts?

### Business Objective

Compare branch performance and identify high-performing locations.

### Key Metrics

- Transaction Count
- Transaction Amount
- Account Count
- Customer Count

---

## BR-06 — Loan Portfolio Health

### Business Question

Assess the overall health and risk of the bank's loan portfolio.

### Business Objective

Monitor loan performance and identify potential credit risk.

### Key Metrics

- Total Loan Amount
- Active Loans
- Defaulted Loans
- Default Rate
- Loan Payment Amount
- Interest Component
- Late Payment Rate

---

# Phase 3 — Card & Fraud Analytics

## BR-07 — Fraud Detection

### Business Question

What is the overall fraud rate for card transactions?

Which merchant categories have the highest frequency of fraudulent transactions?

### Business Objective

Identify areas of elevated fraud exposure and support fraud monitoring.

### Key Metrics

- Total Card Transactions
- Fraudulent Transactions
- Fraud Rate
- Fraud Amount
- Fraud by Merchant Category

---

## BR-08 — Credit Card Utilization

### Business Question

Identify customers who consistently utilize more than 80% of their available credit limit.

### Business Objective

Identify customers with high credit exposure and potential credit risk.

### Key Metrics

- Credit Limit
- Transaction Amount
- Utilization Rate
- High-Utilization Customers

---

# Phase 4 — Customer Support

## BR-09 — SLA & Resolution Time

### Business Question

Calculate the average turnaround time required to resolve customer support tickets.

Identify tickets that exceeded the 48-hour resolution SLA.

### Business Objective

Evaluate operational efficiency and identify service delays.

### Key Metrics

- Ticket Count
- Average Resolution Time
- SLA Breach Count
- SLA Breach Rate

---

## BR-10 — Support Root Cause Analysis

### Business Question

What are the most frequent customer issues?

### Business Objective

Identify recurring operational problems and prioritize improvement initiatives.

### Key Metrics

- Ticket Volume
- Issue Type
- Ticket Status
- Resolution Time

Note: Employee-level complaint analysis is not currently supported because the support ticket data does not contain an employee identifier.

---

## BR-11 — Customer Satisfaction

### Business Question

How does resolution time relate to customer satisfaction?

### Business Objective

Determine whether slower resolution is associated with lower customer satisfaction.

### Key Metrics

- Average CSAT
- Average Resolution Time
- CSAT by Resolution Time
- Satisfaction Distribution

Note: SQL will be used for descriptive analysis. Statistical correlation testing may require Python or another statistical tool.
