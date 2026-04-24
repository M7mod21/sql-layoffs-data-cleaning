# SQL Data Cleaning Project - Layoffs Dataset

## 📌 Project Overview
This project focuses on cleaning and preparing a real-world layoffs dataset using SQL.  
The goal is to transform raw, messy data into a clean and structured format ready for analysis.

---

## 📊 Dataset Description
The dataset contains information about company layoffs, including:
- Company name
- Location
- Industry
- Number of employees laid off
- Percentage of layoffs
- Date
- Company stage
- Country
- Funds raised

---

## 🧹 Data Cleaning Steps

### 1. Create Staging Table
- Created a copy of the original dataset to preserve raw data.

### 2. Remove Duplicates
- Used `ROW_NUMBER()` window function to identify duplicate rows.
- Deleted duplicate records based on key columns.

### 3. Standardize Data
- Removed extra spaces using `TRIM()`
- Standardized industry names (e.g., Crypto)
- Cleaned country values (removed extra characters)
- Converted date column to proper DATE format

### 4. Handle Missing Values
- Converted blank values to NULL
- Filled missing industry values using self JOIN based on company
- Removed rows where both total_laid_off and percentage_laid_off were NULL

### 5. Final Cleanup
- Dropped temporary column `row_num`

---

## 🛠️ Tools Used
- MySQL
- Window Functions (ROW_NUMBER)
- CTE (Common Table Expressions)
- Joins
- Data Cleaning Techniques

---

## 📈 Key Learnings
- How to clean real-world messy datasets using SQL
- How to handle duplicates efficiently
- How to standardize inconsistent data
- How to deal with missing values using SQL techniques

---

## 🚀 Project Outcome
The dataset is now clean, structured, and ready for exploratory data analysis (EDA).

---

## 👤 Author
Mahmoud Aljedaili
