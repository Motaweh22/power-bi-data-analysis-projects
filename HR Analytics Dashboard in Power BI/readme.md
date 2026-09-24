# HR Analytics Dashboard in Power BI

## Project Overview

This project presents an interactive **HR Analytics Dashboard** developed in Microsoft Power BI to analyze workforce demographics, employee performance, and attrition. The dashboard consolidates employee records and performance review data into a single analytical solution that supports HR professionals in monitoring key workforce metrics, evaluating employee satisfaction, and identifying turnover trends.

The report combines multiple analytical perspectives—including employee demographics, performance evaluations, and attrition analysis—through interactive visualizations and KPI-driven reporting.

---

# Business Problem

Organizations require a centralized reporting solution to monitor workforce health, employee performance, and retention. Without a unified dashboard, HR teams may struggle to identify workforce trends, evaluate employee satisfaction, or understand factors related to employee attrition.

This dashboard provides an integrated view of HR data, enabling stakeholders to explore employee information, monitor performance metrics, and analyze workforce changes through interactive reporting.

---

# Project Objectives

- Monitor overall workforce size and employee status.
- Track employee attrition across the organization.
- Analyze workforce demographics.
- Evaluate employee performance reviews.
- Measure employee satisfaction across multiple dimensions.
- Compare self-evaluations with manager evaluations.
- Monitor performance review timelines.
- Support HR decision-making through interactive reporting.

---

# Dataset

## Data Source

HR Analytics Case Study Dataset

## Tables

| Table | Description |
|--------|-------------|
| Employee | Employee master data |
| Performance | Employee performance review records |
| EducationLevel | Education lookup table |
| RatingLevel | Performance rating lookup table |
| SatisfiedLevel | Satisfaction level lookup table |
| DimDate | Calendar table generated using DAX |

## Granularity

- Employee table: One record per employee.
- Performance table: One record per employee performance review.

## Main Fields

### Employee

- EmployeeID
- FirstName
- LastName
- Gender
- Age
- Department
- BusinessTravel
- DistanceFromHome
- State
- Ethnicity
- Education
- EducationField
- JobRole
- MaritalStatus
- Salary
- StockOptionLevel
- Overtime
- HireDate
- Attrition
- YearsAtCompany
- YearsInMostRecentRole
- YearsSinceLastPromotion
- YearsWithCurrManager

### Performance

- PerformanceID
- EmployeeID
- ReviewDate
- EnvironmentSatisfaction
- JobSatisfaction
- RelationshipSatisfaction
- WorkLifeBalance
- SelfRating
- ManagerRating
- TrainingOpportunitiesWithinYear
- TrainingOpportunitiesTaken

---

# Data Preparation

Verified transformations include:

- Creation of a dedicated **DimDate** calendar table.
- Calendar generated dynamically using the minimum and maximum employee hire dates.
- Addition of calendar attributes including:
  - Year
  - Month
  - Quarter
  - Week
  - Fiscal Year
  - Fiscal Quarter
  - Fiscal Month
  - Month Start/End
  - Quarter Start/End

Additional Power Query transformations cannot be verified from the available files.

---

# Data Model

The report follows a **Star Schema**.

## Fact Table

- Performance

## Dimension Tables

- Employee
- EducationLevel
- RatingLevel
- SatisfiedLevel
- DimDate

## Relationships

| From | To |
|------|----|
| Employee.EmployeeID | Performance.EmployeeID |
| EducationLevel.EducationLevelID | Employee.Education |
| RatingLevel.RatingID | Performance.SelfRating |
| RatingLevel.RatingID | Performance.ManagerRating |
| SatisfiedLevel.SatisfactionID | EnvironmentSatisfaction |
| SatisfiedLevel.SatisfactionID | JobSatisfaction |
| SatisfiedLevel.SatisfactionID | RelationshipSatisfaction |
| SatisfiedLevel.SatisfactionID | WorkLifeBalance |

---

# DAX Measures

The following measures are used throughout the report.

| Measure | Purpose | Business Meaning |
|----------|----------|------------------|
| TotalEmployees | Counts employees | Overall workforce size |
| ActiveEmployees | Counts active employees | Current workforce |
| InactiveEmployees | Counts former employees | Employees who have left |
| % Attrition Rate | Calculates attrition percentage | Workforce turnover |
| TotalEmployeesDate | Employee count using alternate date relationship | Time-based employee analysis |
| LastReviewDate | Latest review date | Most recent performance review |
| NextReviewDate | Upcoming review date | Future review planning |
| EnvironmentSatisfaction | Average environment satisfaction | Workplace environment perception |
| JobSatisfaction | Average job satisfaction | Employee satisfaction with role |
| RelationshipSatisfaction | Average relationship satisfaction | Workplace relationships |
| WorkLifeBalance | Average work-life balance | Employee work-life balance |
| SelfRating | Average self-evaluation | Employee performance perception |
| ManagerRating | Average manager evaluation | Manager assessment |

> The underlying DAX expressions are not available from the provided files.

---

# KPIs

