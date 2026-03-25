# Customer Profile Analytics Dashboard

<div align="center">

![Python 3.x](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Data Cleaning](https://img.shields.io/badge/Data-Cleaned-success?style=for-the-badge)
![Mobile Layout](https://img.shields.io/badge/Mobile-Optimized-0A66C2?style=for-the-badge)

<br>

[![Open live dashboard in Power BI](https://img.shields.io/badge/Live_Dashboard-Open_in_Power_BI-1E40AF?style=for-the-badge&logo=powerbi&logoColor=white)](https://app.powerbi.com/view?r=eyJrIjoiNzE3YmU3ZDktN2M3Yi00ODY5LTk2OTktOGI0NmE3YmU1ZDdiIiwidCI6ImI3YWY4Y2FmLTgzZDgtNDY0NC04NWFlLTMxN2M1NDUyMjNjMSIsImMiOjR9&pageName=b29252d974b9cb52bd7f)

</div>

---

## Project Overview

This repository contains the portfolio version of a customer analytics project developed with Python and Power BI. The goal was to transform a raw marketing dataset into a reproducible analytical pipeline and a polished interactive dashboard that explains how customer demographics, household composition, tenure, and channel behavior influence spending patterns.

This public version focuses on:
- a validated preprocessing workflow in Python
- a clean and reproducible analytical dataset
- a Power BI dashboard optimized for desktop and mobile viewing
- business-facing storytelling suitable for GitHub, LinkedIn, and portfolio use

> This project originated from a bootcamp group assignment and is presented here as an individually curated portfolio case study.

---

## Challenge / Solution / Impact

| Challenge | Solution | Impact |
|---|---|---|
| Raw marketing data with duplicated rows and inconsistent categorical logic | Built a reproducible preprocessing notebook and exported a validated clean dataset | Reliable KPIs and defensible segment-level analysis |
| Dashboard originally tied to an outdated local Excel source | Reconnected the Power BI model to the cleaned CSV generated from the notebook | Portfolio-ready workflow aligned with repository artifacts |
| Academic presentation style did not fit a professional analytics portfolio | Redesigned the report into executive pages with desktop and mobile layouts | Sharper storytelling for recruiters and hiring managers |

---

## Key Metrics

| Metric | Value |
|---|---|
| Customers analyzed | 2,021 |
| Total spend | 1,139,418 |
| Average income | 51,687.26 |
| Average ticket | 44.86 |
| High-value customers | 25.0% |
| Average premium spend share | 16.1% |

---

## Dashboard Scope

The final Power BI report is organized into four premium pages:

1. **Executive Overview**  
   High-level KPIs and the main customer spending patterns.

2. **Customer Segments**  
   Comparison of value and spending across education, marital status, and household composition.

3. **Behavior & Channels**  
   Purchase activity, digital behavior, and tenure patterns by customer group.

4. **Insights & Recommendations**  
   A concise business summary supported by the most relevant visuals.

The report also includes mobile-optimized layouts for key pages in Power BI.

---

## Analytical Workflow

```text
marketing_raw.csv
        |
        v
01_eda_preprocessing.ipynb
        |
        v
marketing_clean.csv
        |
        v
customer_profile_dashboard.pbix
        |
        v
Published Power BI dashboard
```

---

## Tech Stack

| Layer | Technologies |
|---|---|
| Data preparation | Python, pandas, Jupyter Notebook |
| Data output | CSV |
| Visualization | Power BI Desktop, Power BI Service |
| Delivery | Publish to web link + GitHub repository |

---

## Repository Structure

```text
customer-profile-analytics-powerbi/
|- dashboard/
|  `- customer_profile_dashboard.pbix
|- data/
|  |- raw/
|  |  `- marketing_raw.csv
|  `- processed/
|     `- marketing_clean.csv
|- docs/
|  `- data_processing_spec.md
|- notebooks/
|  `- 01_eda_preprocessing.ipynb
|- assets/
|- AGENTS.md
|- .gitignore
`- README.md
```

---

## How to Use

### 1. Review the preprocessing workflow
Open [01_eda_preprocessing.ipynb](./notebooks/01_eda_preprocessing.ipynb) to inspect the cleaning logic, derived features, and export steps that generate the analytical dataset.

### 2. Inspect the cleaned data
Use [marketing_clean.csv](./data/processed/marketing_clean.csv) as the validated analytical source for downstream reporting.

### 3. Open the Power BI dashboard
Open [customer_profile_dashboard.pbix](./dashboard/customer_profile_dashboard.pbix) in Power BI Desktop to explore the report locally, or use the public dashboard link above to view the published version.

---

## Key Insights

- Customers with higher education levels concentrate the largest share of total spending, especially `Graduation`, `PhD`, and `Master` segments.
- Households without children allocate a higher proportion of spend to premium products.
- More established customers generate higher purchase volume than recent customers.
- Store purchases remain important across age groups, while digital activity still shows meaningful differences by segment.
- High-value customers represent roughly one quarter of the customer base, making them a strong target for retention and premium positioning.

---

## Documentation

- Data cleaning and modeling rules: [data_processing_spec.md](./docs/data_processing_spec.md)
- Reproducible preprocessing notebook: [01_eda_preprocessing.ipynb](./notebooks/01_eda_preprocessing.ipynb)

---

<div align="center">

### Author

**Samir Caizapasto**  
*Data Analyst / Junior Data Engineer*

[![Visit portfolio website](https://img.shields.io/badge/Portfolio-Visit_Website-success?style=for-the-badge&logo=vercel&logoColor=white)](https://portafolio-samir-tau.vercel.app/)
[![Connect on LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/samir-caizapasto/)
[![Contact by email](https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:samir.leonardo.caizapasto04@gmail.com)

</div>

---

If this project was useful or interesting, consider starring the repository.
