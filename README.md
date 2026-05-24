# 🌍 Europe's Aging Population: A Data Visualization Project

This repository contains a data visualization project developed for the **Data Visualization** course as part of the MSc in Data Science at the **University of Milan-Bicocca (UNIMIB)**.

The project investigates Europe's demographic aging crisis through a rigorous end-to-end pipeline: from raw data acquisition on **Eurostat** to publication-quality charts built with **Python** and **Datawrapper**.

---

## 🎯 Project Objectives & Research Questions

The analysis is structured around three core research questions, each addressing a different dimension of the demographic phenomenon:

* **How old is Europe really getting?** Mapping the scale and geography of demographic aging across EU27 member states, tracing how the age structure has evolved over the past six decades.
* **What are the structural causes?** Investigating the two converging forces behind aging, falling fertility rates and rising life expectancy, and their combined "scissors effect" on the continent's demographic balance.
* **Can migration reverse the trend?** Assessing whether net migration flows are sufficient to compensate for the natural population deficit accumulating across the EU27.

---

## 🛠️ Tech Stack & Workflow

* **Python (`pandas`, `numpy`):** Data acquisition, cleaning, preprocessing and exploratory analysis across all 6 Eurostat datasets.
* **Python (`matplotlib`, `seaborn`):** Draft chart production for data verification and visual prototyping.
* **Python (`geopandas`):** Choropleth map generation for geographical pattern analysis.
* **Datawrapper:** Final publication-quality charts, styled for presentation use.
* **Canva and Powerpoint:** Slide layout and presentation design.

---

## 📊 Key Insights

* **Italy leads Europe** with a median age of **49.1 years** in 2025, the highest in the EU27, nearly 10 years above Ireland (39.6).
* **No EU27 country reaches the replacement threshold** of 2.1 children per woman. The EU27 average stands at just **1.45** in 2022  and has been below replacement since **1978**, 47 consecutive years.
* **Life expectancy gained +12 years** since 1960, reaching **80.9 years** on average in 2024. The gap between Spain (84.0) and Bulgaria (75.8) amounts to 8.2 years within the same Union.
* **20 out of 27 EU countries** record negative natural growth, deaths outnumber births. Migration has become the primary driver of population change across the continent.
* **Latvia** is the only EU27 country losing population from both directions simultaneously: negative natural growth (-7.4) and negative net migration (-2.5).

---

## 📂 Repository Structure

**`Data/`** — Raw Eurostat datasets and all processed outputs

- `europe_aging_analysis.ipynb` — Main notebook: data cleaning, EDA and chart generation
- `demo_pjanind_tabular.tsv` — Median age and dependency ratio by country *(Eurostat: demo_pjanind)*
- `demo_pjangroup_tabular.tsv` — Population by age group, used to build the population pyramid *(Eurostat: demo_pjangroup)*
- `demo_find_tabular.tsv` — Total fertility rate by country *(Eurostat: demo_find)*
- `demo_mlexpec_tabular.tsv` — Life expectancy at birth by country *(Eurostat: demo_mlexpec)*
- `demo_gind_tabular.tsv` — Natural growth and net migration rate *(Eurostat: demo_gind)*
- `spr_exp_pens_tabular.tsv` — Old-age pension expenditure as % of GDP *(Eurostat: spr_exp_pens)*

**`Data/Dataset1–6/`** — Cleaned long-format CSVs produced by the notebook, one folder per Eurostat dataset

**`Data/CSV_Datawrapper/`** — Chart-ready CSVs formatted for direct upload to Datawrapper

**`Data/Grafici_Draft/`** — Draft charts produced with Python (Matplotlib), used to verify data correctness before final styling

**`Grafici_Datawrapper/`** — Final publication-quality charts exported from Datawrapper, organised by chart topic

**`Final_project_data_viz.pdf`** — Final presentation slides in PDF format

---

## 📡 Data Sources

All data are drawn from **[Eurostat](https://ec.europa.eu/eurostat/databrowser/)**, the official statistical office of the European Union. Datasets were downloaded in May 2026 and are available under the **Eurostat open data licence**, which allows free reuse with attribution.

| Dataset | Description | Coverage |
|---|---|---|
| `demo_pjanind` | Median age, dependency ratio | EU27, 1960–2025 |
| `demo_pjangroup` | Population by 5-year age group | EU27, 1960–2023 |
| `demo_find` | Total fertility rate | EU27, 1960–2022 |
| `demo_mlexpec` | Life expectancy at birth | EU27, 1960–2024 |
| `spr_exp_pens` | Pension expenditure % GDP | EU27, 1990–2023 |
| `demo_gind` | Natural growth & net migration | EU27, 1960–2024 |

---

## 👤 Author

*Developed by **Andrea Porro** as part of the MSc in Data Science program at the **University of Milan-Bicocca (UNIMIB)**.*
