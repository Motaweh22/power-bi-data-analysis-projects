# Customer Churn Analysis Dashboard | Power BI

An interactive Power BI dashboard designed to analyze customer churn within a telecommunications company. The report explores customer demographics, contract information, service usage, payment methods, and billing data to identify patterns associated with customer attrition and support data-driven business decisions.

---

## Project Overview

Customer retention is one of the most important performance indicators for subscription-based businesses. Understanding why customers leave allows organizations to improve retention strategies, reduce revenue loss, and enhance customer satisfaction.

This Power BI dashboard provides a comprehensive analysis of customer churn by examining customer demographics, contract details, payment methods, international calling behavior, data plans, and additional service charges. The report combines high-level executive KPIs with detailed analytical views, enabling stakeholders to identify high-risk customer segments and investigate the factors contributing to churn.

---

# Business Problem

A telecommunications company wants to understand the factors that contribute to customer churn and identify customer segments with a higher likelihood of leaving the service.

The dashboard supports business users by answering questions such as:

- Which customer segments have the highest churn rate?
- Does contract length influence customer retention?
- How does customer age relate to churn?
- Do payment methods impact customer retention?
- Are international customers more likely to churn?
- How do additional service charges affect customer behavior?

---

# Project Objectives

- Monitor overall customer churn performance.
- Analyze churn across demographic segments.
- Compare churn between different contract types.
- Evaluate customer behavior based on payment methods.
- Investigate international calling activity.
- Analyze unlimited data plan adoption.
- Explore churn categories and churn reasons.
- Identify relationships between additional charges and customer churn.

---

# Dataset

| Property | Details |
|----------|---------|
| Dataset | Databel Customer Dataset |
| Domain | Telecommunications |
| Format | CSV |
| Number of Tables | 1 |
| Granularity | One record per customer |
| Primary Key | Customer ID |

## Dataset Fields

### Customer Information

- Customer ID
- Churn Label
- Churn Category
- Churn Reason

### Demographics

- Age
- Gender
- Under 30
- Senior

### Contract Information

- Contract Type
- Payment Method
- Group Contract
- State
- Account Length

### Usage Metrics

- Local Calls
- International Calls
- International Minutes
- International Plan
- Customer Service Calls
- Average Monthly GB Download
- Unlimited Data Plan

### Financial Metrics

- Monthly Charges
- Total Charges
- Extra International Charges
- Extra Data Charges

---

# Data Preparation

The dataset was imported into Power BI for analysis.

The following Power Query implementation details **cannot be verified** from the PBIX file alone:

- Data type conversions
- Missing value handling
- Duplicate removal
- Custom columns
- Conditional columns
- Query merges
- Applied transformation steps

> **Status:** Not Available

---

# Data Model

## Verified

- Single customer-level analytical dataset.

## Not Available

The following implementation details cannot be verified without access to the Power BI semantic model:

- Table relationships
- Fact tables
- Dimension tables
- Star schema
- Snowflake schema

---

# DAX Measures

The dashboard contains multiple calculated measures used to produce KPI cards and analytical visuals. However, the PBIX file does not expose DAX expressions outside Power BI Desktop.

Therefore, the following information cannot be verified:

- Measure names
- DAX formulas
- Calculation logic

> **Status:** Not Available

---

# Key Performance Indicators (KPIs)

The dashboard contains multiple KPI cards summarizing customer churn performance.

| KPI | Definition | Business Meaning |
|------|------------|------------------|
| Total Customers | Total number of customers | Overall customer base |
| Churned Customers | Customers who left the company | Measures customer loss |
| Churn Rate | Percentage of churned customers | Primary customer retention metric |
| Additional KPI Cards | Present in the dashboard | Exact calculations cannot be verified |

---

# Dashboard Structure

## 1. Overview

### Purpose

Provides a high-level summary of customer churn performance.

### Business Questions

- What is the overall churn rate?
- How many customers have churned?
- Which customer groups require further analysis?

---

## 2. Churn Demographics

### Purpose

Analyze customer churn across demographic characteristics.

### Business Questions

- Which age groups experience the highest churn?
- Does customer gender influence churn?

---

## 3. Groups & Categories

### Purpose

Investigate churn categories and customer groups.

### Business Questions

- What are the primary churn categories?
- Which customer groups contribute most to churn?

---

## 4. Unlimited Data Plan

### Purpose

Compare customers with and without unlimited data plans.

### Business Questions

- Does unlimited data improve customer retention?
- Are additional data charges associated with churn?

---

## 5. International Calls

### Purpose

Analyze international calling behavior.

