# 💻 Lab: Load CSV and Query in IBM Db2

This lab is part of the **IBM Introduction to Data Engineering** course on Coursera.

## 📌 Objectives
- Provision an IBM Db2 Lite instance on IBM Cloud
- Load a CSV dataset into a table
- Explore data using SQL

## 🗃️ Dataset
**File**: `exercise03_car_sales_data.csv`  
**Description**: Sample dataset on car sales — includes model, make, price, and other fields.

## 🔄 Steps Performed
1. Created IBM Db2 Lite instance
2. Uploaded CSV to object storage
3. Loaded data using `LOAD` command
4. Ran SQL queries to explore dataset

## 🧪 Sample SQL Queries

```sql
SELECT * FROM CAR_SALES FETCH FIRST 5 ROWS ONLY;
SELECT MAKE, COUNT(*) FROM CAR_SALES GROUP BY MAKE;
SELECT AVG(PRICE) FROM CAR_SALES;
