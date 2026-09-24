# Retail Sales Performance Dashboard

## Project Overview

This project was completed as part of the **DataCamp Data Analyst in Power BI** learning path. It serves as a comprehensive retail sales analytics dashboard that consolidates concepts learned throughout the course into a single interactive business intelligence solution.

The report enables users to analyze retail sales performance from multiple perspectives, including products, retailers, revenue, profitability, returns, and overall business KPIs. It demonstrates the use of Power BI for data modeling, interactive reporting, and dashboard design.

---

# Business Problem

Retail organizations generate thousands of sales transactions across multiple products and retailers. Without an interactive reporting solution, it becomes difficult to:

- Monitor sales performance over time.
- Compare product performance.
- Evaluate retailer contribution.
- Identify profitable products.
- Analyze returned orders.
- Track business KPIs.

This dashboard centralizes these metrics into a single interactive report to support business decision-making.

---

# Project Objectives

The dashboard was designed to:

- Analyze retail sales performance.
- Monitor revenue and profitability.
- Compare product performance.
- Evaluate retailer performance.
- Explore individual sales transactions.
- Analyze returned orders.
- Visualize business KPIs.
- Provide interactive filtering across the report.

---

# Dataset

### Data Source

Microsoft Excel Workbooks

### Tables

| Table | Description |
|---------|-------------|
| Orders | Sales transactions (Fact Table) |
| Products | Product information |
| Retailers | Retailer information |
| Returns | Returned orders |

### Dataset Summary

| Table | Rows | Columns |
|---------|------|----------|
| Orders | 8,391 | 13 |
| Products | 1,210 | 7 |
| Retailers | 786 | 8 |
| Returns | 548 | 8 |

### Granularity

One record per sales transaction.

### Time Period

Verified order data begins in **2018**. Return records extend through **2021**.

---

# Data Preparation

## Verified

The report imports data from multiple Excel files.

The PBIX metadata available for this project does not expose the Power Query (M) transformation steps.

**Power Query transformations:** **Not Available**

---

# Data Model

The report follows a classic retail analytical model.

## Fact Table

- Orders

## Dimension Tables

- Products
- Retailers

## Supporting Table

- Returns

### Relationships

| From | To | Relationship |
|------|----|--------------|
| Orders.Product_SKU | Products.Product_SKU | Verified |
| Orders.Retailer_ID | Retailers.Retailer_ID | Verified |
| Returns.Order_ID | Orders.Order_ID | Verified |

The model represents a star-schema style analytical design centered around the Orders fact table.

---

# DAX Measures

The PBIX metadata available for analysis does not expose DAX expressions.

Verified DAX code:

**Not Available**

The report visually indicates the use of business measures including:

- Revenue
- Profit
- Profit Margin
- Sales
- Share Metrics
- KPI Measures

However, their DAX definitions cannot be verified from the available metadata.

---

# KPIs

| KPI | Definition | Business Meaning |
|------|------------|------------------|
| Revenue | Total sales revenue | Measures overall business sales |
| Profit | Total profit generated | Measures business profitability |
| Profit Margin | Profit relative to revenue | Evaluates operational efficiency |
| Share Metrics | Category or product contribution | Identifies contribution to overall business performance |

---

# Dashboard Structure

## 1. Order Details

### Purpose

Provides transaction-level analysis.

### Business Questions

- Which products were sold?
- Which retailers generated the sales?
- How do individual orders compare?

---

## 2. Product Comparison

### Purpose

Compares products across categories.

### Business Questions

- Which products perform best?
- Which categories generate the most sales?

---

## 3. Retailer Breakdown

### Purpose

Evaluates retailer performance.

### Business Questions

- Which retailers contribute the most revenue?
- Which retailers underperform?

---

## 4. Franchise Purchases

### Purpose

Compares franchise purchasing activity.

### Business Questions

- Which franchise retailers purchase the most products?
- How does purchasing vary across retailers?

---

## 5. Revenue and Profit

### Purpose

Analyzes business performance over time.

### Business Questions

- How has revenue changed?
- How has profitability evolved?
- Which periods performed best?

