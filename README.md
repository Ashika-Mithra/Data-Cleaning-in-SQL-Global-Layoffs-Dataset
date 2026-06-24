# 🧹 Data Cleaning in SQL – Global Layoffs Dataset

## 🧾 Project Overview

This project focuses on cleaning and preparing a real-world layoffs dataset using SQL. The goal is to transform raw, inconsistent data into a structured and analysis-ready format by removing duplicates, standardizing values, handling missing data, and improving data quality.

---

## 🎯 Objectives

* Remove duplicate records using SQL window functions
* Standardize text data (company, country, industry)
* Convert and format date fields properly
* Handle missing and null values
* Clean inconsistent or duplicate industry entries
* Remove irrelevant or empty records
* Prepare dataset for exploratory data analysis (EDA)

---

## 🛠️ Tools & Technologies

* SQL (MySQL)
* Window Functions (ROW_NUMBER)
* Common Table Expressions (CTEs)
* Data Cleaning Techniques
* String Functions (TRIM, REPLACE)
* Date Functions (STR_TO_DATE)
* Data Transformation Techniques

---

## 📂 Dataset

* Global Layoffs Dataset (Tech industry layoffs)
* Initial table: `layoffs`
* Cleaned table: `layoffs_staging2`

---

## 🧹 Data Cleaning Process

### 1. Data Staging

* Created a staging table to preserve original dataset
* Copied raw data into working environment

---

### 2. Removing Duplicates

* Used `ROW_NUMBER()` window function
* Partitioned data by company, location, industry, and other key fields
* Deleted duplicate records while retaining original entries

---

### 3. Standardizing Data

* Removed extra spaces using `TRIM()`
* Cleaned inconsistent country naming (e.g., trailing characters)
* Standardized company and industry names

---

### 4. Handling Date Values

* Converted string dates into proper DATE format using `STR_TO_DATE()`
* Modified column type for consistency and time-series analysis

---

### 5. Handling Missing Values

* Identified missing industry values
* Filled missing industry data using self-join logic
* Removed records with no meaningful layoffs data

---

### 6. Final Data Cleanup

* Removed fully null records (no layoffs and no percentage data)
* Dropped helper column (`row_num`)
* Final dataset ready for analysis

---

## 📊 Key SQL Concepts Used

* Window Functions (ROW_NUMBER)
* CTEs (Common Table Expressions)
* Self Joins for data imputation
* Data type conversion
* String cleaning functions
* Data filtering and deletion logic

---

## 🧠 Key Learnings

* Real-world data is messy and requires structured cleaning
* Window functions are powerful for detecting duplicates
* Data consistency is critical before performing analysis
* SQL can be used for full ETL-like data preparation workflows
* Handling missing data improves dataset reliability significantly

---

## 🚀 Outcome

The dataset is now:

* Cleaned
* Standardized
* Duplicate-free
* Analysis-ready for SQL exploration and visualization

---

## 📌 Future Improvements

* Add exploratory data analysis (EDA) on cleaned dataset
* Build Power BI / Tableau dashboard
* Combine with economic indicators for deeper insights
* Automate cleaning pipeline using Python + SQL

---

## 📬 Connect

If you're interested in SQL projects, data cleaning, or analytics workflows, feel free to connect.
