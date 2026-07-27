# Data Quality Report

## Objective

Before starting the analytical phase, a complete data quality assessment was performed to ensure that the imported dataset was suitable for business analysis.

---

# Validation Summary

| Validation | Status |
|------------|--------|
| Primary Keys | ✅ Passed |
| Duplicate IDs | ✅ Passed |
| NULL IDs | ✅ Passed |
| Referential Integrity | ✅ Passed |
| Business Integrity | ⚠ Partially Passed |

---

# Validation Details

## Customers

- Primary Key validated.
- No duplicate customer IDs.
- No NULL customer IDs.

---

## Accounts

- All accounts reference valid customers.
- All accounts reference valid branches.

---

## Loans

- Every loan belongs to a valid customer.
- Every loan belongs to a valid branch.
- Every loan payment references an existing loan.

---

## Cards

A business validation revealed that card ownership does not consistently match account ownership.

Although the technical relationship between Cards and Accounts exists, customer ownership is inconsistent across most records.

This issue has been documented and excluded from analytical assumptions.

---

## Transactions

All transactions reference valid accounts.

---

## Card Transactions

All card transactions reference valid cards.

---

## Support Tickets

All support tickets reference valid customers.

---

## Employees

All employees reference valid branches.
