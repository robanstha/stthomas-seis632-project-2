# Project 2 – Global Connectivity & Economic Indicators Dashboard

## Overview
This repository contains a Power BI Project (`.pbip`) exploring relationships between GDP, Internet usage, and geographic distribution across countries from 1999–2022. It includes the semantic model, report definition, custom theme, datasets, and exported dashboard screenshots.

## Table of Contents
1. [Datasets](#datasets)
2. [Semantic Model](#semantic-model)
3. [Report & Pages](#report--pages)
4. [Screenshots](#screenshots)
5. [Custom Theme](#custom-theme)
6. [Repository Structure](#repository-structure)
7. [How to Open](#how-to-open)

## Datasets
Raw / prepared CSV files are in `datasets/`:
- `Final.csv` – Consolidated, cleaned dataset driving the report
- `GDP by Country 1999-2022.csv` – Original GDP time-series source

## Semantic Model
The model is defined in `Final_Project.SemanticModel/definition/` containing:
- `tables/` – Table metadata (`Country Table.tmdl`, `GDP.tmdl`, `InternetUsage.tmdl`, `Year Table.tmdl`)
- `relationships.tmdl` – Relationship definitions between fact & dimension tables
- `cultures/en-US.tmdl` – Localization / culture settings
- `model.tmdl` & `database.tmdl` – Core model configuration

## Report & Pages
The Power BI report definition is stored under `Final_Project.Report/definition/` with page JSON and visual JSON artifacts. Two primary pages are included:
1. Economic & Internet Usage Trends
2. Geographical Distribution

## Screenshots
Rendered dashboard pages (exported) are in `Dashboard screenshots/`.

### Economic & Internet Usage Dashboard
![Economic & Internet Usage Dashboard](Dashboard%20screenshots/GDP%20and%20Internet%20Usage%20dashboard.png)

### Geographical Distribution Page
![Geographical Distribution Page](Dashboard%20screenshots/Geographical%20Distribution%20page.png)

## Custom Theme
Custom theme JSON files:
- `assets/project2-theme.json` – Project-specific theme configuration
- `Final_Project.Report/StaticResources/RegisteredResources/UST_Minnesota_Brand_Theme9370718331472749.json` – Brand theme resource
- `Final_Project.Report/StaticResources/SharedResources/BaseThemes/CY25SU10.json` – Base theme reference

## Repository Structure
```
Final_Project.pbip                  # Entry point Power BI Project file
Final_Project.Report/               # Report definition & visuals
Final_Project.SemanticModel/        # Data model (tables, relationships)
datasets/                           # Source & prepared CSV datasets
assets/                             # Custom theme assets
Dashboard screenshots/              # Exported dashboard images
log.txt                             # (If used) Processing or refresh logs
```

## How to Open
1. Ensure you have the latest Power BI Desktop with Power BI Project (`.pbip`) support enabled.
2. Clone or download this repository.
3. Open `Final_Project.pbip` in Power BI Desktop.
4. If prompted, confirm data source settings (CSV files in `datasets/`).
5. Refresh to load model and visuals.

## Notes & Next Steps
- Additional pages or KPIs can be added by creating new page folders under `Final_Project.Report/definition/pages/`.
- Consider adding a data refresh script if moving to automated pipelines.
- If distribution is needed, export as `.pbix` or publish to Power BI Service.

## License / Usage
Educational use for SEIS632 coursework. Please attribute if reused.

---
Feel free to open issues or request enhancements.
