# Data Jobs Dashboard - Power BI Portfolio

[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
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
├── README.md                                                      ← README
│
├── dashboards                                                     ← Power BI Dashboard Files
│   ├── Data_Jobs_Dashboard_-_Arruum_Kiranadjie.pbix               ← Dashboard v1
│   └── Data_Jobs_Dashboard_2_0_-_Arruum_Kiranadjie_-_v2.pbix      ← Dashboard v2
│
└── images                                                         ← Source Data For This Project
    ├── Project1_Page1.png                                         ← Dashboard v1 Preview
    ├── Project1_Page2.png                                         ← Dashboard v1 Preview
    └── Project2_Page1.png                                         ← Dashboard v2 Preview
```

## 📊 Dataset

The Dataset is sourced from [Luke Barousse's Power BI for Data Analytics](https://drive.google.com/drive/folders/1DsLqC5OZt6fnUV8UksMhKnjWrNEG89xz) and consists of real-world **2024 Data Job Postings** scraped from major job platforms. It covers a wide range of data roles globally, including salary figures, required skills, work schedules, job posting date, and job platforms.

| Table | Description |
|---|---|
| `job_postings_flat` | Complete job posting attributes |
| `job_postings_monthly` | Multiple Excel sheet of job posting by month for time series analysis |
| `monthly_files` | Multiple Excel files of job posting by month for Power Query |
| `star_schema_files` | Multiple relational tables structured in a star schema for modeling |

## 🧠 Analyses

### Data Jobs Dashboard 1.0

Data Jobs Dashboard 1.0 is a two-page comprehensive report designed to give a broad, navigable view of the 2024 data job market. It prioritizes breadth of insight through interactive filtering and drill-through capabilities, making it suitable for exploratory analysis across multiple dimensions simultaneously.

- **Page 1 – Market Overview:** High-level KPIs covering total job postings, yearly and hourly median salaries, job postings distribution by month, and comparisons between yearly and hourly salaries of the job. Slicers allow filtering by job title.
- **Page 2 – Drill-Through Detail:** A deeper, role-specific breakdown that users access by right-clicking any job title with Drill-Through feature. Surfaces salary distributions, job locations, schedule type, and platform prevalence for the selected role.

### Data Jobs Dashboard 2.0

Data Jobs Dashboard 2.0 represents a single-page interactive dashboard using DAX Measures and Power Query to transforms data that delivers the most critical market data jobs. Focusing into job title, top required skills, salaries with dynamic comparisons between yearly and hourly compensation. Slicers also available to deep through each Job Title or Job Country, and toggle metrics between counts and percentages. 

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

## 👤 About The Author

**Arruum Pratistha Kiranadjie**     
Data Analyst | Quantitative Analyst | Operations Research Analyst

Data-driven professional with a solid background in data analytics and quantitative research. Experienced in transforming complex datasets into actionable business insights using statistical methods, data visualization, and data modeling. Proven success leading end-to-end research projects across various industries. Passionate about leveraging data to drive strategic decisions and business growth.

- [LinkedIn: Arruum Kiranadjie](https://www.linkedin.com/in/arruumkiranadjie)
- [GitHub: Arruum Kiranadjie](https://github.com/arruumkiranadjie)
- [Tableau: Arruum Kiranadjie](https://public.tableau.com/app/profile/arruum.kiranadjie/vizzes)

© 2026 Arruum Kiranadjie. All rights reserved.
