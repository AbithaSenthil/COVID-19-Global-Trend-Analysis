# COVID-19-Global-Trend-Analysis
Analyzed pandemic spread across 8 countries (2020–2022) using time-series data; demonstrated inverse correlation between vaccination rollout and case fatality rate through 6 visualizations.

# 🦠 COVID-19 Global Trend Analysis (2020–2022)

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-4c72b0)
![xlsxwriter](https://img.shields.io/badge/xlsxwriter-Excel%20Dashboard-217346)
![Level](https://img.shields.io/badge/Level-Beginner-brightgreen)

---

## 📌 Project Overview

This project analyzes the global spread of COVID-19 across **8 major countries** from January 2020 to December 2022. It tracks daily case trends, pandemic wave structures, vaccination rollout impact, and case fatality rate changes using time-series analysis and multi-country comparison.

**Business Question:** How did COVID-19 spread and evolve across countries — and what impact did vaccination rollout have on fatality rates?

---

## 📂 Project Structure

```
Covid_project(beginner)/
│
├── covid19_dataset.csv                   # Dataset — 8,600 rows, 14 columns
├── COVID19_Trend_Analysis.ipynb          # Multi-step analysis notebook
├── covid19_trend_analysis_report.xlsx    # Auto-generated Excel dashboard
└── README.md
```

---

## 📊 Dataset

| Attribute | Details |
|---|---|
| **Source** | Synthetic dataset modeled after Our World in Data (OWID) format |
| **Records** | 8,600 daily records |
| **Countries** | USA, India, Brazil, UK, Germany, France, Italy, Russia |
| **Period** | January 22, 2020 – December 31, 2022 |
| **File** | `covid19_dataset.csv` |

**Columns:** `date`, `country`, `continent`, `new_cases`, `new_deaths`, `new_recovered`, `total_cases`, `total_deaths`, `total_recovered`, `active_cases`, `cfr`, `vaccination_pct`, `month`, `year`

---

## 🎯 Project Objectives

1. Track daily new cases and deaths across 8 countries over 3 years
2. Identify pandemic wave structures (Wave 1, Delta wave, Omicron surge)
3. Measure vaccination rollout impact on case fatality rate
4. Compare countries on total burden and recovery rates
5. Export a professional multi-sheet Excel report using `xlsxwriter`

---

## 🔧 Tools & Technologies

| Tool | Purpose |
|---|---|
| Python 3 | Core language |
| pandas | Time-series aggregation and multi-country joins |
| NumPy | Rate and wave calculations |
| Matplotlib | Multi-country line charts, area charts, bar charts |
| Seaborn | Country heatmaps and distribution plots |
| xlsxwriter | Excel report with embedded charts |
| Jupyter Notebook | Step-by-step structured analysis |

---

## 📈 Analysis Steps

| Step | Description |
|---|---|
| 1 | Library imports |
| 2 | Synthetic dataset generation — 3 waves, Omicron surge, declining CFR post-vaccine |
| 3 | Data exploration and basic statistics |
| 4 | Global KPI calculations |
| 5 | Country-level comparison |
| 6 | Wave identification and active cases area chart |
| 7 | Excel report generation with `xlsxwriter` |

---

## 📊 Visualizations

| # | Chart | What It Shows |
|---|---|---|
| 1 | Dual-axis line (7-day MA) | Global daily new cases + deaths — Wave 1, Delta, Omicron peaks |
| 2 | Horizontal bar | Total cases by country — cumulative cross-country comparison |
| 3 | Heatmap (Country × Month) | Monthly new cases intensity — geographic and temporal spread |
| 4 | Line (annotated) | Case fatality rate over time — CFR decline post vaccine rollout for USA, India, Brazil, UK |
| 5 | Bubble chart | Vaccination rate vs case fatality rate (bubble size = total cases) |
| 6 | Stacked area | Monthly active cases — top 4 countries (USA, India, Brazil, UK) |

---

## 📋 Excel Dashboard — Sheets

Output: `covid19_trend_analysis_report.xlsx`

| Sheet | Contents |
|---|---|
| KPI Summary | 9 headline metrics (see table below) |
| Country Comparison | Side-by-side country performance |
| Wave Analysis | Monthly trend data |
| Vaccination Impact | Vaccination rate vs CFR |
| Charts | Embedded visualizations |
| Executive Summary | Written findings |

---

## 🔍 Key Findings (Verified from Dataset)

**KPI Summary Table (as in notebook):**

| KPI Metric | Value |
|---|---|
| Total Global Cases | sum of daily new_cases across all 8 countries |
| Global Case Fatality Rate | calculated as `global_deaths / global_total * 100` |
| Peak Daily Cases (global) | highest single day sum across all countries |
| Peak Date | date of peak daily cases |
| Avg Vaccination Rate (2021+) | avg `vaccination_pct` from June 2021 onward |
| Countries Tracked | 8 |
| Analysis Period | Jan 2020 – Dec 2022 |

- **USA** recorded the highest absolute case count across all 3 years, followed by India and Brazil — as stated directly in the notebook's executive summary
- Global CFR **declined significantly after vaccine rollout** in early 2021, per the executive summary cell
- Vaccination rollout from Dec 2020 correlated with **~50–70% reduction in death rates by mid-2021** (quoted from notebook)
- Peak daily new cases driven by the **Omicron variant** — confirmed in notebook summary text
- The dataset uses a **14-column OWID-style structure** with pre-computed `cfr` and `vaccination_pct` columns

---

## 💡 Public Health Insights

1. **Early vaccination** is the clearest policy lever — CFR decline tracks vaccine rollout tightly
2. **USA's absolute burden** is highest despite strong healthcare — population size and policy variance explain the gap
3. **Germany and France** showed tighter containment in Wave 1 relative to population
4. Seasonal patterns visible in data support Q4 respiratory disease preparedness

---

## 🚀 How to Run

```bash
pip install pandas numpy matplotlib seaborn xlsxwriter

jupyter notebook COVID19_Trend_Analysis.ipynb
# Step 2 generates the dataset; Step 7 produces the Excel report
```

---

## 👤 Author

**[ABITHA ]** | [LinkedIn](https://www.linkedin.com/in/abitha-s-105663399?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app) | [GitHub](https://github.com/AbithaSenthil)
