# Sales Analysis Dashboard | Power BI

## Project Overview

This Power BI project presents a sales analysis dashboard designed to visualize financial values across different product categories and time periods. The report provides a high-level overview through KPI cards and interactive charts that support trend analysis using Power BI's built-in date hierarchy.

> **Note:** This documentation is based only on the information verifiable from the provided Power BI report. Any unavailable information is intentionally marked as **Not Available** rather than assumed.

---

# Business Problem

**Not Available**

The Power BI report does not explicitly describe the business problem or business scenario.

Based on the report structure, the dashboard appears to support financial monitoring by comparing budget-related values across time and product categories.

---

# Project Objectives

Based on the report, the dashboard aims to:

- Present high-level financial KPIs.
- Analyze budget values over time.
- Compare product category performance.
- Allow users to drill down into different date levels.
- Provide an interactive overview of business performance.

---

# Dataset

**Status:** Partially Verifiable

The report references the following tables:

| Table | Type |
|--------|------|
| FactStrategyPlan | Fact Table |
| DimDate | Dimension |
| DimProductCategory | Dimension |
| DimAccount | Dimension |

The complete dataset structure and data source are **not available** from the provided report.

---

# Data Preparation (Power Query)

**Not Available**

The Power Query transformations cannot be verified from the provided PBIX metadata.

No assumptions have been made regarding:

- Removed duplicates
- Data type changes
- Merge queries
- Conditional columns
- Custom columns
- Data cleansing steps

---

# Data Model

## Identified Tables

### Fact Table

- FactStrategyPlan

### Dimension Tables

- DimDate
- DimProductCategory
- DimAccount

The report structure suggests a **Star Schema**; however, the complete relationship diagram cannot be verified.

---

# Relationships

**Not Available**

The PBIX metadata available for analysis does not expose the relationship configuration.

---

# DAX Measures

No custom DAX measures could be verified.

The report visuals currently aggregate data using:

```DAX
SUM(FactStrategyPlan[Amount])
```

No evidence was found for measures using:

- CALCULATE()
- FILTER()
- DIVIDE()
- USERELATIONSHIP()
- DATEADD()
- TOTALYTD()

---

# Calculated Columns

**Not Available**

---

# KPIs

The dashboard displays three KPI cards.

| KPI | Calculation |
|------|-------------|
| Actual | SUM(Amount) |
| Budget | SUM(Amount) |
| Forecast | SUM(Amount) |

The report metadata does not expose the filtering logic that differentiates these KPIs.

---

# Dashboard Structure

## Report Pages

### Sales Analysis

The report currently contains a single dashboard page.

---

# Dashboard Components

| Visual | Purpose |
|---------|----------|
| Card | Display Actual value |
| Card | Display Budget value |
| Card | Display Forecast value |
| Clustered Column Chart | Monthly budget analysis |
| Clustered Column Chart | Budget by product category |
| Text Box | Report title or description |

---

# Visualizations

## KPI Cards

Three KPI cards provide an immediate summary of the most important financial values, allowing users to evaluate overall performance before exploring detailed charts.

---

## Budgeted Monthly Amount

Visual Type:

- Clustered Column Chart

Purpose:

- Analyze budget values across time.

Features:

- Date hierarchy
- Product Category legend
- Monthly comparison
- Drill-down support

---

## Budget Product Sold

Visual Type:

- Clustered Column Chart

Purpose:

Compare financial values across product categories.

---

# Date Hierarchy

The dashboard uses a hierarchical date structure.

```
Year
   ↓
Quarter
   ↓
Month
   ↓
Date
```

This enables users to progressively investigate business performance at different time granularities.

---

# Filters & Interactions

Verified interactions include:

- Date hierarchy drill-down
- Category comparison

No slicers, bookmarks, drill-through pages, or tooltips could be verified.

---

# Key Insights

Only structural insights can be confirmed from the report.

The dashboard enables users to:

- Monitor overall financial values.
- Compare categories.
- Analyze monthly trends.
- Navigate through different date levels.

Business conclusions cannot be drawn because the underlying data values are not available.

---

# Technical Skills Demonstrated

This project demonstrates experience with:

- Microsoft Power BI
- Dashboard Design
- KPI Development
- Date Hierarchies
- Clustered Column Charts
- Interactive Drill Down
- Data Aggregation
- Financial Reporting
- Business Intelligence Reporting

---

# Challenges

The provided PBIX metadata does not expose:

- Power Query transformations
- Relationship configuration
- DAX model
- Calculated columns

Therefore, only verifiable information has been documented.

---

# Tools & Technologies

- Microsoft Power BI Desktop
- DAX (SUM aggregation verified)
- Interactive Visualizations
- Date Hierarchies

---

# What This Project Demonstrates

This project demonstrates the ability to:

- Design a clean Power BI dashboard.
- Present business KPIs.
- Build interactive reports.
- Use hierarchical date analysis.
- Organize business metrics using visual storytelling.
- Develop reports suitable for executive-level monitoring.

---

# Repository Structure

```
Sales-Analysis-Dashboard/
│
├── Sales Analysis.pbix
├── README.md
├── images/
│   └── dashboard-overview.png
└── dataset/
```

---

# Dashboard Screenshot

> Replace with an actual screenshot after exporting the report.

```markdown
![Dashboard Overview](images/dashboard-overview.png)
```

---

# Notes

This documentation intentionally avoids assumptions. Every section is based only on information that could be verified from the provided Power BI report.
