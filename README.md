# Insurance Claims Analytics & Fraud Risk Assessment | Power BI

An interactive, three-page Power BI report exploring insurance claim costs, fraud patterns, policy coverage, customer demographics, and vehicle-related claims.

## Dashboard Preview

### 1. Insurance Claims Overview
![Insurance Claims Overview](screenshots/page-1.png)

### 2. Fraud Analysis & Risk Assessment
![Fraud Analysis](screenshots/page-2.png)

### 3. Customer & Vehicle Claim Analysis
![Customer and Vehicle Analysis](screenshots/page-3.png)

## Project Overview

The report analyzes **1,000 insurance claims** with a combined claim amount of approximately **52.76M**. It highlights monthly claim activity, differences across policy coverage levels, fraud concentrations, and customer and vehicle claim patterns.

## Tools & Skills

- **Power BI Desktop** — interactive dashboards and report design
- **DAX** — calculated measures and KPIs
- **Power Query** — data preparation
- **Data visualization** — bar, column, line, and donut charts
- **Business analysis** — interpreting claims and fraud patterns

## Dashboard Pages

| Page | Focus |
| --- | --- |
| Claims Overview | Total claims, claim amount, average claim amount, fraud rate, monthly trends, policy coverage and slicers |
| Fraud Analysis | Fraud distribution, fraud rates by incident type, severity and policy coverage |
| Customer & Vehicle Analysis | Average claim amount by age, claims by gender and education, average vehicle claim by manufacturer |

## Key Insights

- **1,000 claims** total approximately **52.76M** in claim amounts.
- The overall reported **fraud rate is 24.7%** (247 claims).
- Claim volume decreased from **516 in January to 472 in February**, a decrease of approximately **8.5%**.
- **100/300** policy coverage has the highest total claim amount, approximately **19.29M**.
- **Major Damage** incidents under **250/500** policy coverage show a fraud rate of approximately **64.9%**.
- The **60–69 age band** has the highest displayed average claim amount, approximately **63K**.
- **Ford** has the highest displayed average vehicle claim amount, approximately **41K**.

## Interactive Features

The Power BI report includes slicers for **month**, **gender**, **policy coverage**, and **fraud status**. The PDF is a static preview; open the `.pbix` file in Power BI Desktop to explore the interactive report.

## Files

- [`Insurance_Claims_Analytics.pbix`](Insurance_Claims_Analytics.pbix) — Power BI report
- [`Insurance_Claims_Dashboard.pdf`](Insurance_Claims_Dashboard.pdf) — exported dashboard preview
- [`screenshots/`](screenshots/) — page previews used in this README

## How to Open

1. Download or clone the repository.
2. Open `Insurance_Claims_Analytics.pbix` using **Microsoft Power BI Desktop**.
3. Explore the three report pages and use the slicers to filter the visuals.

## Notes

This is a portfolio/learning project. Figures reflect the included report and are not live insurance-industry statistics. The original data source and licensing details should be added if the dataset is distributed separately.


## Dataset files and cleaning

The `data/` directory contains the original uploaded insurance dataset and a separately prepared cleaned version, both in CSV and Excel formats.

**Cleaning performed for the provided portfolio dataset:**
- Preserved all 1,000 original claim records and the original 39 source columns.
- Trimmed leading/trailing whitespace from text fields.
- Converted `?` placeholders and blank categorical values to `Unknown` (including missing `authorities_contacted` entries).
- Standardized `incident_date` and `policy_bind_date` to `YYYY-MM-DD`.
- Retained numeric measurements, claim amounts, and fraud flags without artificial imputation.
- Confirmed the total claim amount (52,761,940) and fraudulent claim count (247) remain unchanged.

**Important:** This cleaned export was prepared separately from the uploaded CSV. It is not a verified export of the exact Power Query transformation history embedded in the `.pbix` report. The report's data source path may need updating after cloning.

**Dataset attribution:** Original file supplied with the Power BI training exam (LMS). Review redistribution permissions before publishing this repository publicly.
