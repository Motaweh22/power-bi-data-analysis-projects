# Wake County Budget Expenditure Analysis Dashboard

> Power BI Data Analytics Dashboard for Monitoring Public Sector Budget Expenditures and Department Spending

---

# Project Overview

This project presents an interactive Power BI dashboard designed to analyze public expenditure data from the Wake County WATCH FY2019 dataset. The dashboard enables users to explore departmental spending, identify over-budget expenditures, analyze expenditure categories, and investigate spending trends through multiple analytical views.

The solution consolidates expenditure information from multiple related datasets into an interactive reporting experience that supports financial transparency and expenditure monitoring. By providing high-level KPIs alongside detailed departmental and expenditure-line analysis, the dashboard allows users to move from executive-level summaries to detailed transaction-level exploration.

The dashboard is intended for analysts, financial managers, auditors, and decision-makers who need to monitor budget utilization, identify departments exceeding planned budgets, and better understand expenditure distribution across cost centers and funds.

---

# Business Problem

Organizations managing public budgets require continuous monitoring of expenditures to ensure departments remain within approved budgets and to identify areas where spending requires further investigation.

Without an integrated reporting solution, analyzing expenditure data across departments, cost centers, and expenditure categories can become time-consuming and difficult.

This dashboard addresses that challenge by providing interactive visualizations that simplify expenditure monitoring and support financial analysis.

## Key Business Questions

- Which departments are operating over budget?
- Which departments contribute the highest expenditures?
- How are expenditures distributed across expenditure categories?
- How does spending vary across departments?
- Which expenditure line items contribute most to total spending?

---

# Project Objectives

## Business Objectives

- Monitor departmental spending.
- Identify departments exceeding budget.
- Analyze expenditure distribution.
- Improve financial reporting through interactive dashboards.

## Analytical Objectives

- Compare expenditure across departments.
- Analyze expenditure categories.
- Identify spending concentration.
- Support detailed expenditure investigation.

## Technical Objectives

- Build an interactive Power BI report.
- Create multiple analytical report pages.
- Implement interactive navigation.
- Provide drill-down style exploration using dedicated report pages and tooltips.

---

# Dataset

| Item | Details |
|-------|---------|
| Data Source | Wake County Open Data (WATCH FY2019) |
| Dataset | WATCH FY2019 Public Expenditure Data |
| Time Period | FY2019 |
| Main Tables | Cost Centers, Expenditures, Expenditure Line Items, Funds |
| Number of Tables | 4 |
| Number of Rows | Not Available |
| Number of Columns | Not Available |
| Data Granularity | Public expenditure records |
| Key Entities | Departments, Cost Centers, Funds, Expenditure Line Items |

The project uses multiple related datasets generated from the Wake County WATCH FY2019 public expenditure data. :chatgpt-content-reference{index="0"}

---

# Data Preparation

The Power BI report was built using multiple structured datasets.

Specific Power Query transformations cannot be verified from the available project files.

**Verified information**

- Multiple datasets imported.
- Public expenditure data consolidated into a single report.

**Power Query Transformations**

Not Available.

---

# Data Model

The report integrates the following tables:

- Cost Centers
- Expenditures
- Expenditure Line Items
- Funds

The exact Power BI semantic model, relationships, cardinality, filter direction, and schema cannot be verified from the available project files.

| Component | Status |
|------------|--------|
| Fact Table(s) | Not Available |
| Dimension Tables | Not Available |
| Relationships | Not Available |
| Cardinality | Not Available |
| Filter Direction | Not Available |
| Schema | Not Available |

---

# DAX Measures

The PBIX report contains DAX calculations; however, the underlying measure definitions cannot be extracted from the available files.

| Measure | Purpose |
|----------|---------|
| Not Available | Not Available |

---

# KPIs

The dashboard includes KPI Card visuals.

The KPI definitions cannot be verified from the available report metadata.

| KPI | Definition | Business Meaning |
|------|------------|------------------|
| Not Available | Not Available | Not Available |

---

# Dashboard Structure

## Page 1 — Over Budget

### Purpose

Provides an executive overview of departments exceeding budget limits.

### Key Components

- KPI Card
- Clustered Bar Chart
- Table
- Navigation Buttons

### Business Questions

- Which departments are over budget?
- Which departments require immediate attention?

---

## Page 2 — Department Breakdown

### Purpose

Provides a detailed departmental spending analysis.

### Key Components

- Line Chart
- Treemap
- Scatter Chart
- KPI Card
- Navigation Button

### Business Questions

- How does spending vary by department?
- Which departments contribute most to expenditures?
- How are expenditures distributed?

