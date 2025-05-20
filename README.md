# 🦠 COVID-19 Vaccination Impact Analysis (Dec 2020 – June 2022)

## 📊 Project Overview  
This project investigates the relationship between COVID-19 **vaccination coverage** and **case trends** across U.S. states from **December 17, 2020 to June 16, 2022**. The analysis integrates **SQL (SQLite)**, **Excel**, and **Power BI** to assess the effectiveness of vaccination efforts.

---

## 📅 Why These Dates?  
The analysis starts on **December 17, 2020**, when COVID-19 vaccines first rolled out in the U.S., and ends on **June 16, 2022**, before updated boosters and variant-specific vaccines became widespread. This timeframe captures the early vaccine impact during major variant waves like Alpha, Delta, and Omicron, includes policy responses and booster campaigns, and marks the shift from emergency pandemic response to endemic management.

---

## 🛠 Tools & Workflow

- **SQL (SQLite via DBeaver)**  
  Cleaned and joined case/vaccine datasets using custom SQL queries; used joins, subqueries, filtering, and aggregation.  
- **Excel**  
  Exported SQL query results to CSV and imported to Power BI.  
- **Power BI**  
  Built interactive dashboards and visualizations; applied DAX calculations and slicers.  
- **Data Sources**  
  - [CDC Case Surveillance](https://data.cdc.gov/)  
  - [CDC Vaccination Data](https://github.com/CDCgov/)  
  - [U.S. Census Bureau](https://www.census.gov/)

---

## 🎯 Project Goal  
To determine whether **higher vaccination rates** were associated with **lower COVID-19 case growth**, especially in the **top 5 most populous states**:  
- California  
- Texas  
- Florida  
- New York  
- Pennsylvania  

---

## 📌 Vaccination Threshold  
A **70% fully vaccinated** threshold was used, based on **WHO** recommendations for herd immunity levels.

---

## 📈 Key Findings

- States with **higher vaccine coverage** tended to have **slower growth in new COVID-19 cases**.  
- States with **early and sustained vaccination efforts** (like CA and NY) showed more favorable trends.  
- Variants, public health policies, and population density were also influential.

---

## 🧮 SQL Operations Summary

- ✅ **Joins**  
  Combined `clean_covid_cases` and `clean_vaccinations` using `state` and `date_updated` to create a unified dataset (`covid_joined`) for export to Excel and Power BI.  
- ✅ **Subqueries**  
  Used for threshold detection (e.g., states surpassing 70% full vaccination) and aggregated comparisons.  
- ✅ **Filtering & Aggregation**  
  Applied `WHERE`, `GROUP BY`, `ORDER BY`, and `SUM()` to extract key metrics by state and date.

---

## 📂 File Descriptions

| File Name                     | Description                               |
|-------------------------------|-------------------------------------------|
| `SQL Scripts`                 | SQL queries for table creation and joins  |
| `README.md`                   | Project documentation (this file)         |
| `covid_joined.csv`            | Final cleaned dataset for Power BI import |
| `covid_cases_raw.csv`         | Raw COVID-19 case data                    |
| `covid_vaccinations_raw.csv`  | Raw vaccination data                      |
| `powerbi_dashboard.pbix`      | Power BI interactive report/dashboard     |

---

## 📬 Contact  
Feel free to reach out with feedback or collaboration ideas!
