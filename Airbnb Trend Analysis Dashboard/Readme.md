# Airbnb Trend Analysis Dashboard | Power BI

## Project Overview

This project presents an exploratory data analysis (EDA) and trend analysis dashboard built in Microsoft Power BI using Airbnb listing data. The report focuses on understanding data quality, exploring statistical distributions, analyzing temporal trends, identifying anomalies, and discovering the factors that influence Airbnb listing prices.

Unlike a traditional business dashboard, this report follows a data exploration workflow, gradually moving from data profiling and descriptive statistics to advanced analytical techniques such as Year-over-Year (YoY) analysis, anomaly detection, and AI-powered Key Influencers.

---

# Business Problem

Pricing and listing characteristics in the Airbnb marketplace are influenced by numerous factors including property features, host characteristics, and temporal trends. Before building predictive models or making business decisions, it is essential to understand:

- Overall data quality
- Statistical characteristics of the dataset
- Distribution of important variables
- Trends over time
- Seasonal patterns
- Anomalies within the data
- Key drivers affecting listing prices

This report provides an interactive environment for exploring these analytical questions.

---

# Project Objectives

- Assess dataset quality by identifying missing values.
- Explore descriptive statistics for numerical variables.
- Analyze the distribution of listing prices.
- Investigate engineered price transformations.
- Analyze host registration trends over time.
- Examine patterns across different days of the week.
- Compare Year-over-Year changes.
- Identify trends using time-series analysis.
- Detect unusual observations using Power BI anomaly detection.
- Discover which variables have the strongest influence on listing prices.

---

# Dataset

### Primary Dataset

**File:** `airbnb.csv`

### Dataset Characteristics

| Attribute | Details |
|-----------|---------|
| Dataset | Airbnb Listings |
| Records | 7,210 |
| Columns | 18 |
| Data Source | CSV File |
| Granularity | One record per Airbnb listing |

### Main Columns

- listing_id
- host_id
- host_since_datekey
- host_response_rate
- host_acceptance_rate
- host_is_superhost
- host_total_listings_count
- neighbourhood
- city
- latitude
- longitude
- property_type
- accommodates
- bedrooms
- price
- review_scores_rating
- instant_bookable
- listing_size_sqft

### Additional Dataset

A second dataset (`glassdoor.csv`) is included in the repository but is **not used** by this Power BI report.

---

# Data Preparation

The report includes data preparation prior to visualization.

Verified transformation:

- Engineered price values for analytical purposes (Modified Price).

Other Power Query transformations cannot be verified directly from the Power BI report metadata and therefore are not documented.

---

# Data Model

## Model Structure

The report primarily uses a single Airbnb dataset.

A date-based analytical structure is used for trend analysis.

### Relationships

Not Available.

---

# DAX Measures

The PBIX contains calculated measures supporting trend analysis and time intelligence. However, the exact DAX expressions cannot be extracted directly from the report.

Verified measures include:

| Measure | Purpose |
|----------|---------|
| Year-over-Year Change | Compare values between consecutive years |
| Time Trend Measures | Support trend analysis |
| Modified Price Measure | Analyze transformed price values |

Exact DAX formulas: **Not Available**

---

# KPIs

| KPI | Definition | Business Meaning |
|------|------------|------------------|
| Average Price | Average listing price | Understand overall pricing level |
| Price Distribution | Distribution of listing prices | Detect skewness and pricing variation |
| Host Growth | Number of hosts over time | Measure marketplace expansion |
| Year-over-Year Change | Annual comparison | Identify growth or decline |
| Time Trend | Trend over time | Detect long-term patterns |
| Price Influencers | AI-generated feature importance | Understand pricing drivers |
| Detected Anomalies | Automatically identified unusual observations | Highlight abnormal behavior |

---

# Dashboard Structure

## Page 1 — Missing

### Purpose

Evaluate dataset completeness.

### Business Questions

- Which variables contain missing values?
- How complete is the dataset?

---

## Page 2 — Describe

### Purpose

Provide descriptive statistics.

### Business Questions

- What are the average values?
- What are the minimum and maximum values?
- How much variability exists?

---

## Page 3 — Distribution

### Purpose

Analyze statistical distributions.

### Business Questions

- Is price normally distributed?
- Are there outliers?
- Is the data skewed?

---

## Page 4 — Modified Price

### Purpose

Analyze transformed pricing data.

### Business Questions

- How does transformed pricing improve analysis?
- Does feature engineering reduce skewness?

---

## Page 5 — Host Since Date

### Purpose

Analyze host growth over time.

### Business Questions

