# 🚲 Bike Station Analytics (2022–2025)

> **Tools:** Power BI | Power Query | DAX | Data Modeling
> **Domain:** Transportation | Public Bike Sharing

## 🚲 Bike Station Analytics (2022–2025)

**Tools:**  
<img src="https://cdn.jsdelivr.net/npm/bootstrap-icons/icons/bar-chart-fill.svg" width="16"/> Power BI &nbsp; | &nbsp;
<img src="https://cdn.jsdelivr.net/npm/bootstrap-icons/icons/funnel-fill.svg" width="16"/> Power Query &nbsp; | &nbsp;
<img src="https://cdn.jsdelivr.net/npm/bootstrap-icons/icons/calculator-fill.svg" width="16"/> DAX &nbsp; | &nbsp;
<img src="https://cdn.jsdelivr.net/npm/bootstrap-icons/icons/diagram-3-fill.svg" width="16"/> Data Modeling  

**Domain:**  
<img src="https://cdn.jsdelivr.net/npm/bootstrap-icons/icons/bicycle.svg" width="16"/> Transportation | Public Bike Sharing

***

## 🧩 Project Overview

This project analyzes **bike station operations across multiple contracts (2022–2025)**, focusing on capacity utilization, availability patterns, geographic distribution, and service coverage. Using **Power Query and Power BI**, raw station-level data was cleaned, transformed, and visualized through interactive dashboards to support strategic fleet management and infrastructure planning.

***

## 🎯 Project Objectives

### 1. Analyze Capacity & Availability
Study docking capacity distribution and bike availability across contracts to identify high-utilization zones and excess capacity areas.

### 2. Evaluate Station Performance
Assess operational status (OPEN vs CLOSED) and measure station concentration across leading contracts.

### 3. Understand Geographic Coverage
Map station locations and analyze banking/card payment service rollout to identify accessibility gaps.

### 4. Compare Contract Performance
Benchmark bike availability against total capacity by contract to highlight balanced vs imbalanced operations.

### 5. Build Interactive Dashboards
Create dynamic **Power BI reports** with slicers for status, bonus features, and geographic exploration.

***

## 📂 Data Sources

**Source & Timeline:**
* 📊 *Bike Station Operations Dataset (2022–2025)*
* 🌐 *Public Bike Sharing Data*

**Domain:** Transportation (Public Bike Sharing)

***

## ❓ Problem Statement

* Analyze bike station capacity and availability trends from 2022–2025 across multiple contracts.
* Identify over-supplied vs under-supplied contracts through capacity-utilization analysis.
* Map geographic distribution and banking service coverage to uncover accessibility gaps.
* Evaluate OPEN vs CLOSED station performance and bonus station impact.
* Develop interactive dashboards for fleet management and infrastructure optimization.

***

## 🧾 Attribute Details

| **Attribute Name**          | **Data Type**    | **Description**                          |
| --------------------------- | ---------------- | ---------------------------------------- |
| Station No.                 | Integer          | Unique identifier for each bike station  |
| Contract Name               | Categorical      | City/contract area (Lyon, Valence, etc.) |
| Station Name                | Categorical      | Full name of the bike station            |
| Address                     | Categorical      | Street address/location description      |
| Latitude                    | Numeric (Decimal)| Geographic latitude coordinate           |
| Longitude                   | Numeric (Decimal)| Geographic longitude coordinate          |
| Banking                     | Boolean          | Supports bank card payments (TRUE/FALSE) |
| Bonus                       | Boolean          | Bonus station with incentives            |
| Bike Stands                 | Numeric          | Total docking capacity at station        |
| Available Bike Stands       | Numeric          | Empty docking slots available            |
| Available Bikes             | Numeric          | Bikes ready for rental                   |
| Status                      | Categorical      | Operational status (OPEN/CLOSED)         |
| Last Update (Year)          | Date             | Year from last update timestamp          |

***