---

## Page 3 — Department Tooltip

### Purpose

Provides contextual information when interacting with report visuals.

### Key Components

- Clustered Bar Chart

---

## Page 4 — Expenditure Lines

### Purpose

Provides detailed analysis of expenditure line items.

### Key Components

- KPI Card
- Treemap
- Table
- Q&A Visual
- Navigation Button

### Business Questions

- Which expenditure line items account for the largest spending?
- How are expenditures distributed across categories?

---

# Visualizations

| Visualization | Analytical Purpose |
|---------------|-------------------|
| KPI Cards | Display high-level performance indicators. |
| Clustered Bar Chart | Compare expenditure values across departments or categories. |
| Line Chart | Analyze expenditure trends. |
| Treemap | Visualize proportional contribution of expenditure categories. |
| Scatter Chart | Compare multiple expenditure-related measures. |
| Table | Provide detailed tabular records. |
| Q&A Visual | Enable natural-language exploration of report data. |

---

# Filters & User Interactions

Verified report interactions include:

- Multiple report pages
- Navigation buttons
- Tooltip page
- Cross-page navigation
- Interactive visuals
- Q&A visual

The following features cannot be verified:

- Drill-through
- Bookmarks
- Slicers
- Dynamic titles
- Custom tooltips beyond the dedicated tooltip page

---

# Key Insights

The report structure supports identifying:

- Departments operating above budget.
- Departments with higher expenditure levels.
- Distribution of expenditure across expenditure categories.
- Major expenditure line items.

Specific numerical findings cannot be verified from the available project files.

---

# Findings

- The report provides executive and detailed expenditure analysis.
- Multiple analytical views support financial monitoring.
- Public expenditure information is consolidated into a single interactive dashboard.

---

# Recommendations

The following recommendations are analytical suggestions rather than measured outcomes:

- Monitor departments consistently exceeding budget.
- Investigate expenditure categories with unusually high spending.
- Review major expenditure line items to identify optimization opportunities.
- Use the dashboard regularly for budget monitoring and financial reporting.

---

# Technical Skills Demonstrated

### Power BI

- Interactive Dashboard Development
- Multi-page Report Design
- KPI Reporting
- Navigation Design
- Tooltip Pages
- Q&A Visual

### Data Analysis

- Financial Data Analysis
- Department-Level Analysis
- Budget Monitoring
- Comparative Analysis

### Data Visualization

- KPI Cards
- Line Charts
- Treemaps
- Scatter Charts
- Clustered Bar Charts
- Tables

### Business Intelligence

- Interactive Reporting
- Executive Dashboard Design
- Financial Reporting
- Data Storytelling

---

# Analytical Workflow

```text
Public Expenditure Data
        │
        ▼
Data Import
        │
        ▼
Data Integration
        │
        ▼
Interactive Report Design
        │
        ▼
Department Analysis
        │
        ▼
Budget Monitoring
        │
        ▼
Expenditure Investigation
```

---

# Challenges & Limitations

| Challenge | Impact |
|------------|--------|
| Power Query transformations unavailable | Cannot document data preparation steps. |
| DAX measures unavailable | Measure definitions cannot be documented. |
| Semantic model unavailable | Relationships and schema cannot be verified. |
| KPI formulas unavailable | KPI calculations cannot be described. |

---

# Repository Structure

```text
Wake-County-Budget-Analysis/
│
├── PowerBI/
│   └── 4_5_final_solution.pbix
│
├── Dataset/
│   ├── Cost_Centers.csv
│   ├── Expenditures.csv
│   ├── Expenditure_Line_Items.csv
│   └── Funds.xlsx
│
├── Images/
│   ├── overview.png
│   ├── over-budget.png
│   ├── department-breakdown.png
│   └── expenditure-lines.png
│
└── README.md
```

---

# Dashboard Screenshots

```markdown
![Over Budget](images/over-budget.png)

![Department Breakdown](images/department-breakdown.png)

![Expenditure Lines](images/expenditure-lines.png)

![Dashboard Overview](images/overview.png)
```

---

# Tools & Technologies

- Power BI
- Power Query
- DAX
- Microsoft Excel
- CSV Data Sources

---

# What This Project Demonstrates

This project demonstrates the ability to develop an interactive Power BI dashboard for financial analysis using public expenditure data. It showcases skills in report design, interactive visualization, KPI reporting, departmental expenditure analysis, budget monitoring, and business-focused data storytelling. The report combines multiple datasets into a unified analytical solution that enables users to explore financial information at both executive and detailed levels while supporting informed budget oversight and expenditure analysis.
