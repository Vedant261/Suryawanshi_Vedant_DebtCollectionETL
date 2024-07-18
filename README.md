# Suryawanshi_Vedant_DebtCollectionETL
Perform a basic ETL (Extract, Transform, Load) process on a CSV file containing borrower data, load it into a SQL database, and conduct simple analysis for debt collection purposes
# Debt Collection ETL and Basic Analysis

## Overview
This project involves extracting, transforming, and loading (ETL) borrower data from a CSV file into a MySQL database and conducting basic analysis for debt collection purposes. The project includes Python code in a Jupyter Notebook, SQL queries for analysis, and a detailed report on the analysis results.

## Files and Directories

### 1. `Debt_Collection_ETL.ipynb`
- **Description:** Jupyter Notebook containing the Python code for the ETL process. This notebook reads the borrower data from a CSV file, performs necessary data transformations, and loads the data into a MySQL database.
- **Key Sections:**
  - **Data Extraction:** Reads data from `5k_borrowers_data.csv`.
  - **Data Transformation:** Cleans and standardizes the data.
  - **Data Loading:** Creates a table in MySQL and loads the transformed data into it.
  - **Error Handling:** Includes basic error handling for common issues like file not found or database connection errors.

### 2. `analysis_queries.sql`
- **Description:** SQL script containing queries for basic analysis of the borrower data. These queries are designed to answer specific business questions related to debt collection.
- **Queries:**
  - **Average Loan Amount:** Calculates the average loan amount for borrowers who are more than 5 days past due.
  - **Top Borrowers:** Identifies the top 10 borrowers with the highest outstanding balance.
  - **Good Repayment History:** Lists all borrowers with a good repayment history (no delayed payments).
  - **Loan Type Analysis:** Provides a brief analysis of loan types, including count, average loan amount, and average credit score for each loan type.

### 3. `analysis_results.txt`
- **Description:** Text file containing the results of the SQL queries executed against the MySQL database. This file provides the output of each analysis query along with brief interpretations.
- **Contents:**
  - **Query Results:** Detailed results of each SQL query, formatted in a readable manner.
  - **Interpretations:** Brief interpretations and insights derived from the query results.

### 4. `README.md`
- **Description:** This file. Provides an overview of the project, detailed descriptions of each file, and instructions for setting up and running the project.

## Prerequisites
- Python 3.x
- Jupyter Notebook
- pandas library
- mysql-connector-python library
- MySQL database

## Setup

### 1. Install Required Python Packages
Install the necessary Python packages using pip:
```bash
pip install pandas mysql-connector-python jupyter