### Business Questions

- Are international customers more likely to churn?
- How do international charges relate to customer retention?

---

## 6. Contract Type

### Purpose

Compare customer churn across different contract durations.

### Business Questions

- Which contract type has the highest churn?
- Do long-term contracts improve retention?

---

## 7. Age Groups

### Purpose

Analyze churn across different customer age ranges.

### Business Questions

- Which age groups have the highest churn?
- Are younger customers more likely to leave?

---

## 8. Payment & Contracts

### Purpose

Analyze payment behavior and contract information.

### Business Questions

- Which payment methods are associated with churn?
- How do payment methods interact with contract types?

---

## 9. Extra Charges

### Purpose

Investigate the relationship between additional service charges and customer churn.

### Business Questions

- Do additional fees increase churn?
- Which customers incur the highest extra charges?

---

## 10. Insights

### Purpose

Summarize the major analytical findings and support executive decision-making.

---

# Visualizations

The report uses a variety of visualization types to present customer churn insights.

| Visualization | Purpose |
|--------------|---------|
| KPI Cards | Present high-level business metrics |
| Clustered Bar Charts | Compare customer segments |
| Clustered Column Charts | Compare categorical values |
| Line Charts | Display trends and comparisons |
| Line & Column Combo Charts | Compare totals and rates simultaneously |
| Donut Charts | Show proportional distributions |
| Pie Charts | Display category composition |
| Scatter Plot | Explore relationships between numerical variables |
| Tables | Present detailed customer information |
| Matrix | Compare multiple dimensions simultaneously |
| Map | Visualize customer distribution by state |
| Slicers | Enable interactive filtering |

---

# Filters & Interactions

The report includes interactive features that allow users to explore the data dynamically.

### Verified

- Interactive slicers
- Cross-filtering between visuals
- Multi-page report navigation

### Not Available

The following features cannot be verified from the PBIX file:

- Drill-through pages
- Bookmarks
- Custom tooltips
- Buttons
- Sync slicers

---

# Key Insights

The dashboard is designed to help identify:

- Customer segments with higher churn rates.
- The impact of contract duration on customer retention.
- Relationships between payment methods and churn.
- International customer behavior.
- The effect of unlimited data plans.
- Customer groups associated with higher churn.
- Common churn categories and reasons.
- The relationship between additional charges and customer retention.

> **Note:** Specific numerical findings are intentionally omitted because they cannot be verified without interacting with the report.

---

# Recommendations

The following are analytical recommendations based on the objectives of the dashboard and should not be interpreted as measured outcomes.

- Develop targeted retention campaigns for high-risk customer segments.
- Encourage customers to transition to longer-term contracts.
- Review pricing strategies related to additional service charges.
- Improve customer support for segments with frequent service interactions.
- Monitor customers with heavy international usage for retention opportunities.

---

# Technical Skills Demonstrated

This project demonstrates practical experience with:

- Microsoft Power BI
- Interactive Dashboard Design
- Business Intelligence Reporting
- Customer Churn Analytics
- KPI Development
- Data Visualization
- Exploratory Data Analysis
- Business Storytelling
- Interactive Filtering
- Telecommunications Analytics

---

# Challenges & Limitations

- Power Query transformations cannot be extracted from the PBIX package.
- DAX measures are not accessible outside Power BI Desktop.
- The semantic data model cannot be inspected.
- Table relationships cannot be verified.

Where implementation details could not be confirmed, they have been documented as **Not Available** rather than inferred.

---

# Repository Structure

```text
Customer-Churn-Analysis-Dashboard/
│
├── Dataset/
│   └── Databel - Data.csv
│
├── Report/
│   └── Customer Churn Analysis.pbix
│
├── Images/
│   ├── overview.png
│   ├── demographics.png
│   ├── contracts.png
│   ├── payment-analysis.png
│   └── insights.png
│
├── README.md
└── LICENSE
```

---

# Dashboard Screenshots

```markdown
![Overview](images/overview.png)

![Customer Demographics](images/demographics.png)

![Contract Analysis](images/contracts.png)

![Insights](images/insights.png)
```

---

# Tools & Technologies

- Microsoft Power BI Desktop
- Power Query
- DAX
- CSV Dataset

---

# What This Project Demonstrates

This project demonstrates the ability to design an interactive business intelligence dashboard that transforms customer-level telecommunications data into actionable insights. It showcases skills in dashboard design, KPI reporting, exploratory analysis, data visualization, and business storytelling, enabling stakeholders to investigate customer churn from multiple analytical perspectives and support informed decision-making.
