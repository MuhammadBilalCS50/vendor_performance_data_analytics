# Vendor Performance Data Analytics

## Project Overview

This project builds an end-to-end **data analytics pipeline** to
evaluate vendor performance, profitability, and inventory efficiency
using transactional data.

The workflow covers: - Automated data ingestion into a relational
database - SQL-based data modeling and aggregation - Exploratory Data
Analysis (EDA) - Statistical testing and profitability analysis -
Business-focused insights for vendor selection and pricing optimization

------------------------------------------------------------------------

## Architecture & Workflow

### 1️⃣ Data Ingestion Pipeline

-   Raw CSV files are programmatically ingested using **Pandas**
-   Data is loaded into a **SQLite relational database**
-   Reusable ingestion function implemented with `DataFrame.to_sql()`
-   Logging configured using Python `logging` module
-   Runtime tracking using `time` module
-   Database connection managed via **SQLAlchemy**

🔹 Demonstrates: Data Engineering fundamentals, ETL pipeline design,
logging best practices, database integration

------------------------------------------------------------------------

### 2️⃣ Database Exploration & Modeling

-   SQL queries used to:
    -   Inspect schema and tables
    -   Validate record counts
    -   Join and explore transactional data
-   Created aggregated summary table: `vendor_sales_summary`
-   Structured vendor-level KPIs for downstream analysis

🔹 Demonstrates: SQL proficiency, relational data modeling, validation
workflows

------------------------------------------------------------------------

### 3️⃣ Exploratory Data Analysis (EDA)

-   Summary statistics using `describe()`
-   Distribution analysis with histograms (Seaborn/Matplotlib)
-   Outlier detection using boxen plots
-   Identification of:
    -   Negative gross profit
    -   Infinite / undefined profit margins
    -   Unsold inventory
    -   High variance vendors

🔹 Demonstrates: Data profiling, anomaly detection, visualization skills

------------------------------------------------------------------------

### 4️⃣ Statistical Analysis

-   Hypothesis testing using **SciPy**
-   Independent t-tests (`ttest_ind`) for vendor comparison
-   Profitability distribution analysis
-   Margin behavior evaluation

🔹 Demonstrates: Applied statistics, hypothesis-driven analysis,
business interpretation of results

------------------------------------------------------------------------

## Key Business Insights Generated

-   Identified vendors generating negative gross profit
-   Detected inventory inefficiencies (products purchased but never
    sold)
-   Evaluated profit margin stability
-   Highlighted high-performing vs underperforming vendors
-   Provided data-backed direction for:
    -   Vendor selection
    -   Pricing optimization
    -   Inventory management

------------------------------------------------------------------------

## Tech Stack

-   Python
-   Pandas
-   NumPy
-   SQLite
-   SQLAlchemy
-   Matplotlib
-   Seaborn
-   SciPy
-   Logging (production-style monitoring)

------------------------------------------------------------------------

## Skills Demonstrated

✔ End-to-End Data Pipeline Development\
✔ Relational Database Design & SQL Querying\
✔ Data Cleaning & Validation\
✔ Exploratory Data Analysis (EDA)\
✔ Statistical Testing & Hypothesis Validation\
✔ Business-Oriented Data Interpretation\
✔ Production-Level Logging & Structured Workflow

------------------------------------------------------------------------

## Why This Project Matters

This project goes beyond notebook-level analysis. It demonstrates the
ability to:

-   Engineer a reproducible data pipeline
-   Work with structured databases
-   Translate raw transactional data into strategic vendor insights
-   Apply statistical rigor to business decisions


------------------------------------------------------------------------
