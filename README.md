# Hospice Utilization & Payment Dashboard

## Overview

Power BI analysis of Medicare hospice utilization, payments, provider characteristics, and geographical patterns.

## Business Question

How does hospice utilization and payment vary across geography and provider characteristics?

## Data

- **Source:** Centers for Medicare & Medicaid Services (CMS)
- **Dataset:** Medicare Post-Acute Care Utilization — Hospice by Geography/Provider
- **Reporting year:** 2023
- **Level:** Hospice provider
- **Data type:** Public provider-level healthcare data
- **Source:** https://data.cms.gov/provider-data/topics/hospice-care
- Raw data is not included in this repository.

## Tools

- Power BI
- Power Query
- DAX
- GitHub

## Analysis

- Total hospice beneficiaries
- Total Medicare payments
- Total service days
- Average Medicare payment per beneficiary
- Top 10 states by hospice beneficiaries
- Top 10 states by Medicare payments
- Provider-level relationship between Medicare payments and service days
- State and summary-category filtering

## Dashboard
![Hospice Utilization Dashboard](screenshots/hospice_dashboard.png)

## Key Findings
- Hospice utilization and Medicare payments vary substantially across states.
- A small number of large providers account for substantially higher beneficiary volume and Medicare payments than many smaller providers.
- Provider service volume and Medicare payments show a broad distribution, with several large providers standing apart from the majority of providers.
- Interactive state and summary-category filters allow users to explore utilization patterns at a more granular level.

## Data Preparation

Data was prepared in Power Query before analysis. Steps included:

- Reviewed and standardized data types
- Renamed CMS field names for readability
- Prepared provider, beneficiary, payment, and utilization fields for analysis
- Preserved missing/suppressed CMS values rather than treating them as zero

## Limitations

This analysis uses publicly available provider-level CMS data and describes reported utilization and payment patterns. It does not establish causation or evaluate individual patient outcomes.

CMS data may contain suppressed or missing values for privacy and reporting purposes.

## Project Structure

- `Hospice_Utilization_Dashboard.pbix` — Power BI dashboard
- `screenshots/hospice_dashboard.png` — dashboard screenshot
- `README.md` - project documentation
