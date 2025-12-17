## Shein E-commerce Data Cleaning Project

- ## 📋 Project Overview

This project demonstrates advanced SQL data cleaning techniques on a real-world e-commerce dataset from Shein containing ~20,000 products across 19 product categories. The dataset was heavily corrupted with misaligned columns, inconsistent formatting, and malformed records requiring systematic cleaning.
Goal: Transform a messy, unusable dataset into a clean, analysis-ready table using only SQL.

- ## 🔴 Data Quality Issues Identified

The raw data presented multiple critical issues:

Misaligned columns: Price values appearing in discount field, selling propositions in price field
Inconsistent formatting: Missing currency symbols, irregular patterns across fields
Duplicate entries: Same products with slight variations causing redundancy
Malformed records: URL fragments corrupting the discount field
Null/empty values: Requiring strategic handling and cleanup
Non-standardized values: Bestseller ranks with inconsistent naming (#1 Best Seller vs #1 Best Sellers)

- ## 📊 Dataset Overview

Total products : 59,000+
Categories : 19 (Fashion, Home, Electronics, etc.)
Issues fixed : Misaligned columns, formatting errors, duplicates

- ## 📁 Files

- `Cleaning process with SQL` - Complete cleaning pipeline
- `Analysis queries with SQL` - Business analysis queries  
- `shein clean table.csv` - Final cleaned dataset 
- `shein excel analysis queries tables.xlsx` - Query results visualization

## 🛠️ SQL Techniques Demonstrated

### Data Integration & Schema Design
- `UNION ALL` operations to merge 19 category tables
- Strategic handling of missing columns with `NULL` values
- Column aliasing and standardization

### Data Transformation & Cleaning
- Complex `CASE` statements for conditional logic
- `REGEXP` pattern matching for validation
- String manipulation with `REPLACE()`, `CONCAT()`, `CAST()`
- Numeric conversion handling (e.g., "5k+ sold" → 5000)

### Data Quality & Validation
- Pattern validation to identify malformed records
- `DELETE` operations for corrupted data removal
- Multi-column realignment with conditional `UPDATE`

### Schema Normalization
- `ALTER TABLE` for column renaming and reordering
- Logical column sequencing
- Data type optimization

### Business Analysis
- Aggregations with `GROUP BY` and statistical functions
- Percentage calculations using subqueries
- Custom sorting with `ORDER BY CASE`
- Multi-level categorization with nested `CASE` statements
