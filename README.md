# NYC Traffic Safety Analytics (2020)

## Project Overview
Analyzes NYC Motor Vehicle Collisions (2020) to identify **when, where, and why severe crashes occur**. Focus is on severity, risk prioritization, and actionable insights for public safety interventions.

## Problem Statement
City agencies face challenges:  

* Distinguishing high-impact crashes from minor incidents  
* Prioritizing locations, time windows, and behaviors for intervention  
* Avoiding reliance on aggregate counts that ignore injury/fatality risk  

**Core Question:**  
> How can NYC deploy enforcement and infrastructure resources effectively based on crash severity?

## Dataset
* **Source:** `NYC Accidents 2020.csv`  
* **Unit of Analysis:** Individual crash events  
* **Domain:** Urban safety / transportation risk  
* **Data Quality:** Missing values, inconsistent categories, uneven geographic coverage  

### Key Fields
| Field | Purpose |
|-------|---------|
| `CRASH_DATE` | Temporal trends & seasonality |
| `CRASH_TIME` | Hour-of-day and time-window risk |
| `BOROUGH` | Borough-level risk comparison |
| `LATITUDE`, `LONGITUDE` | Geospatial analysis & hotspot identification |
| `NUMBER_OF_PERSONS_INJURED` | Injury severity metric |
| `NUMBER_OF_PERSONS_KILLED` | Fatality severity metric |
| `CONTRIBUTING_FACTOR_VEHICLE_1` | Primary behavioral cause |
| `VEHICLE_TYPE_CODE_1` | Vehicle type in severe crashes |

## Analytical Approach
1. **Data Cleaning & Feature Engineering** – standardize fields, create severity flags  
2. **Severity-Centered Metrics** – prioritize crashes by impact  
3. **Risk Segmentation** – analyze by borough, time, and contributing factors  
4. **Spatial Prioritization** – identify high-severity clusters  

## Key Performance Indicators (KPIs)
* Injury Rate per Crash  
* Fatality Rate per 1,000 Crashes  
* Severe Crash Share  
* Borough Risk Index (severity-weighted)  
* Top Contributing Factors by Severity  

## Value Delivered
* Severity-weighted insights for operational decision-making  
* Prioritized risk signals for enforcement and infrastructure planning  
* Moves focus from crash frequency to where crashes cause the most harm  

## Skills Demonstrated
* Data cleaning & feature engineering  
* Severity-focused KPI design  
* Risk segmentation & geospatial analysis  
* Analytical storytelling for non-technical audiences  

## Next Steps
1. Engineer temporal and severity features  
2. Analyze borough-level and time-based risk  
3. Identify high-risk contributing factors & locations  
4. Visualize results for decision support
