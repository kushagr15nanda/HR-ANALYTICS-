# HR Analytics Dashboard

## Overview
This repository contains a Tableau dashboard that provides insights into employee attrition and related HR metrics. The dashboard helps HR professionals understand key trends affecting workforce retention, job satisfaction, and employee demographics.

## Dataset Information
- **Data Source**: The dataset used in this dashboard is related to employee attrition and demographics.
- **Key Metrics Analyzed**:
  - Employee Count
  - Attrition Count
  - Attrition Rate
  - Active Employees
  - Average Age
  - Attrition Rate by Gender
  - Department-wise Attrition
  - Education Field-wise Attrition
  - Job Satisfaction Ratings
  - Number of Employees by Age Group

## Key Performance Indicators (KPIs)
The following KPIs are calculated and visualized in the dashboard:
- **Employee Count**: Total number of employees in the dataset.
- **Attrition Count**: Total number of employees who left the company.
- **Attrition Rate Calculation**: `IF [Attrition] = 'YES' THEN 1 ELSE 0 END`
- **Overall Attrition Rate**: `SUM ([Calculation_27021658477756416]) / SUM ([Employee Count])`
- **Active Employees**: `SUM ([Employee Count]) - SUM ([Calculation_27021658477756416])`
- **Average Age of Employees**: Calculated to understand the workforce age distribution.

## Dashboard Components
The dashboard consists of multiple worksheets providing various perspectives on employee attrition:
1. **Attrition by Gender** - Compares the attrition rate between male and female employees.
2. **Attrition Rate by Gender for Different Age Groups** - Analyzes how attrition varies across different age brackets for each gender using circular charts.
3. **Department-wise Attrition** - Highlights which departments experience the highest turnover through a pie chart representation.
4. **Education Field-wise Attrition** - Examines attrition trends based on employees' educational backgrounds using a horizontal bar chart.
5. **Number of Employees by Age Group** - Provides a demographic breakdown of employees by age using a histogram.
6. **Job Satisfaction Rating** - Displays employee satisfaction ratings using a heatmap, helping HR understand engagement levels.
7. **KPI Overview** - Summarizes key performance metrics in one place for quick reference.

## Insights & Conclusions
- The **Sales** and **HR** departments show the highest attrition rates, suggesting a need for targeted retention strategies.
- Employees in the **30-35 age group** have the highest attrition rate, indicating potential dissatisfaction or career transitions at this stage.
- **Job satisfaction ratings vary by role**, with some roles experiencing lower satisfaction, which may contribute to higher attrition.
- **Education field-wise attrition** reveals that employees with Life Sciences and Medical backgrounds leave more often than others.
- **Gender-based analysis** suggests that male employees have a higher attrition rate than female employees.

## Filters Used in the Dashboard
- **Education**: A dropdown filter allows users to analyze attrition trends by education field.
- **Age Group Binning**: The employee age distribution can be adjusted with a slider.
- **Department Selection**: Users can explore department-wise attrition trends dynamically.

## How to Use
1. Download the `.twb` file from this repository.
2. Open the file using **Tableau Desktop**.
3. Explore different worksheets and dashboards to analyze trends and insights.
4. Use filters to drill down into specific attributes such as department, education, and age groups.

## Technologies Used
- **Tableau Desktop** (for visualization)
- **Data Source**: HR Attrition Dataset (assumed to be from an HR analytics source)

## Contribution
Feel free to modify, improve, or extend the dashboard to suit different HR analytics use cases.

## Screenshot Reference
![HR Analytics Dashboard](./Screenshot.png) 

## License
This project is open-source. You may use and modify it as needed.

