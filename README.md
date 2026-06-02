# SCT_DA_3 - HR Employee Attrition Dashboard
Project Overview

This project is an interactive HR Employee Attrition Dashboard developed using Power BI. The dashboard analyzes employee attrition patterns and helps identify the key factors contributing to employee turnover.

The objective is to answer the question:

"Why are employees leaving the organization?"

Dataset
Dataset: IBM HR Analytics Employee Attrition Dataset
Format: CSV
Records: Employee demographic, job, salary, satisfaction, and attrition information.
Tools Used
Power BI Desktop
Power Query Editor
DAX (Data Analysis Expressions)
Dashboard Features
KPI Cards
Total Employees
Attrition Count
Attrition Rate (%)
Visualizations
Attrition Count by Department
Attrition Count by Age Group
Attrition Count by Job Satisfaction
Overtime Analysis (Pie Chart)
Interactive KPI Metrics
Interactive Filters (Slicers)
Department
Age Group
Job Role
Key Insights
Research & Development department has the highest attrition.
Employees working overtime are more likely to leave.
Adult age group contributes the highest attrition count.
Lower job satisfaction is associated with increased attrition.
Overall attrition rate is approximately 22.84%.
DAX Measures Used
Total Employees
Total Employees =
COUNT('WA_Fn-UseC_-HR-Employee-Attrition'[EmployeeNumber])
Attrition Count
Attrition Count =
CALCULATE(
    COUNT('WA_Fn-UseC_-HR-Employee-Attrition'[Attrition]),
    'WA_Fn-UseC_-HR-Employee-Attrition'[Attrition] = "Yes"
)
Attrition Rate
Attrition Rate % =
DIVIDE([Attrition Count], [Total Employees])
Project Workflow
Imported HR Attrition Dataset into Power BI.
Cleaned and transformed data using Power Query.
Created Age Group categories.
Developed DAX measures for KPIs.
Built interactive visualizations.
Added slicers for dynamic filtering.
Derived insights from attrition trends.
Dashboard Objective

The dashboard enables HR teams and management to:

Monitor employee turnover.
Identify departments with high attrition.
Understand the impact of overtime and job satisfaction.
Support data-driven employee retention strategies.
Repository Structure
HR-Employee-Attrition-Dashboard/
│
├── Dataset/
│   └── WA_Fn-UseC_-HR-Employee-Attrition.csv
│
├── PowerBI/
│   └── HR_Employee_Attrition_Dashboard.pbix
│
├── Screenshots/
│   └── Dashboard.png
│
└── README.md
Author

Mouni

Internship Task

SkillCraft Technology – Task 03
Interactive Visualization Dashboard using Power BI.
