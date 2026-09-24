# Exploratory Data Analysis in Power BI

## Project Overview

This project demonstrates an **Exploratory Data Analysis (EDA)** workflow using **Power BI**. The report investigates employee demographic, career, and compensation data through interactive visualizations to uncover distributions, identify patterns, detect outliers, and explore relationships between employee attributes and income.

Rather than answering a predefined business question, this project focuses on understanding the underlying characteristics of the dataset using descriptive statistics and visual analytics. It showcases how Power BI can be used as an effective exploratory analysis tool before predictive modeling or business reporting.

---

# Business Problem

**Not Available.**

This project is an exploratory analysis of an employee dataset and is intended to investigate the data rather than solve a specific business problem.

---

# Project Objectives

- Explore the distribution of employees across different job roles.
- Compare employee demographics such as gender, education, and marital status.
- Analyze salary distributions across career stages.
- Detect potential outliers in employee compensation.
- Investigate relationships between work experience and monthly income.
- Visualize correlations using scatter plots.
- Demonstrate statistical visualization techniques available in Power BI.

---

# Dataset

| Property | Details |
|----------|---------|
| Dataset | Glassdoor Employee Dataset |
| Primary Table | `glassdoor` |
| Number of Tables | 1 |
| Number of Records | 500 |
| Number of Columns | 36 |
| Granularity | One record per employee review |
| Time Period | Not Available |

### Selected Columns

- ReviewId
- Age
- Gender
- Education
- MaritalStatus
- JobRole
- Department
- CareerStage
- MonthlyIncome
- HourlyRate
- JobLevel
- YearsAtCompany
- TotalWorkingYears
- NumCompaniesWorked
- Attrition

---

# Data Preparation

Power Query transformation steps could not be verified from the available report metadata.

**Verified Information**

- Dataset successfully loaded into Power BI.

**Not Available**

- Data cleaning
- Missing value handling
- Data type changes
- Query merging
- Column transformations
- Custom columns
- Removed duplicates

---

# Data Model

The report uses a simple data model consisting of a single table.

### Tables

- glassdoor

### Relationships

None.

### Schema

Single-table analytical model.

---

# DAX Measures

No custom DAX measures could be verified from the report metadata.

The report primarily uses implicit aggregations including:

| Aggregation | Purpose |
|-------------|----------|
| Count of ReviewId | Employee count |
| Sum of MonthlyIncome | Total salary |
| Average HourlyRate | Average hourly compensation |

---

# KPIs

| KPI | Definition | Business Meaning |
|-----|------------|------------------|
| Employee Count | Count of ReviewId | Number of employee records |
| Total Monthly Income | Sum of MonthlyIncome | Total monthly compensation represented in the dataset |
| Average Hourly Rate | Average HourlyRate | Average employee hourly compensation |

---

# Dashboard Structure

## Page 1 — Employee Overview

### Purpose

Provide a high-level overview of employee distribution and compensation by job role.

### Business Questions

- Which job roles have the highest number of employees?
- Which job roles contribute the highest total monthly income?

---

## Page 2 — Proportional Analysis

### Purpose

Compare the composition of employees across categorical variables.

### Business Questions

- How does marital status vary across job roles?
- What percentage of employees belongs to each marital status category?

---

## Page 3 — Multiple Category Comparison

### Purpose

Compare employee demographics and compensation across multiple categorical dimensions.

### Business Questions

- How is gender distributed across education levels?
- Does hourly compensation vary across education groups?

---

## Page 4 — Salary Distribution Analysis

### Purpose

Analyze salary distributions using box-and-whisker plots.

### Business Questions

- How does salary vary across career stages?
- Are there salary outliers?
- How do salary distributions differ by gender?

---

## Page 5 — Correlation Analysis

### Purpose

Explore relationships between experience-related variables and monthly income.

### Business Questions

- Does experience correlate with salary?
- Does job level relate to monthly income?
- Does company tenure influence salary?

---

## Page 6 — Enhanced Scatter Analysis

### Purpose

Extend scatter plot analysis by incorporating categorical coloring.

### Business Questions

- How do salary patterns differ across job roles?
- Are specific job roles clustered together?

---

# Visualizations

## Table

Used to present detailed numerical summaries by job role.

**Why**

Allows precise comparison of employee counts and salary totals.

---

## Matrix

Used to compare multiple categorical variables simultaneously.

