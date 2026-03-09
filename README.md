# HR-Analytics-Dashboard-End-to-End-BI-Project
End-to-end BI Analytics project using CSV Data Source, SSIS, SQL Server, and Power BI to analyze HR data.

## Project Overview

This project demonstrates the design and implementation of a complete Business Intelligence (BI) pipeline for HR analytics. The objective was to transform raw HR data into actionable insights through an ETL workflow, structured data modeling, and interactive data visualization.

The solution extracts employee data from a CSV dataset, processes and loads it using an ETL pipeline built with SQL Server Integration Services (SSIS), transforms and models the data within SQL Server using relational tables and analytical views, and finally visualizes key workforce metrics through an interactive dashboard built in Power BI.

The final dashboard was published to the cloud using Microsoft Power BI Service to enable accessible reporting and decision-making.

---

# Business Problem

Organizations rely on HR analytics to understand workforce trends, employee distribution, compensation patterns, and workforce mobility. However, raw HR datasets stored in flat files are difficult to analyze effectively without structured processing and visualization tools.

This project addresses that challenge by building a complete BI pipeline that converts raw HR data into structured insights, enabling HR teams to explore workforce demographics, departmental salary distribution, employee travel patterns, performance ratings, and retirement status.

---

# Data Source

The dataset used in this project is a Human Resources dataset stored as a CSV file containing employee information such as:

- Employee demographics (age, gender, marital status)
- Department and job role
- Monthly income
- Business travel frequency
- Performance ratings
- Attrition indicators
- Employment status and retirement indicators

---

# Data Architecture

The project follows a typical modern BI architecture pipeline:

CSV HR Dataset  
↓  
SSIS ETL Pipeline  
↓  
SQL Server Staging & Analytical Tables  
↓  
SQL Data Cleaning and Transformation  
↓  
SQL Reporting Views  
↓  
Power BI Data Model  
↓  
Interactive Dashboard  
↓  
Published to Power BI Service

---

# ETL Pipeline (SSIS)

An ETL workflow was implemented using SQL Server Integration Services to automate the data ingestion and transformation process.

Key ETL steps include:

1. Extract HR dataset from CSV source
2. Load raw data into SQL Server staging tables
3. Validate and standardize employee attributes
4. Transform and structure data into analytical tables
5. Prepare the dataset for reporting and dashboard consumption

This ETL pipeline ensures data consistency and prepares the dataset for analytical processing.

---

# Data Modeling (SQL Server)

The transformed data is stored in SQL Server where relational tables and reporting views were created.

### Tables

- HR employee data table
- Department reference data
- Job role attributes

### Views
-HR_Data views
- Department workforce summaries
- Salary aggregation views
- Employee demographic reporting views

These views serve as the primary data source for the Power BI report.

---

# Power BI Dashboard

An interactive dashboard was built using Microsoft Power BI Desktop to provide insights into workforce composition and HR metrics.

The dashboard uses DAX measures to calculate key indicators and provide interactive filtering capabilities.

### Workforce Overview

- Total Employees: **1,470**
- Gender Distribution
- Total Monthly Salary Expenditure

### Workforce Distribution

- Total Employees per Job Position
- Employees by Department
- Departmental salary distribution

### Workforce Demographics

- Employees by marital status
- Gender balance

### Workforce Behavior

- Business travel frequency by department
- Performance rating by department

### Workforce Lifecycle

- Employee retirement status (Active vs Near Retirement)

### Detailed Employee Table

A detailed table provides granular insights into:

- Job role
- Department
- Gender distribution
- Salary totals
- Travel frequency metrics
- Retirement status

---

# Key Insights

Some insights derived from the dashboard include:

- Research & Development has the largest workforce and highest salary expenditure.
- A significant portion of employees travel rarely for business across departments.
- Workforce demographics show balanced gender representation.
- Most employees are currently active with a smaller percentage approaching retirement.
- Sales and Research roles make up a large portion of the employee base.

These insights help HR teams monitor workforce structure and support strategic workforce planning.

---

# Tools & Technologies

This project was built using the following tools:

- SQL Server
- SQL Server Integration Services (SSIS)
- Microsoft Power BI Desktop
- Microsoft Power BI Service
- CSV Data Source

---

# Repository Structure

```
HR-Analytics-End-to-End-BI-Project
│
├── Data
│   └── HR_dataset.csv
│
├── SSIS_ETL
│   └── HR_ETL_Package.dtsx
│
├── SQL
│   ├── create_tables.sql
│   ├── data_cleaning.sql
│   └── reporting_views.sql
│
├── PowerBI
│   └── HR_Analytics_Dashboard.pbix
│
├── Images
│   └── SSIS_ETL_Package.png
│   └── HR_dashboard.png
│   └── HR_Detailed_Dashboard.png
│   └── SQL_Database_Create_Views.png 
│
└── README.md
```

---

# Skills Demonstrated

This project demonstrates several key data analytics and BI engineering skills:

- ETL pipeline development using SSIS
- SQL data transformation and cleaning
- relational data modeling
- DAX measure development
- Power BI dashboard design
- business intelligence reporting
- data storytelling through visualization

---

# Author

**Brian Nyakeri Amisi**

Data Analyst | BI Developer | Data Engineer

This project forms part of my professional BI portfolio showcasing end-to-end analytics workflows using SQL Server, SSIS, and Power BI.
