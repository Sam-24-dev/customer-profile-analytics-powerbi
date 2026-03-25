# Project Agent Guide

## Project

Customer Profile Analytics with Power BI

This repository is the public portfolio version of a bootcamp group project. Treat it as an individual, curated portfolio case study with transparent authorship and professional presentation.

## Current Goal

The active priority is Phase 2: data credibility and reproducibility.

Before any dashboard redesign or portfolio polish, the project must have:

- a validated preprocessing workflow
- a corrected analytical notebook
- a reproducible processed dataset
- alignment between notebook logic and Power BI outputs

## Public Positioning Rules

- Do not add academic PDFs or classroom deliverables to the public repository.
- Do not reintroduce messy file names, duplicate exports, or bootcamp-style submission artifacts.
- Keep the repository framed as a portfolio version of the original project, not as a hidden group submission.

## Repository Structure

- `data/raw/marketing_raw.csv`: original dataset, must stay unchanged
- `data/processed/`: generated clean dataset for analysis and Power BI
- `notebooks/01_eda_preprocessing.ipynb`: source notebook for EDA and cleaning
- `dashboard/customer_profile_dashboard.pbix`: public dashboard file
- `docs/`: planning notes and portfolio support files

## Working Rules

- Never edit `data/raw/marketing_raw.csv` directly.
- Any cleaned dataset must be generated into `data/processed/marketing_clean.csv`.
- Prefer fixing the analytical logic before editing Power BI visuals.
- Keep names consistent across notebook, dataset, dashboard, and README.
- Use concise business language instead of academic phrasing where possible.
- Avoid unsupported claims in documentation or dashboard text.

## Known Issues To Fix

- `education_2n Cycle` is currently omitted from the notebook reconstruction of `Education_Level`, which causes misclassification into `Basic`.
- The current public materials imply there are no duplicates and that all rows are unique customers; this must be validated and corrected before making that claim again.
- Notebook logic, dashboard narrative, and supporting notes are not fully aligned on the final business questions and KPI definitions.

## Phase 2 Deliverables

- audited notebook with corrected preprocessing logic
- explicit duplicate handling policy
- corrected categorical reconstruction logic
- `data/processed/marketing_clean.csv`
- synced KPI definitions for notebook and dashboard

## Preferred Skills and Tools

Prefer these skills when relevant:

- `jupyter-notebook`
- `python-patterns`
- `lint-and-validate`
- `verification-loop`
- `doc-coauthoring`

Prefer these tools when relevant:

- GitHub MCP for repository operations
- Chrome DevTools or Playwright for validating published dashboard flows

## Definition of Done for Phase 2

Phase 2 is complete only when:

- the notebook can justify every transformation
- the processed dataset is reproducible from the notebook
- the main data issues are resolved or explicitly documented
- the project is ready for dashboard refinement and README premium work