- How has Airbnb host registration changed?
- Are there periods of rapid growth?

---

## Page 6 — Day of Week

### Purpose

Analyze metrics by weekday.

### Business Questions

- Does listing activity differ by day?
- Are prices affected by weekdays?

---

## Page 7 — YoY Change

### Purpose

Compare annual performance.

### Business Questions

- How has performance changed year over year?
- Which years experienced growth or decline?

---

## Page 8 — Time Series

### Purpose

Visualize long-term trends.

### Business Questions

- Are there seasonal patterns?
- What long-term trends exist?

---

## Page 9 — Anomalies

### Purpose

Automatically detect unusual observations.

### Business Questions

- Which periods behave abnormally?
- Where should further investigation begin?

---

## Page 10 — Price Influencers

### Purpose

Identify the variables influencing listing prices.

### Business Questions

- Which features have the strongest impact on price?
- How do property characteristics affect pricing?

---

# Visualizations

## Tables

Used to summarize descriptive statistics and missing value information.

---

## Line Charts

Used to visualize temporal trends and Year-over-Year performance.

---

## Distribution Charts

Used to understand the statistical behavior of numerical variables.

---

## Box & Whisker Plot

Chosen to identify:

- Median
- Quartiles
- Outliers
- Distribution spread

---

## Time-Series Charts

Used for trend analysis across time.

---

## Key Influencers Visual

Power BI AI visual used to automatically identify variables with the greatest influence on listing prices.

---

## Anomaly Detection

Power BI AI feature used to automatically highlight unusual observations within time-series data.

---

# Filters & Interactions

Verified interactions include:

- Page-level filters
- Cross-filtering between visuals
- Interactive visual selections
- Time intelligence filtering

The following features cannot be verified from the report metadata:

- Drill Through
- Bookmarks
- Buttons
- Tooltips

---

# Key Insights

The report enables several important analytical observations:

- Missing value analysis helps identify data quality issues before modeling.
- Statistical summaries provide an overview of the dataset's characteristics.
- Price distribution analysis reveals the overall spread and variability of listing prices.
- Modified price analysis demonstrates the effect of feature engineering on skewed numerical data.
- Host registration trends provide insight into marketplace growth over time.
- Year-over-Year analysis highlights annual changes in key metrics.
- Time-series analysis reveals long-term behavioral trends.
- Anomaly detection automatically identifies observations that require further investigation.
- AI-powered Key Influencers help explain which features contribute most to listing price variation.

---

# Recommendations

Based on the analytical capabilities demonstrated in this report:

- Improve data quality by addressing missing values before predictive modeling.
- Investigate anomalies to determine whether they represent genuine business events or data quality issues.
- Continue monitoring long-term trends using time-series analysis.
- Use identified pricing drivers to support pricing strategy and market analysis.
- Incorporate additional business variables for deeper predictive analysis.

---

# Technical Skills Demonstrated

- Power BI
- Exploratory Data Analysis (EDA)
- Statistical Data Analysis
- Data Visualization
- Time-Series Analysis
- Year-over-Year Analysis
- Feature Engineering
- Data Profiling
- AI-Powered Analytics
- Anomaly Detection
- Key Influencers
- Interactive Reporting
- Business Intelligence

---

# Challenges & Limitations

- Exact Power Query transformation steps cannot be extracted from the PBIX metadata.
- DAX expressions are not directly accessible.
- Data model relationships cannot be fully verified.
- Report-level filters and interactions are only partially visible from metadata.
- The Glassdoor dataset is present but not utilized within this report.

---

# Repository Structure

```
Airbnb-Trend-Analysis-PowerBI/
│
├── Dashboard/
│   └── Trend Analysis in Power BI.pbix
│
├── Data/
│   ├── airbnb.csv
│   └── glassdoor.csv
│
├── Images/
│   └── dashboard-overview.png
│
└── README.md
```

---

# Dashboard Screenshot

> Replace the placeholder below with an exported screenshot of the report.

```text
images/dashboard-overview.png
```

```markdown
![Dashboard Overview](images/dashboard-overview.png)
```

---

# Tools & Technologies

- Microsoft Power BI Desktop
- Power Query
- DAX
- AI Visuals (Key Influencers)
- Anomaly Detection
- CSV Data Sources

---

# What This Project Demonstrates

This project demonstrates the ability to perform exploratory data analysis within Power BI by combining statistical profiling, distribution analysis, feature engineering, time-series analytics, AI-assisted insights, and interactive visualizations. It showcases practical skills in transforming raw data into meaningful analytical insights through Power BI's reporting, visualization, and built-in artificial intelligence capabilities.
