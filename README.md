# Employee Data SQL Practice

A beginner-friendly SQL script covering database/table creation, data insertion, and basic querying/filtering techniques using an `employee_data` table.

## 📋 Overview

This script demonstrates core SQL operations on a sample dataset of 10 employee records, including personal details, income, and occupation.

## 🗂️ Table Structure

**Table:** `employee_data`

| Column         | Data Type    | Description                  |
|----------------|--------------|-------------------------------|
| FirstName      | varchar(10)  | Employee's first name        |
| LastName       | varchar(10)  | Employee's last name         |
| DOB            | int          | Year of birth                |
| MaritalStatus  | varchar(10)  | Single / Married             |
| Gender         | varchar(10)  | M / F                         |
| EmailAddress   | varchar(50)  | Employee's email address     |
| AnnualIncome   | int          | Annual income (in currency units) |
| Occupation     | varchar(40)  | Job title / role             |

## 🛠️ What This Script Covers

1. **Database & Table Creation** — Setting up the `task` database and `employee_data` table.
2. **Data Insertion** — Populating the table with 10 sample employee records.
3. **Basic Retrieval** — Selecting all columns and specific columns.
4. **Filtering with WHERE** — Retrieving rows based on column value comparisons.
5. **Sorting** — Ordering results using `ORDER BY`.
6. **Aggregate Functions** — Using `MIN()` combined with a comparison filter.

## 🚀 How to Run

1. Open your preferred SQL client (MySQL Workbench, phpMyAdmin, DBeaver, etc.).
2. Run the script top to bottom, or copy-paste into a query window.
3. Make sure you're connected to a MySQL-compatible server (this script uses MySQL syntax).

```bash
mysql -u your_username -p < employee_data.sql
```

## 📌 Notes

- Column identifiers should not be wrapped in double quotes in MySQL (double quotes are treated as string literals unless `ANSI_QUOTES` mode is enabled). Use backticks (`` ` ``) if quoting is needed, or no quotes at all.
- `DIFFERENCE()` is a SQL Server function and is **not available in MySQL** — an alternative approach (e.g., `ORDER BY` or `LIKE` pattern matching) is used instead for similarity-based filtering.

## 📄 File Structure

```
├── employee_data.sql   # Main SQL script
└── README.md            # Project documentation
```

## 🧑‍💻 Author

Practice project for learning SQL fundamentals: DDL, DML, filtering, and aggregate functions.

## 📜 License

This project is open-source and free to use for learning purposes.