---

## 6. Shares

### Purpose

Visualizes contribution metrics.

### Business Questions

- Which products contribute the largest share?
- How is revenue distributed?

---

## 7. KPIs

### Purpose

Provides an executive summary of key business metrics.

### Business Questions

- Is the business performing well?
- Are KPIs improving over time?

---

# Visualizations

| Visual | Purpose |
|---------|----------|
| Table | Displays detailed order-level information |
| Scatter Chart | Explores relationships between sales metrics |
| Clustered Bar Chart | Compares products and retailers |
| Clustered Column Chart | Compares purchasing activity |
| Line Chart | Shows trends over time |
| Line & Clustered Column Chart | Compares multiple business metrics simultaneously |
| Pie Chart | Displays proportional contribution |
| Treemap | Highlights category contribution |
| Gauge | Monitors KPI progress toward targets |
| KPI Visual | Displays executive performance indicators |
| Cards | Shows important summary metrics |

---

# Filters & Interactions

Verified interactions include:

- Product slicers
- Category slicers
- Date slicers
- Cross-filtering
- Cross-highlighting
- Interactive report filtering

The following features could not be verified from the PBIX metadata:

- Drill-through
- Bookmarks
- Buttons
- Custom tooltips

---

# Key Insights

The dashboard enables users to:

- Identify top-performing products.
- Compare retailer performance.
- Monitor revenue and profitability trends.
- Analyze sales at the transaction level.
- Examine returned orders.
- Track overall business performance through KPIs.

Specific business findings cannot be verified without executing the report using live data interactions.

---

# Recommendations

The following are analytical recommendations based on the dashboard capabilities rather than measured outcomes.

- Monitor low-performing retailers for potential improvement opportunities.
- Focus marketing efforts on high-performing products.
- Investigate products with high return rates.
- Track profitability alongside revenue instead of relying solely on sales volume.
- Use interactive filtering to analyze seasonal sales patterns.

---

# Technical Skills Demonstrated

- Power BI Desktop
- Data Modeling
- Star Schema Design
- Interactive Dashboards
- KPI Development
- Business Intelligence Reporting
- Cross-filtering
- Slicers
- Time-Series Analysis
- Retail Sales Analytics
- Data Visualization
- Dashboard Design

---

# Challenges & Limitations

- Power Query transformation steps could not be verified from the PBIX metadata.
- DAX expressions are not accessible through the available metadata.
- Certain report interactions such as bookmarks and drill-through cannot be confirmed without opening the report in Power BI Desktop.

---

# Repository Structure

```
Retail-Sales-PowerBI-Dashboard/
│
├── Dashboard/
│   └── Retail Sales Performance Dashboard.pbix
│
├── Dataset/
│   ├── Orders.xlsx
│   ├── Products.xlsx
│   ├── Retailers.xlsx
│   └── Returns.xlsx
│
├── images/
│   ├── overview.png
│   ├── order-details.png
│   ├── product-comparison.png
│   ├── retailer-breakdown.png
│   ├── revenue-profit.png
│   ├── shares.png
│   └── kpis.png
│
└── README.md
```

---

# Dashboard Screenshots

> Add screenshots after exporting each report page.

```markdown
![Overview](images/overview.png)

![Order Details](images/order-details.png)

![Product Comparison](images/product-comparison.png)

![Retailer Breakdown](images/retailer-breakdown.png)

![Revenue & Profit](images/revenue-profit.png)

![Shares](images/shares.png)

![KPIs](images/kpis.png)
```

---

# Tools & Technologies

- Microsoft Power BI Desktop
- Power Query
- DAX
- Microsoft Excel
- Data Modeling
- Data Visualization

---

# What This Project Demonstrates

This project demonstrates the development of an interactive retail sales analytics dashboard using Power BI. It showcases practical skills in data modeling, business intelligence reporting, dashboard design, KPI development, and interactive data visualization. By integrating multiple related datasets into a unified analytical model, the project provides decision-makers with an efficient way to explore sales performance, retailer effectiveness, product contribution, and overall business trends.
