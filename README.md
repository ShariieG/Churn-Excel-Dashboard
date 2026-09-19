# Churn-Excel-Dashboard
# Databel Customer Churn Analysis

An Excel-based analysis of customer churn for Databel, a telecom provider. The
project turns a flat export of 6,687 customer records into a self-service
workbook that surfaces where churn is happening and why — by contract type,
tenure, geography, and stated reason for leaving.

<img width="1451" height="853" alt="image" src="https://github.com/user-attachments/assets/0cc1bf70-a5b6-4af5-9982-926912b1586f" />


## Headline numbers

| Metric | Value |
|---|---|
| Total customers | 6,687 |
| Churned customers | 1,796 |
| Overall churn rate | 26.9% |
| Month-to-month churn rate | 46.3% |
| Two-year contract churn rate | 2.8% |
| Highest-churn state | California (61.8%) |

## What's in the workbook

`data/Databel_Churn_Analysis.xlsx` contains:

- **Databel - Customer** — the customer-level source table (6,687 rows, 29 columns:
  usage, billing, plan, demographics, and churn outcome), converted to a
  structured Excel Table.
- **Databel - Aggregate** — a derived table with formula-driven segmentation:
  - `Demographics`: nested `IF()` bucketing customers into Under 30 / Senior / Other
  - `Grouped Consumption`: nested `IF()` bucketing average monthly GB download into
    Less than 5GB / Between 5–10GB / 10+ GB
- **Churn Analysis** / **Customer Analyses** — 10 PivotTables and 9 PivotCharts
  breaking churn down by contract type, age group, data usage, state, and
  stated churn reason.
- **Overview** — a one-page executive dashboard consolidating the headline KPIs
  and the top charts, so the story is visible without digging through tabs.

## Key findings

- **Contract length is the strongest churn driver.** Month-to-month customers
  churn at 46.3%, versus 11.3% for one-year and 2.8% for two-year contracts —
  a ~17x gap between the extremes.
- **Churn risk rises sharply with age/tenure.** Customers aged 79–88 churn at
  43.8%, roughly double the rate of customers under 29 (22.0%).
- **Geography is uneven.** California sits at 61.8% churn, more than double the
  national average, with several other states above 35%.
- **Competitive pressure dominates stated reasons.** "Competitor made better
  offer" and "competitor had better devices" together account for about a
  third of all stated churn reasons, with support experience close behind.

## Tools & techniques

Excel Tables · nested `IF()` formulas for segmentation · PivotTables · PivotCharts ·
one-page dashboard design

## Author

Sharon Galela
