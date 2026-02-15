# Adecco-Analytics

<div align="center">
  <img src="adecco.jpg" alt="Adecco logo"
       width="420" height="420"
       style="border-radius: 50%; object-fit: cover;" />
</div>

<!--![Adecco](https://logos-world.net/wp-content/uploads/2023/08/Adecco-Logo.png)
![Adecco](https://raw.githubusercontent.com/PratyushPuri/Adecco-Analytics/refs/heads/main/Adecco%20Dash.png)-->

<br>

## Overview

Employee turnover at Adecco India is rising, particularly among junior sales employees. This attrition raises the cost of hiring and training new employees and affects productivity.

In order to determine the main causes of employee departures, this project examines HR data. Finding trends in departmental difficulties, demographics, and job satisfaction is the main goal. The objective is to offer practical insights to boost engagement, lower turnover, and improve retention tactics.

The result will be data-driven suggestions to assist management in cultivating a more stable and contented workforce, which will directly support the expansion and ongoing operations of the business.

## Dataset

This analysis uses a synthetic HR analytics dataset from [Kaggle: HR Analytics Case Study](https://www.kaggle.com/datasets/bhanupratapbiswas/hr-analytics-case-study). It is designed to mimic real-world employee attrition scenarios in a mid-sized organization. The dataset contains **1,470 employee records** across **35 columns**, which include demographic, job-related, and satisfaction-related variables.

- **Source**: Publicly available Kaggle dataset that simulates employee data for attrition modeling.
- **Time Coverage**: Cross-sectional (snapshot of employee status at a single time).
- **Key Variables**:
  - **Target**: `Attrition` (binary: "Yes" or "No") which indicates whether an employee left the company.
  - **Demographics**: `Age`, `Gender`, `MaritalStatus`, `DistanceFromHome`.
  - **Job Details**: `Department`, `JobRole`, `JobLevel`, `YearsAtCompany`, `BusinessTravel`.
  - **Compensation**: `MonthlyIncome`, `HourlyRate`, `DailyRate`, `PercentSalaryHike`.
  - **Satisfaction Metrics**: `JobSatisfaction`, `EnvironmentSatisfaction`, `WorkLifeBalance`, `RelationshipSatisfaction` (all on a scale from 1 to 4).
  - **Work History**: `TotalWorkingYears`, `NumCompaniesWorked`, `YearsSinceLastPromotion`.
- **Notes**: 
  - `EmployeeCount` and `StandardHours` are constants (1 and 80, respectively) and were excluded from the analysis.
  - `Over18` is consistently "Y" and therefore redundant.
  - All data is anonymized and synthetic, meant for educational and analytical practice.

## Analysis

> Solution File for Analytics is `Adecco.xlsx`

### **Data Analysis Process in Excel**

I analyzed Adecco India's HR data using Microsoft Excel to find insights into employee attrition. The process went step-by-step from data preparation to visualization.

#### **Data Cleaning & Preparation**
* **Initial Assessment:** I loaded the raw HR dataset into Excel to understand its structure, column names, and data types.
* **Standardization & Deduplication:** I removed duplicates and ensured consistency in categorical data, such as department names and attrition status.
* **Handling Missing Values:** I identified and addressed missing or inconsistent entries using filters and logical checks to ensure data integrity for calculations.

#### **Exploratory Data Analysis (EDA) Using Core Excel Functions**
* **Insights:** I used essential functions to answer key questions:
    * **Overall Attrition Rate:** I used `COUNTIF` and `COUNTA` to find the overall turnover rate.
    * **Departmental Trends:** I created **PivotTables** to calculate and compare attrition rates across Engineering, Sales, Marketing, and more, identifying Sales as a critical area.
    * **Demographic Analysis:** I applied **AVERAGE**, **FILTER**, and **PivotTables** to analyze the profiles of departing employees, including average age, income, and gender split.
    * **Key Metrics:** I calculated average employee tenure, overtime prevalence, and satisfaction scores by role using 
