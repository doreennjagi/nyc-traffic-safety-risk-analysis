# NYC Traffic Safety Analytics (2020)

## Project Overview
Analyzes NYC Motor Vehicle Collisions (2020) to identify **where, why, and which factors drive severe crashes**. Focus is on **severity, risk prioritization, and actionable insights** for city agencies to make **data-driven safety interventions**.

## Problem Statement
City agencies face persistent challenges:  

- Distinguishing high-impact crashes from minor incidents  
- Prioritizing locations, behaviors, and vehicle types for intervention  
- Avoiding reliance on raw counts that ignore injury/fatality risk  

**Core Question:**  
> How can NYC **deploy enforcement and infrastructure resources effectively** based on crash severity?

### Gap Addressed
- Existing data is descriptive — agencies know where crashes occur, but **not where they cause the most harm**  
- No severity-weighted view of contributing factors, vehicles, or locations  
- Limited prioritization for **resource allocation and policy action**  

---

## Dataset
- **Source:** `NYC Accidents 2020.csv`  
- **Unit of Analysis:** Individual crash events  
- **Domain:** Urban safety / transportation risk  
- **Data Quality Challenges:** Missing values, inconsistent categorical entries, uneven geographic coverage  

### Key Fields
| Field | Purpose |
|-------|---------|
| `CRASH_DATE` | Temporal trends & seasonality |
| `BOROUGH` | Borough-level risk segmentation |
| `LATITUDE`, `LONGITUDE` | Geospatial analysis & hotspot identification |
| `NUMBER_OF_PERSONS_INJURED` | Injury severity metric |
| `NUMBER_OF_PERSONS_KILLED` | Fatality severity metric |
| `CONTRIBUTING_FACTOR_VEHICLE_1` | Primary behavioral cause |
| `VEHICLE_TYPE_CODE_1` | Vehicle type in severe crashes |
| `ON_STREET_NAME` / `CROSS_STREET_NAME` | Street-level risk prioritization |

> **Note:** Time-of-day analysis skipped due to missing `CRASH_TIME` values. Focus remains on **severity-weighted insights**.

---

## Analytical Approach
1. **Data Cleaning & Feature Engineering**  
   - Standardized columns and cleaned coordinates  
   - Created **severity flags** (`INJURY_FLAG`, `FATALITY_FLAG`) and a **weighted `SEVERITY_SCORE`**

2. **Severity-Centered Metrics**  
   - Prioritized crashes by injury/fatality impact rather than frequency  

3. **Risk Segmentation**  
   - Analyzed **boroughs, streets, contributing factors, and vehicle types** by severity  

4. **Spatial Prioritization & Visualization**  
   - Generated **hotspot maps** and top streets to highlight high-impact locations  

---

## Key Performance Indicators (KPIs)
- **Injury Rate per Crash** – injuries normalized per incident  
- **Fatality Rate per 1,000 Crashes** – normalized lethality measure  
- **Severe Crash Share** – % of crashes with ≥1 injury or fatality  
- **Borough Risk Index** – severity-weighted comparison across boroughs  
- **Top Contributing Factors & Vehicle Types by Severity** – behavioral and vehicle risks  
- **Top Streets / Hotspots** – recurring high-severity locations  

---

## Value Delivered
- Moves beyond descriptive statistics to **severity-weighted insights**  
- Provides **prioritized risk signals** for enforcement and infrastructure planning  
- Answers **where crashes cause the most harm**, not just where they occur  

---

## Skills Demonstrated
- Data cleaning & feature engineering for **messy, real-world datasets**  
- Severity-focused KPI design and **risk segmentation**  
- Geospatial analysis and hotspot visualization  
- Analytical storytelling tailored for **policy and operational decision-makers**  

---

## Next Steps / Extensions
1. Integrate additional years for trend analysis  
2. Explore external factors (weather, traffic volume) to refine risk segmentation  
3. Develop **interactive dashboards** for city planners  
4. Extend to **predictive modeling** for proactive safety interventions  
