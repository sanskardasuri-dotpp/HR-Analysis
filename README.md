# HR-Analysis
A comprehensive Power BI HR Analytics Dashboard analyzing employee attrition. It tracks key metrics like a 16.1% attrition rate across 1,470 employees. Features interactive visualizations breaking down turnover by age, gender, salary, education, and job role to help organizations make data-driven decisions for employee retention.


# HR Analytics Dashboard 📊

A comprehensive Power BI project designed to track, analyze, and uncover key drivers behind employee attrition. This dashboard empowers HR professionals and business leaders to make data-driven decisions to improve employee retention, optimize workplace satisfaction, and manage human resources effectively.

## 📌 Project Objective
The primary goal of this project is to understand the factors contributing to employee turnover (attrition). By analyzing demographic, financial, and role-based data, this dashboard identifies high-risk areas within the organization, enabling proactive retention strategies.

## 🛠️ Requirements & Tools
To recreate or modify this project, you will need the following:
* **Software:** Microsoft Power BI Desktop (Latest Version)
* **Data Source:** HR Employee Attrition Dataset (typically a CSV or Excel file containing demographic, salary, and job role data).
* **Prerequisite Knowledge:** Basic understanding of Power Query (for data cleaning), DAX (Data Analysis Expressions for calculating KPIs), and Data Modeling.

## 🚀 How We Proceeded (Project Workflow)

### 1. Data Gathering & Import
* Imported the raw HR dataset into Power BI Desktop.
* Verified data types and ensured all columns were correctly formatted for analysis.

### 2. Data Cleaning & Transformation (Power Query)
* Removed duplicates and handled missing values (Nulls/Blanks).
* Created calculated columns where necessary (e.g., grouping ages into specific "Age Groups" like 18-25, 26-35, etc.).
* Standardized text formats for consistency across visuals.

### 3. Data Modeling & DAX Calculations
* Established relationships between tables.
* Created **Key Performance Indicators (KPIs)** using DAX measures, such as:
    * *Total Employees* = `COUNTROWS(HR_Data)`
    * *Total Attrition* = `CALCULATE(COUNTROWS(HR_Data), HR_Data[Attrition] = "Yes")`
    * *Attrition Rate* = `[Total Attrition] / [Total Employees]`

### 4. Dashboard Design & Visualization
* Designed an intuitive UI with a clear visual hierarchy.
* Added slicers (Human Resources, Research & Development, Sales) for interactive filtering.
* Built diverse visualizations (Bar charts, Area charts, Donut charts) to break down attrition by various dimensions.

---

## 💡 Key Insights Extracted

Based on the dashboard analysis, we have uncovered the following critical insights regarding employee turnover:

* **Overall Attrition:** The company is experiencing an overall attrition rate of **16.1%**, with **237** employees leaving out of a total workforce of 1,470.
* **Salary Impact:** Compensation is a massive driver of turnover. The vast majority of attrition (**163 out of 237**) occurs in the lowest salary bracket (Up to 5k). As salary increases, attrition drops dramatically.
* **Age Factor:** The **26-35 age group** shows the highest flight risk (**116 employees**), suggesting mid-level or early-career professionals are leaving the most, possibly for better compensation or career advancement.
* **Tenure & Years at Company:** Attrition spikes heavily in the very **first year** of employment (**59 employees**), indicating potential issues with onboarding, initial job expectations, or probationary periods.
* **High-Risk Job Roles:** **Laboratory Technicians** (62) and **Sales Executives** (57) have the highest turnover rates among all roles.
* **Educational Background:** Employees with a background in **Life Sciences (38%)** and **Medical (27%)** make up the largest portion of the departed workforce.

## 📈 Dashboard Visuals Overview
* **KPI Cards:** Quick glance at Total Employees, Total Attrition, Attrition Rate, Average Age, Average Salary, and Average Years.
* **Attrition by AgeGroup:** Column chart highlighting vulnerable age brackets.
* **Attrition by Salary:** Horizontal bar chart proving the inverse relationship between pay and turnover.
* **Attrition by Years:** Area chart tracking the timeline of when employees are most likely to leave.
* **Attrition by JobRole:** Detailed breakdown (both chart and matrix) of which specific positions struggle with retention.
* **Attrition by Education & Gender:** Demographic breakdowns using Donut and Button visuals.

---
**Author:** [Sanskar Dasuri]
