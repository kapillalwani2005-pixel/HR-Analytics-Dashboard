HR Analytics Dashboard | Power BI
Project Overview
This project analyzes employee attrition, workforce demographics, salary distribution, and departmental performance using the IBM HR Analytics dataset. The dashboard provides HR managers and business leaders with actionable insights to identify workforce trends, reduce employee turnover, and improve employee retention strategies.

The dashboard was built in Power BI using data cleaning, transformation, DAX measures, and interactive visualizations.

Business Problem
Employee attrition is a major challenge for organizations as it impacts productivity, recruitment costs, and organizational performance.

The objective of this project is to answer key HR questions such as:

What is the current employee attrition rate?
Which departments experience the highest turnover?
How does salary influence employee retention?
What are the demographic characteristics of the workforce?
Which education backgrounds are most represented among employees?
Dataset
Dataset: IBM HR Analytics Employee Attrition Dataset

Records: 1,470 Employees

Features Include:

Employee Age
Department
Gender
Education Field
Monthly Income
Job Role
Attrition Status
Job Satisfaction
Work Life Balance
Years at Company
Tools & Technologies
Power BI
Power Query
DAX
Excel
Data Cleaning & Preparation
Performed the following steps using Power Query:

Checked and handled missing values
Verified data quality using column profiling
Removed duplicate records
Corrected data types
Standardized categorical data
Created custom business columns
Custom Columns Created
Age Group
18-25
26-35
36-45
46-55
55+
Salary Band
Low Salary
Medium Salary
High Salary
Executive Salary
Experience Level
New Employee
Junior
Mid-Level
Senior
DAX Measures Created
Total Employees
Total Employees =
COUNTROWS('HR-Employee-Attrition')
Employees Left
Employees Left =
CALCULATE(
    [Total Employees],
    'HR-Employee-Attrition'[Attrition] = "Yes"
)
Attrition Rate
Attrition Rate =
DIVIDE(
    [Employees Left],
    [Total Employees]
)
Average Salary
Average Salary =
AVERAGE('HR-Employee-Attrition'[MonthlyIncome])
Average Age
Average Age =
AVERAGE('HR-Employee-Attrition'[Age])
Dashboard Features
Executive KPIs
Total Employees
Employees Left
Attrition Rate
Average Salary
Average Employee Age
Department Analysis
Employee distribution across departments
Department-wise attrition analysis
Gender Analysis
Workforce distribution by gender
Attrition comparison by gender
Education Analysis
Employee count by education field
Education background trends
Salary Analysis
Salary distribution by job role
Income contribution across positions
Interactive Filters
Department
Gender
Education Field
Key Insights
Workforce Overview
Total Employees: 1,470
Employees Left: 237
Attrition Rate: 16%
Department Analysis
Research & Development has the largest workforce.
Sales department is another major contributor to employee turnover.
Human Resources has the smallest employee count.
Education Analysis
Life Sciences represents the largest employee group.
Medical and Marketing fields follow in workforce contribution.
Salary Analysis
Management and Sales Executive roles contribute significantly to total salary expenses.
Dashboard Preview
images/hr-dashboard.png

Business Recommendations
Focus retention initiatives on departments with high attrition.
Implement employee engagement programs for at-risk groups.
Review salary structures for critical roles.
Improve career development opportunities for long-tenured employees.
Monitor attrition trends regularly using interactive dashboards.
Project Structure

HR-Analytics-Dashboard/
│
├── Data/
│   └── HR-Employee-Attrition.xlsx
│
├── Dashboard/
│   └── HR Analytics Dashboard.pbix
│
├── Images/
│   └── Dashboard Screenshot.png
│
└── README.md

Skills Demonstrated
Data Cleaning
Data Modeling
Power Query
DAX
Data Visualization
Dashboard Design
HR Analytics
Business Intelligence
KPI Development
Author
Your Name

LinkedIn: https://linkedin.com/in/your-profile

GitHub: https://github.com/your-username