**Why**

Ideal for cross-tabulation between demographics such as education, gender, and marital status.

---

## Clustered Column Chart

Displays employee counts by job role.

**Why**

Provides quick comparison across categories.

---

## Clustered Bar Chart

Shows total monthly income across job roles.

**Why**

Makes ranking categories easier when labels are long.

---

## 100% Stacked Column Chart

Displays proportional comparisons.

**Why**

Allows comparison of category composition independent of total counts.

---

## Scatter Plot

Visualizes relationships between numerical variables.

Examples include:

- Years at Company vs Monthly Income
- Total Working Years vs Monthly Income
- Job Level vs Monthly Income
- Number of Companies Worked vs Monthly Income

**Why**

Scatter plots are well suited for exploratory correlation analysis.

---

## Box & Whisker Plot

Displays salary distributions.

**Why**

Highlights

- Median
- Quartiles
- Distribution spread
- Outliers

making it valuable for exploratory statistical analysis.

---

## Cards

Summarize key numerical metrics.

**Why**

Provide immediate high-level statistics for the report.

---

# Filters & Interactions

Verified interactions include:

- Cross-filtering
- Cross-highlighting
- Interactive visual selection

No evidence was found for:

- Drill-through
- Drill-down
- Bookmarks
- Buttons
- Report tooltips

---

# Key Insights

The report focuses on exploratory analysis rather than business reporting.

Key observations include:

- Employee distribution varies across different job roles.
- Salary distributions differ among career stages.
- Box plots reveal variation in employee compensation and identify potential outliers.
- Scatter plots enable visual exploration of relationships between experience variables and monthly income.
- Proportional charts facilitate comparison of demographic composition across categories.
- Matrix visuals provide multidimensional comparisons between employee characteristics.

---

# Recommendations

> **The following are analytical recommendations rather than findings from the report.**

- Apply statistical correlation coefficients to quantify observed relationships.
- Perform regression analysis to validate salary trends.
- Introduce slicers for improved report interactivity.
- Add custom DAX measures to calculate descriptive statistics such as median, variance, and standard deviation.
- Incorporate time-based analysis if temporal data becomes available.

---

# Technical Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Microsoft Power BI
- Interactive Dashboard Design
- Statistical Data Visualization
- Distribution Analysis
- Correlation Analysis
- Categorical Data Analysis
- Outlier Detection
- Descriptive Statistics
- Cross-filtering and Visual Interactions
- Business Intelligence Reporting

---

# Challenges & Limitations

- Power Query transformation steps could not be verified.
- No custom DAX measures were available in the report metadata.
- The dataset contains a single table with no relational model.
- No predefined business problem or business requirements were provided.
- Time-series analysis was not possible because the dataset does not include a verified time dimension.

---

# Repository Structure

```
Exploratory-Data-Analysis-PowerBI/
│
├── Dataset/
│   └── glassdoor.csv
│
├── Report/
│   └── Exploratory Data Analysis.pbix
│
├── Images/
│   ├── report-overview.png
│   ├── page1.png
│   ├── page2.png
│   ├── page3.png
│   ├── page4.png
│   ├── page5.png
│   └── page6.png
│
└── README.md
```

---

# Dashboard Screenshots

## Report Overview

![Overview](Images/report-overview.png)

---

## Employee Overview

![Employee Overview](Images/page1.png)

---

## Proportional Analysis

![Proportions](Images/page2.png)

---

## Multiple Category Comparison

![Multiple](Images/page3.png)

---

## Salary Distribution

![Box Plot](Images/page4.png)

---

## Correlation Analysis

![Scatter Plot](Images/page5.png)

---

## Enhanced Scatter Analysis

![Scatter Plot Color](Images/page6.png)

---

# Tools & Technologies

- Microsoft Power BI
- Power Query
- Microsoft Excel / CSV
- MAQ Software Box & Whisker Visual
- Data Visualization
- Exploratory Data Analysis (EDA)

---

# What This Project Demonstrates

This project demonstrates the use of **Power BI as an exploratory data analysis platform**. It showcases how interactive visualizations can be used to understand data distributions, compare categorical variables, identify outliers, and investigate relationships between numerical variables. The report highlights essential analytical techniques—including descriptive statistics, correlation exploration, and distribution analysis—that are commonly performed during the initial stages of a data analysis workflow.
