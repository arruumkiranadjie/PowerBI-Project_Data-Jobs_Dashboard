# Data Jobs Dashboard - Power BI Portfolio

[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![DAX](https://img.shields.io/badge/DAX-F2C811?style=for-the-badge)]()
[![Power Query](https://img.shields.io/badge/Power_Query-217346?style=for-the-badge)]()
[![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)](https://www.microsoft.com/en-us/microsoft-365/excel)
[![Markdown](https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white)](https://www.markdownguide.org)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com)

## 📌 Overview

*Power BI Portfolio - Data Jobs Dashboard* is a two-part dashboard series built as the **Final Project** of [Luke Barousse's Power BI for Data Analytics Course](https://www.lukebarousse.com/courses). The dashboards explore real-world **2024 data science job postings**, translating raw hiring data into actionable workforce intelligence across roles, salaries, skills, and locations.

The portfolio consists of two versions, each applying a distinct design philosophy and data modeling approach:

- **v1 – Data Jobs Dashboard:** A comprehensive two-page report featuring a broad market overview with drill-through interactivity and dynamic filtering across job titles, platforms, and geographies.
- **v2 – Data Jobs Dashboard 2.0:** A refined single-page dashboard focused on delivering streamlined, high-signal insights using advanced DAX measures and a star schema data model for improved performance and scalability.

Together, they demonstrate end-to-end proficiency across the full Power BI workflow — from raw data ingestion and transformation in **Power Query**, to relational modeling, to expressive visualization design and DAX-driven analytical depth.

## 📂 Repository Structure

```
Power-BI-Portfolio_DataJobs
│
├── README.md                                              ← README
│
├── dashboards                                             ← Power BI Dashboard Files
│   ├── Data_Jobs_Dashboard_-_Arruum_Kiranadjie.pbix              ← v1
│   └── Data_Jobs_Dashboard_2_0_-_Arruum_Kiranadjie_-_v2.pbix    ← v2
│
└── src                                                    ← Source Data For This Project
    └── data
        ├── job_postings_flat.csv                          ← Single flat table format
        ├── job_postings_monthly.xlsx                      ← Monthly breakdown (multi-sheet)
        ├── monthly_files/                                 ← Individual monthly Excel files
        └── star_schema_files/                             ← Normalized star schema tables
```

## 📊 Dataset

The dataset is sourced from [Luke Barousse's Power BI for Data Analytics Course](https://www.lukebarousse.com/courses) and consists of real-world **2024 data science job postings** scraped from major job platforms. It covers a wide range of data roles globally, including salary figures, required skills, work schedules, and job platforms.

| Table / File | Description |
|---|---|
| `job_postings_flat.csv` | Single denormalized table containing all job posting attributes |
| `job_postings_monthly.xlsx` | Multi-sheet Excel file organized by month for time series analysis |
| `monthly_files/` | Individual monthly Excel files for folder-based batch import in Power Query |
| `star_schema_files/` | Normalized relational tables structured as a star schema for v2 modeling |

## 📈 Dashboards

### v1 — Data Jobs Dashboard

The first dashboard is a **two-page comprehensive report** designed to give a broad, navigable view of the 2024 data job market. It prioritizes breadth of insight through interactive filtering and drill-through capabilities, making it suitable for exploratory analysis across multiple dimensions simultaneously.

**Key Features:**
- **Page 1 – Market Overview:** High-level KPIs covering total job postings, median salaries, job platform distribution, and top hiring locations. Slicers allow filtering by job title, country, schedule type, and work-from-home status.
- **Page 2 – Drill-Through Detail:** A deeper, role-specific breakdown that users access by right-clicking any job title. Surfaces salary distributions, top required skills, and platform prevalence for the selected role.
- **Interactive Filtering:** Cross-visual filtering and slicers enable dynamic exploration without page navigation.

### v2 — Data Jobs Dashboard 2.0

The second dashboard represents a deliberate evolution — trading breadth for precision. It is a **single-page focused dashboard** that delivers the most critical market signals in a clean, consolidated layout. The underlying data model was also redesigned to reflect professional-grade Power BI architecture.

**Key Features:**
- **Streamlined Single-Page Layout:** All core insights are surfaced on one page, prioritizing clarity and reducing cognitive load for the end user.
- **Advanced DAX Measures:** Explicit measures are used throughout for median salary calculations, percentage breakdowns, and dynamic metric switching via parameters.
- **Star Schema Data Model:** Data is structured into fact and dimension tables (`dim_jobs`, `dim_skills`, `dim_companies`, `fact_postings`), improving query performance, model maintainability, and scalability.

## 🛠️ Power BI Techniques Reference

| Technique | Implementation |
|---|---|
| Data Transformation | Power Query (M Language), Append & Merge Queries, Advanced Column Transformations |
| Data Modeling | Star Schema (Fact & Dimension Tables), Table Relationships, Cardinality Management |
| DAX Measures | `CALCULATE`, `MEDIAN`, `DIVIDE`, `COUNTROWS`, `SELECTEDVALUE` |
| DAX Parameters | Dynamic measure switching via `SWITCH(TRUE(), ...)` pattern |
| Visualizations | Bar Charts, Line Charts, Map Visuals, Matrix, Cards, Slicers |
| Interactivity | Drill-Through, Cross-Filtering, Bookmarks, Conditional Formatting |
| Report Design | Themed Layout, Custom Formatting, Tooltip Pages |

## 💡 Key Findings Summary

- **Data Analyst is the Highest-Volume Role:** Data Analyst postings dominate the 2024 job market by volume, though Data Engineer and Data Scientist roles command significantly higher median salaries.
- **SQL is the Universal Skill:** SQL appears as a required skill across virtually every data role, reinforcing its position as the baseline technical requirement for entering the data field.
- **Python Separates Junior from Senior Roles:** Python requirements are concentrated in higher-paying roles, suggesting it is a key differentiator for salary progression within data careers.
- **Remote Work Remains Prevalent:** A substantial portion of data job postings continue to offer remote or hybrid flexibility, particularly for senior-level positions.
- **Platform Diversity Matters:** Job postings are distributed across multiple platforms, with LinkedIn and company-direct postings accounting for the largest share of listings.

## 🚀 How to Open the Dashboards

To explore the dashboards, you will need **Power BI Desktop** installed on your machine (free to download from [Microsoft](https://powerbi.microsoft.com/desktop/)). Once installed, simply download the `.pbix` files from the `dashboards/` folder and open them directly in Power BI Desktop. If prompted with an "Enable Content" dialog, click to allow data connections.

Should you encounter data source errors after opening, navigate to **Home → Transform Data → Data Source Settings**, update the file paths to point to your local copy of the `src/data/` folder, and refresh the model.

## 👤 About The Author

**Arruum Pratistha Kiranadjie**  
Data Analyst | Quantitative Analyst | Operations Research Analyst

Data-driven professional with a solid background in data analytics and quantitative research. Experienced in transforming complex datasets into actionable business insights using statistical methods, data visualization, and data modeling. Proven success leading end-to-end research projects across various industries. Passionate about leveraging data to drive strategic decisions and business growth.

- [LinkedIn: Arruum Kiranadjie](https://www.linkedin.com/in/arruumkiranadjie)
- [GitHub: Arruum Kiranadjie](https://github.com/arruumkiranadjie)
- [Tableau: Arruum Kiranadjie](https://public.tableau.com/app/profile/arruum.kiranadjie/vizzes)

© 2026 Arruum Kiranadjie. All rights reserved.
