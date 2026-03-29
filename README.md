HR Analytics Dashboard Report (Power BI)
1. Project Overview

This project focuses on transforming raw HR data into an interactive Power BI dashboard to analyze employee attrition trends. The goal was to provide actionable insights into workforce behavior, identify key drivers of attrition, and support data-driven HR decision-making.

2. Data Preparation
Data Source

The dataset consists of employee-level HR records, including:

Demographics (Age, Gender, Education)
Job details (Role, Department, Salary)
Employment metrics (Years at Company, Attrition)
Data Cleaning (Power Query)

I performed the following steps in Power Query:

Removed duplicate and null records
Standardized column names for consistency
Converted data types (e.g., numeric, categorical)
Created categorical bins:
Salary groups (e.g., Up to 5k, 5k–10k, etc.)
Age groups (e.g., 18–25, 26–35, etc.)
3. Data Modeling
Data Structure
Used a single-table model (sufficient for this dataset size)
Ensured proper relationships (if multiple tables were used)
Calculated Measures (DAX)

Created key KPIs using DAX:

Employee Count = COUNT(Employee ID)
Attrition Count = COUNT where Attrition = Yes
Attrition Rate (%) = Attrition Count / Employee Count
Average Age
Average Salary
Average Years at Company
4. Dashboard Design
Layout Strategy

The dashboard was designed using a top-down analytical flow:

High-level KPIs (Top Section)
Demographic Analysis (Middle Section)
Behavioral & Job Insights (Bottom Section)
5. Key Visualizations
A. KPI Cards

Displayed key metrics:

Total Employees: 1470
Attrition Count: 238
Attrition Rate: 16%
Average Age: 37
Average Salary: 6.5K
Average Years: 7

B. Attrition by Gender
Visual: Stacked bar chart
Insight: Higher attrition among male employees (151) vs female (87)
C. Attrition by Education
Visual: Donut chart
Insight:
Life Sciences contributes the highest attrition (37%)
Followed by Medical and Marketing
D. Attrition by Age Group
Visual: Column chart
Insight:
Highest attrition in 26–35 age group
Younger employees show higher turnover tendency
E. Attrition by Salary
Visual: Horizontal bar chart
Insight:
Majority of attrition occurs in lower salary ranges (≤5k)
F. Attrition by Years at Company
Visual: Line chart
Insight:
Peak attrition occurs in early tenure (0–2 years)
Indicates onboarding/retention issues
G. Attrition by Job Role
Visual: Horizontal bar chart
Insight:
Research Scientist (100) has the highest attrition
Followed by Human Resources and Sales
H. Job Role Matrix
Visual: Table with breakdown
Insight:
Shows attrition distribution across levels/ratings per job role
Helps identify role-specific risk areas
6. Interactivity
Added department filters (HR, R&D, Sales) for dynamic analysis
Enabled cross-filtering across visuals
Users can drill down into specific segments
7. Key Insights
Attrition is concentrated among:
Younger employees (26–35)
Lower salary brackets
Employees with shorter tenure
Certain roles (e.g., Research Scientist) have significantly higher attrition
Education background also influences attrition trends
8. Conclusion

This dashboard transforms raw HR data into meaningful insights by:

Highlighting high-risk employee segments
Supporting strategic HR decisions
Enabling interactive exploration of attrition drivers

It demonstrates strong capabilities in:

Data cleaning and transformation
DAX calculations
Data visualization and storytelling
Business insight generation
9. Tools Used
Power BI
Power Query (ETL)
DAX (Data Analysis Expressions)
