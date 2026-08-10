# DAX Measures

## Transaction Measures

### Total Transaction Amount

```DAX
Total Transaction Amount =
SUM(transactions[amount])

Total Transactions
Total Transactions =
DISTINCTCOUNT(transactions[transaction_id])

Customer Measures
Total Customers
Total Customers =
DISTINCTCOUNT(customers[customer_id])

Average Accounts per Customer
Average Accounts per Customer =
DIVIDE(
    [Total Accounts],
    [Total Customers]
)



Loan Measures

Total Loans =
DISTINCTCOUNT(loans[loan_id])

Total Loan Amount
Total Loan Amount =
SUM(loans[loan_amount])

YOY Analysis
Total Loan Amount PY =
CALCULATE(
    [Total Loan Amount],
    SAMEPERIODLASTYEAR(DimDate[Date]),
    USERELATIONSHIP(
        loans[start_date],
        DimDate[Date]
    )
)

Total Loan Amount YoY % =
DIVIDE(
    [Total Loan Amount] -
    [Total Loan Amount PY],
    [Total Loan Amount PY]
)
Transaction Type Measures
Deposit Amount

Deposit Amount =
CALCULATE(
    SUM(transactions[amount]),
    transactions[txn_type] = "Deposit"
)


Withdrawal Amount

Withdrawal Amount =
CALCULATE(
    SUM(transactions[amount]),
    transactions[txn_type] = "Withdrawal"
)

Transfer In Amount

Transfer In Amount =
CALCULATE(
    SUM(transactions[amount]),
    transactions[txn_type] = "Transfer In"
)

Transfer Out Amount
Transfer Out Amount =
CALCULATE(
    SUM(transactions[amount]),
    transactions[txn_type] = "Transfer Out"
)

Interest Credit Amount
Interest Credit Amount =
CALCULATE(
    SUM(transactions[amount]),
    transactions[txn_type] = "Interest Credit"
)


Dynamic KPI Indicators

YoY KPI indicators were implemented using DAX measures that dynamically change:

Arrow direction
Percentage value
Color

Green indicates positive performance while red indicates negative performance, depending on the business meaning of the KPI.


Date Dim
A dedicated Date Dimension was created to support time intelligence calculations.

Important columns include:

Date
Year
Month Name
Month Number
Year Month
Year Month Sort

The Year Month column is sorted using Year Month Sort to maintain chronological ordering.




---