| KPI | Definition | Business Meaning |
|-----|------------|------------------|
| Total Employees | Total employee count | Organization size |
| Active Employees | Current employees | Active workforce |
| Inactive Employees | Employees who left | Workforce turnover |
| Attrition Rate | Percentage of inactive employees | Employee retention |
| Last Review Date | Most recent performance review | Review tracking |
| Next Review Date | Upcoming review date | Performance planning |
| Manager Rating | Average manager score | Manager evaluation |
| Self Rating | Average self score | Employee self-assessment |
| Job Satisfaction | Average satisfaction score | Employee engagement |
| Environment Satisfaction | Average environment score | Workplace quality |
| Relationship Satisfaction | Average relationship score | Team collaboration |
| Work-Life Balance | Average work-life balance | Employee wellbeing |

---

# Dashboard Structure

## 1. Overview

### Purpose

Provides an executive summary of the workforce.

### Target Audience

- HR Managers
- HR Directors
- Executives

### Business Questions

- How many employees are currently active?
- What is the attrition rate?
- How is the workforce distributed?
- What are the organization's key HR metrics?

---

## 2. Demographics

### Purpose

Analyzes employee characteristics and workforce composition.

### Target Audience

- HR Business Partners
- Workforce Planning Teams

### Business Questions

- What is the employee age distribution?
- How are employees distributed across departments?
- What is the gender distribution?
- What education levels exist within the company?

---

## 3. Performance Tracker

### Purpose

Evaluates employee performance and satisfaction.

### Target Audience

- HR Managers
- Department Managers

### Business Questions

- How satisfied are employees?
- How do employees rate themselves?
- How do managers rate employees?
- How has performance changed over time?

---

## 4. Attrition

### Purpose

Analyzes employee turnover.

### Target Audience

- HR Leadership
- Management

### Business Questions

- Which employee groups experience higher attrition?
- How has attrition changed over time?
- Which workforce segments require attention?

---

# Visualizations

## KPI Cards

Display headline workforce metrics for quick executive monitoring.

---

## Clustered Column Charts

Compare employee metrics across different categories.

---

## Clustered Bar Charts

Highlight comparisons between departments and workforce groups.

---

## Line Charts

Display changes in performance and HR metrics over time.

---

## Line & Column Combination Charts

Combine trends and totals for easier comparison.

---

## Donut Chart

Visualizes proportional distributions such as workforce composition.

---

## Treemap

Displays hierarchical workforce composition.

---

## Tables

Provide detailed employee and performance information.

---

## Date Slicer

Allows users to filter performance metrics by review date.

---

# Filters & Interactions

The report includes:

- Interactive date slicer
- Cross-filtering between visuals
- Interactive KPI updates
- Page navigation buttons
- Page Navigator visual

Bookmarks and advanced interactions cannot be verified from the available files.

---

# Key Insights

The dashboard enables users to:

- Monitor workforce growth and employee counts.
- Analyze employee attrition across the organization.
- Compare self-assessments with manager evaluations.
- Monitor employee satisfaction across multiple dimensions.
- Evaluate workforce demographics.
- Track employee performance review timelines.

The report is designed for exploratory analysis rather than presenting fixed business conclusions.

---

# Recommendations

> The following recommendations are analytical suggestions based on the dashboard's capabilities and are **not measured outcomes**.

- Investigate departments with higher attrition rates.
- Monitor employees reporting low satisfaction scores.
- Compare manager and self-evaluation discrepancies.
- Increase training opportunities for lower-performing employee groups.
- Use demographic insights to support workforce planning.
- Monitor long-term employee retention trends.

---

# Technical Skills Demonstrated

- Microsoft Power BI
- Interactive Dashboard Design
- HR Analytics
- Data Modeling
- Star Schema Design
- DAX Measures
- Date Intelligence
- KPI Development
- Workforce Analytics
- Employee Performance Analysis
- Attrition Analysis
- Data Visualization
- Cross-filtering
- Interactive Reporting
- Business Intelligence

---

# Challenges & Limitations

- Power Query transformation steps cannot be verified from the provided files.
- The underlying DAX formulas are not available.
- Visual interaction settings beyond standard filtering cannot be confirmed.
- Dataset time period is not explicitly provided.
- Bookmark behavior cannot be fully verified.

---

# Repository Structure

```
HR-Analytics-Dashboard/
│
├── Dashboard/
│   └── HR Analytics.pbix
│
├── Dataset/
│   ├── Employee.csv
│   ├── PerformanceRating.csv
│   ├── EducationLevel.csv
│   ├── RatingLevel.csv
│   └── SatisfiedLevel.csv
│
├── Images/
│   ├── overview.png
│   ├── demographics.png
│   ├── performance.png
│   └── attrition.png
│
└── README.md
```

---

# Dashboard Screenshots

## Overview

![Overview](images/overview.png)

---

## Demographics

![Demographics](images/demographics.png)

---

## Performance Tracker

![Performance](images/performance.png)

---

## Attrition

![Attrition](images/attrition.png)

---

# Tools & Technologies

- Microsoft Power BI Desktop
- DAX
- Power Query
- Data Modeling
- CSV Files
- Microsoft Excel (Dataset Preparation)

---

# What This Project Demonstrates

This project demonstrates the development of an end-to-end HR analytics solution in Power BI, integrating employee and performance data into an interactive dashboard. It showcases skills in data modeling, DAX-based KPI development, date intelligence, interactive visualization design, and HR reporting. The dashboard enables HR professionals to monitor workforce composition, employee performance, satisfaction, and attrition through a centralized business intelligence solution.
