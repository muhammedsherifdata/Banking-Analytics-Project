# Project Workflow

This project follows a structured end-to-end analytics workflow similar to real-world business environments.

---

# Phase 1 — Database Design

The first phase focused on preparing the analytical database.

Activities:

- Creating the SQL Server database
- Designing the relational schema
- Creating database tables
- Defining primary keys
- Reviewing foreign key relationships
- Importing raw CSV files into SQL Server

---

# Phase 2 — Data Validation

After importing the data, several validation checks were performed.

Validation included:

- Duplicate Detection
- NULL Detection
- Primary Key Validation
- Foreign Key Validation
- Data Type Validation
- Referential Integrity Checks
- Business Integrity Checks

---

# Phase 3 — Data Quality Assessment

Instead of assuming that the imported data was correct, business rules were validated before starting the analysis.

Several inconsistencies were identified and documented.

One important finding was that card ownership did not consistently match account ownership. The technical relationship existed, but the business relationship was inconsistent.

Rather than modifying the source data, the issue was documented as a data quality finding.

---

# Phase 4 — Data Preparation

Power Query will be used to:

- Clean data
- Standardize formats
- Handle missing values
- Create calculated columns
- Prepare analytical tables

---

# Phase 5 — Data Modeling

A semantic model will be built in Power BI using star-schema principles whenever applicable.

Relationships between dimensions and fact tables will be reviewed and optimized for reporting performance.

---

# Phase 6 — Business Analysis

Business KPIs and metrics will be created using DAX.

The analysis will cover:

- Customer Analytics
- Transaction Analytics
- Loan Analytics
- Card Analytics
- Fraud Analysis
- Branch Performance
- Customer Support

---

# Phase 7 — Dashboard Development

An interactive dashboard will be developed for executive reporting and operational analysis.

The dashboard will focus on actionable business insights rather than visual complexity.
