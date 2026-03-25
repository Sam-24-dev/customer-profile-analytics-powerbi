# Repo Setup Plan

## Objective

Prepare this project to become a portfolio-grade GitHub repository before any deeper improvement work starts.

This phase focuses on:

- choosing a professional repository name
- defining a clean folder structure
- deciding what should and should not be published
- documenting the move from the current academic delivery format to a portfolio format

## Recommended Repository Name

### Primary Recommendation

`customer-profile-analytics-powerbi`

Why this is the best option:

- clear business topic: customer profile analytics
- clear tool focus: Power BI
- cleaner and more professional than the current mixed-style name
- easy to read in GitHub, LinkedIn, CV, and portfolio cards

### Good Alternatives

- `customer-profile-dashboard-powerbi`
- `marketing-customer-analytics-powerbi`
- `customer-analytics-python-powerbi`

### Assessment of Current Name

Current local folder name:

`Customer-Profile-Analysis-PowerBI`

This is not bad, but it is not the strongest final name for a public portfolio project.

Main issues:

- mixed capitalization
- "analysis" is weaker than "analytics" for portfolio positioning
- it sounds more like a class folder than a polished case study

## Ownership Positioning

Because the original work came from a group bootcamp project, the public version should be positioned honestly as:

`Original project developed as part of a bootcamp group assignment. This repository contains my curated individual portfolio version, documentation, and presentation of the work.`

That gives you room to:

- present it as your portfolio project
- improve it under your own standards
- avoid sounding like you are hiding the group origin

## Target Repository Structure

```text
customer-profile-analytics-powerbi/
|-- .gitignore
|-- README.md
|-- LICENSE
|-- data/
|   |-- raw/
|   |   `-- marketing_raw.csv
|   `-- processed/
|       `-- marketing_clean.csv
|-- notebooks/
|   `-- 01_eda_preprocessing.ipynb
|-- dashboard/
|   `-- customer_profile_dashboard.pbix
|-- docs/
|   |-- REPO_SETUP_PLAN.md
|   |-- project_report.pdf
|   `-- portfolio_notes.md
|-- assets/
|   |-- dashboard-main.png
|   `-- dashboard-insights.png
`-- references/
    |-- bootcamp-deliverable-1.pdf
    `-- bootcamp-deliverable-final.pdf
```

## What Each Folder Is For

- `data/raw/`: original dataset, unchanged
- `data/processed/`: cleaned dataset used by Power BI
- `notebooks/`: Python notebook used for EDA, cleaning, and feature engineering
- `dashboard/`: final `.pbix`
- `docs/`: written documentation for project setup, report, and portfolio narrative
- `assets/`: screenshots and visual assets used in README or portfolio pages
- `references/`: optional academic or course documents kept for traceability

## Recommended File Renaming Map

Current file -> recommended file

- `Grupo3_PerfilCliente_EDA_Preprocesamiento (1).ipynb` -> `notebooks/01_eda_preprocessing.ipynb`
- `marketing_raw.csv` -> `data/raw/marketing_raw.csv`
- `presentacion_final (1).pbix` -> `dashboard/customer_profile_dashboard.pbix`
- `presentacion_final (1) (2) (1).pdf` -> `docs/dashboard_export.pdf`
- `INFORME_PBI.docx` -> `docs/project_report.docx`
- `Entregable I- Power BI-2.pdf` -> `references/bootcamp-deliverable-1.pdf`
- `Entregable Final- Power BI.pdf` -> `references/bootcamp-deliverable-final.pdf`

## What Should Be Public

Recommended to publish:

- final notebook
- raw dataset if redistribution is allowed
- processed dataset
- final `.pbix`
- dashboard screenshots
- README
- concise report or summary notes

Recommended not to feature prominently in the root:

- bootcamp instructions
- duplicate exports
- messy file names
- temporary outputs
- local scratch files

If you want, the academic PDFs can still be kept under `references/` without making them the center of the repo.

## Phase 1 Sequence

1. Rename the local project folder to the final repo name.
2. Create the professional folder structure.
3. Move and rename the current files into the new structure.
4. Add `.gitignore`.
5. Initialize Git locally.
6. Review the final tree and remove noise.
7. Create the GitHub repository with the same final name.
8. Push the cleaned project to GitHub.

## Publish Rules for This Phase

Before publishing, the repo should already satisfy these minimum conditions:

- no class-style file names in the root
- no temporary files
- no editor junk
- no duplicate exports in the main project path
- one clear dashboard file
- one clear notebook file
- one clear raw dataset location

## Recommended First Commit Scope

The first public commit should contain:

- the cleaned folder structure
- renamed files
- `.gitignore`
- the existing source materials organized into the right places

The first public commit should not try to include:

- deep data corrections
- major Power BI redesign
- final README polish
- public dashboard link

Those belong to the next phases.

## Decision for This Project

Recommended final repository name:

`customer-profile-analytics-powerbi`

Recommended action order:

1. finish repo structure
2. publish repo to GitHub
3. improve data logic and dashboard quality
4. add README, screenshots, and public Power BI link

## Definition of Done for Phase 1

Phase 1 is complete when:

- the repo has a professional name
- files are organized into clear folders
- `.gitignore` exists
- the project is ready to be pushed as a clean public repository