## 🧹 Data Preprocessing Steps

1. **Data Collection:**
   Imported comprehensive bike station dataset with capacity, availability, and service attributes.

2. **Data Cleaning (Power Query):**
   Removed duplicates, handled null values, standardized data types, and renamed columns for clarity.

3. **Data Transformation:**
   Split position data into Latitude/Longitude, derived Last Update (Year), structured categorical fields.

4. **Filtering & Sorting:**
   Filtered invalid records and sorted by contracts/stations for optimal reporting.

5. **Data Integration:**
   Consolidated into single analysis-ready table for Power BI modeling.

***

## 🧮 Data Modeling & DAX (Power BI)

* **Model Design:**
  Implemented **star-style model** with main fact table (station metrics) and dedicated **Measures Table** for centralized DAX calculations.

### 📐 Key DAX Measures

* **Total Capacity** – Sum of all bike stands
* **Available Bikes** – Sum of rental-ready bikes
* **Available Stations** – Stations with available bike stands
* **Total Stations** – Distinct station count
* **Open Stations** – Count where Status = OPEN
* **Closed Stations** – Count where Status = CLOSED
* **Banking Enabled** – Stations with Banking = TRUE
* **Bikes in Use** – Total Capacity - Available Bike Stands
* **Occupancy Rate %** – (Bikes in Use / Total Capacity) × 100
* **Utilization Rate** – Available Bikes / Total Capacity

***

## 📊 Analysis & Visualizations

Created **interactive Power BI dashboards** featuring:

* Bar & Stacked Bar Charts
* Donut Charts
* KPI Cards
* Detailed Tables
* Interactive Maps
* Trend Line Charts

### 🔍 Dashboard Highlights

* **Capacity vs Availability:** Contract-level capacity distribution and bike availability trends
* **Station Status:** OPEN vs CLOSED station breakdown with slicers
* **Service Coverage:** Banking-enabled stations by top contracts
* **Geographic View:** Interactive map showing station locations
* **Performance Tables:** Top stations by availability and utilization
* **Trend Analysis:** Bike availability evolution (2022–2025)

* <img width="976" height="551" alt="Home" src="https://github.com/user-attachments/assets/9c29e5ed-5c1c-453f-840b-073987762f7e" />

***

## 📈 Performance Insights

* 🏙️ **Lyon, Valence, Bruxelles Capitale** dominate capacity and station counts.
* 🔄 **66% dock utilization** indicates healthy but imbalanced bike distribution.
* 💳 **Banking coverage concentrated** in top 5 contracts creates payment convenience gaps.
* 📍 **High-capacity contracts** operate near full occupancy while others show excess stands.
* 📈 **Upward availability trend** (2023–2025) signals expansion but risks under-utilization.
* 🎯 **Bonus stations** and geographic clustering reveal optimization opportunities.

***

## 🧠 Conclusion

**Power Query and Power BI** transformed raw bike station data into actionable insights for transportation planners. Key findings reveal contract imbalances, banking coverage gaps, and geographic concentration patterns. The interactive dashboard enables continuous monitoring of capacity utilization, service coverage, and operational performance to optimize fleet management and infrastructure investments.

***

## 👩‍💻 Author

**KUMAR C**
*Data Analyst | Power BI Developer*

* 🌐 GitHub: [Kumar C](https://github.com/kumar-c-git-hub)
* 💼 LinkedIn: [kumar C](https://www.linkedin.com/in/kumar-c/)
* 📧 Email: [kumarak04122021@gmail.com](mailto:kumarak04122021@gmail.com)

***

## 📚 Tags

`#PowerBI` `#BikeSharing` `#TransportationAnalytics` `#CapacityAnalysis`
`#DataVisualization` `#DAX` `#PowerQuery` `#GeospatialAnalytics`

***

Would you like me to adjust any specific sections, add placeholder images, or modify the technical emphasis for a particular audience (government transport authority, private operator, etc.)?
