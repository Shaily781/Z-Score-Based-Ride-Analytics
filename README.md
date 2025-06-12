## Z-Score-Based-Ride-Analytics  

A Power BI dashboard project analyzing ride booking behavior and efficiency across airport pickup points in Bangalore, segmented by peak and non-peak hours.

----
## 📌 Project Overview

AeroCab operates cab services from five major airport pickup points. To ensure service efficiency, the company wants to understand the ride booking flow and identify performance gaps between **peak** (5–9 AM, 6–11 PM) and **non-peak** hours.

This project includes:
- Full **ETL pipeline** in Power BI
- Analysis of booking efficiency metrics
- **Outlier detection** using Z-score analysis
- Filtering for normal vs. outlier-influenced data
- Custom dashboards to visualize and compare performance

---

## 🛠 ETL Process

1. **Extract:** Loaded raw ride data into Power BI  
2. **Transform:**
   - Calculated key metrics (ABT, ACT, ABOT)
   - Derived Z-scores for booking outcome time
   - Binned Z-scores into 0.20 ranges
   - Labeled Z-score > 2 as **“Outliers”** and <= 2 as **“Normal”**
3. **Load:** Created relationships and built dashboard visualizations

---

## 📊 Metrics Tracked

| Metric                     | Description |
|---------------------------|-------------|
| **Total Rides**           | Number of ride requests |
| **Confirmed Rides (%)**   | Booking success rate |
| **Unconfirmed Rides (%)** | Booking failures |
| **ABT**                   | Average Booking Time |
| **ACT**                   | Average Cancellation Time |
| **ABOT**                  | Average Booking Outcome Time |
| **Z-Score Binning**       | Grouped by 0.2 ranges to analyze outlier impact |

---

## 🔍 Key Insights

- **Peak Hour Efficiency:** Certain pickup zones show higher confirmation rates during peak hours.
- **Outlier Impact:** Outlier rides (Z > 2) significantly increase average booking outcome times.
- **Data Comparison:** Filtering out outliers improves visibility into operational norms.
- **Booking Gaps:** Zones with high unconfirmed rates may benefit from process redesign or staffing changes.

---

## 📊 Dashboard Features

- Ride KPIs filtered by:
  - Pickup Area
  - Peak vs Non-Peak
  - Outlier vs Normal Rides
- Distribution of Z-Score bins
- Visual filters for interactive comparisons
- Comparison view of metrics before and after removing outliers

---

## 🖼 Dashboard Preview

<img src="https://i.postimg.cc/BZ7sjvcC/Screenshot-2025-06-12-124618.png" alt="Dashboard Preview" width="850"/>
<img src="https://i.postimg.cc/1RFh3KXy/Screenshot-2025-06-12-124713.png" alt="Dashboard Preview" width="850"/>
<img src="https://i.postimg.cc/Yqy1DQNm/Screenshot-2025-06-12-124811.png" alt="Dashboard Preview" width="850"/>

---

## 🧰 Tools & Techniques

- **Power BI Desktop**
- **DAX (Data Analysis Expressions)**
- **Z-Score for Outlier Detection**
- **ETL Process Modeling**
- **KPI Cards, Line & Bar Charts, Filters**

---

## 📈 Business Value

- 🧠 Identify zones and hours with low booking success
- 🚫 Detect and analyze impact of anomalous bookings
- ⏱ Improve operational efficiency by targeting ABT, ABOT, and ACT
- 🗺 Optimize fleet resources based on peak-hour booking trends


