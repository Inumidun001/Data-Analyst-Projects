# 🧾 Excel HR Analytics Dashboard – Employees & Departments

## 📌 Project Overview
This project demonstrates how to utilize **Excel** for HR data analysis and dashboard creation. It connects employee records with department details and visualizes key HR metrics, such as the average salary per department and employee count by gender, using PivotTables and formulas.

---

## 🧰 Tools Used
- Microsoft Excel
  - VLOOKUP
  - Conditional Formatting
  - PivotTables
  - Charts 

---

## 📁 File: `Employees Data.xlsx`

### 🔹 Sheet: `Employees`
Contains the raw employee dataset with the following fields:
- `Employee_ID`
- `Name`
- `Gender`
- `Department_ID`
- `Salary`
- `Department_Name` (retrieved using VLOOKUP)

#### ✅ Conditional Formatting
Salary cells have been formatted using the following rules:
- **Above €6,000** → highlighted in **green**
- **Below €4,000** → highlighted in **red**

This highlights outliers and helps quickly spot high or low earners.

---

### 🔹 Sheet: `Departments`
Lookup table for:
- `Department_ID` → `Department_Name`


### 🔹 Sheet: `Dashboard`
Includes key PivotTable outputs:
- **Average Salary by Department**
- **Number of Employees by Gender (Filtered by Departments)**
- **Total Salary per Department**
- **Number of Employees per Department**						

---

## 🔍 VLOOKUP Implementation

The `Department_Name` column in `Employees` was created with:
```excel
=VLOOKUP(D2, Departments!$A$2:$B$6, 2, FALSE)

---


## 🧠 What I Achieved
- Structure clean HR data for analysis
- PivotTables to summarize salary data
- Mapping department names using lookup logic
-Applying conditional formatting to highlight insights
- Planning an HR dashboard to display KPIs


---

📌 This project is a strong example of practical Excel-based data analytics used in HR or business operations.
