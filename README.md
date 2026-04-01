# Data Jobs Dashboard - Power BI Project

[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)](https://www.microsoft.com/en-us/microsoft-365/excel)
[![Markdown](https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white)](https://www.markdownguide.org)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com)

## 📌 Overview

*Power BI Project - Data Jobs Dashboard* provides an analytical dashboard series built to map the **2024 data job market** examining role demand, compensation benchmarks, required skills, and geographic hiring patterns across real-world job postings. The project is structured as a deliberate progression across two dashboards:
1. **Data Jobs Dashboard 1.0** prioritizes analytical breadth, delivering a comprehensive report with **drill-through interactivity, detailed visualizations, and dynamic filtering** across job titles, platforms, and geographies.
2. **Data Jobs Dashboard 2.0** advances the work architecturally and analytically consolidating insights into a focused, measurement dashboard powered by a **star schema data model, explicit DAX measures, and structured Power Query transformations**, reflecting the design standards expected in professional BI environments.

## 📂 Repository Structure

```
Power-BI-Project_DataJobs
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

1. **Data Jobs Dashboard 1.0**
Data Jobs Dashboard 1.0 is a two-page comprehensive report designed to give a broad, navigable view of the 2024 data job market.      It prioritizes breadth of insight through interactive **filtering and drill-through capabilities**, making it suitable for exploratory analysis across multiple dimensions simultaneously.
    - **Page 1 – Market Overview:** High-level KPIs covering total job postings, yearly and hourly median salaries, job postings             distribution by month, and comparisons between yearly and hourly salaries of the job. Slicers allow filtering by job title.
    - **Page 2 – Drill-Through Detail:** A deeper, role-specific breakdown that users access by right-clicking any job title with             Drill-Through feature. Surfaces salary distributions, job locations, schedule type, and platform prevalence for the selected          role.

2. **Data Jobs Dashboard 2.0**
Data Jobs Dashboard 2.0 represents a single-page interactive dashboard using **DAX Measures** and **Power Query** to transforms data that delivers the most critical market data jobs. Focusing into job title, top required skills, salaries with dynamic comparisons between yearly and hourly compensation. Slicers also available to deep through each Job Title or Job Country, and **toggle metrics between counts and percentages**. 

## 🛠️ Power BI Techniques Reference

| Technique | Implementation |
|---|---|
| Data Transformation | Power Query (M Language), Append & Merge Queries, Advanced Transformations |
| Data Modeling | Star Schema (Fact & Dimension Tables), Table Relationships, Cardinality Management |
| DAX Measures | `CALCULATE`, `MEDIAN`, `DIVIDE`, `COUNTROWS`, `SELECTEDVALUE` |
| DAX Parameters | Dynamic measure switching between Count and Percentage |
| Visualizations | Bar Charts, Line Charts, Map Visuals, Matrix, Cards, Slicers |
| Interactivity | Drill-Through, Cross-Filtering, Bookmarks, Conditional Formatting |

## 💡 Key Findings Summary
 
- **Data Engineer Leads Both in Demand and Compensation:** Data Engineer postings represent the highest share of total listings in 2024 and simultaneously command the highest median salary both yearly and hourly compared to Data Scientist and Data Analyst roles. This dual dominance signals that the market is actively pricing specialized engineering skills, and that demand for data infrastructure talent has outpaced supply.
- **Python Is the Primary Salary Lever:** Python requirements are disproportionately concentrated in higher-compensated postings, establishing it as the key technical differentiator between entry-level and senior-level data roles. Candidates who extend beyond SQL into Python meaningfully expand both their addressable job market and their salary ceiling. 
- **SQL Is the Non-Negotiable Baseline:** SQL surfaces as a required skill across virtually every data role and seniority level, making it the single most consistent hiring signal in the dataset. Its near-universal presence positions SQL proficiency not as a differentiator, but as the minimum viable credential for market entry.
- **LinkedIn Still Tops Across Platforms:** LinkedIn lists account for the largest volume, the distribution across LinkedIn indicates that a single-channel job search strategy creates meaningful coverage gaps for both employers and candidates.

## 👤 About The Author

**Arruum Pratistha Kiranadjie**     
Data Analyst | Quantitative Analyst | Operations Research Analyst

Data-driven professional with a solid background in data analytics and quantitative research. Experienced in transforming complex datasets into actionable business insights using statistical methods, data visualization, and data modeling. Proven success leading end-to-end research projects across various industries. Passionate about leveraging data to drive strategic decisions and business growth.

- [LinkedIn: Arruum Kiranadjie](https://www.linkedin.com/in/arruumkiranadjie)
- [GitHub: Arruum Kiranadjie](https://github.com/arruumkiranadjie)
- [Tableau: Arruum Kiranadjie](https://public.tableau.com/app/profile/arruum.kiranadjie/vizzes)

© 2026 Arruum Kiranadjie. All rights reserved.
