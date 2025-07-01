# Layoffs Data Cleaning Project (SQL)
This project focuses on cleaning and preparing a dataset on layoffs using SQL. It was inspired by Alex The Analyst's SQL Data cleaning walkthrough, and all SQL queries were written, grouped, and customized by me to reflect real-world data cleaning steps. 
The dataset was originally provided by [Alex The Analyst](https://github.com/AlexTheAnalyst/SQL-Project), and it contains information on layoffs from global companies across different industries.

## 📦 Dataset
- *Source*: [GitHub – Alex The Analyst](https://github.com/AlexTheAnalyst/SQL-Project)
- *Author*: Alex Freberg (a.k.a. Alex The Analyst)
- *Format*: CSV file imported into MySQL database

## 🛠 Skills Used
- SQL Joins & Subqueries  
- Window Functions (ROW_NUMBER)  
- Common Table Expressions (CTEs)  
- Data Type Conversion  
- Handling NULLs and Empty Strings  
- Text Standardization  
- Date Formatting  
- Self-joins for Filling Missing Values  

## 🧰 Tools Used
- MySQL  
- MySQL Workbench  
- GitHub  
- Notepad  

## 🧹 Cleaning Steps Overview

### Step 1: Setup Staging Tables
- Copied raw data into a staging table  
- Created a second staging table with a row_num column  

### Step 2: Removed Duplicate Records
- Used ROW_NUMBER() in a CTE to identify duplicates  
- Deleted duplicate rows  

### Step 3: Standardized Text Columns
- Trimmed whitespace from company names  
- Cleaned inconsistent values in industry and country columns  

### Step 4: Formatted Dates
- Converted date column from text to proper DATE type  

### Step 5: Handled NULL and Blank Values
- Replaced empty strings with NULL  
- Removed rows with no layoff data  

### Step 6: Filled Missing Industry Info
- Used self-join to fill in missing industry values based on matching company and location  

### Step 7: Final Checks
- Queried cleaned data for edge cases  
- Dropped helper column row_num  

## 💾 Output
The final cleaned table layoffs_staging2 is now ready for use in analysis, visualization, or reporting.

## 📁 Files Included
- layoffs_data_cleaning.sql – Full SQL script grouped by cleaning task  
- README.md – This documentation  

## 👩🏽‍💻 About Me
I’m a data analyst in training, learning by building practical projects. This one helped me apply core SQL techniques used in real-world data cleaning.

## 🔗 Let’s Connect
Have feedback, suggestions or want to collaborate? Feel free to reach out connect with me on LinkedIn.
LinkedIn:https://www.linkedin.com/in/hawawu-a-ogundimu-8a7738371
