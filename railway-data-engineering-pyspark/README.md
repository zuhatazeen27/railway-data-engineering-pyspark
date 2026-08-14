# 🚆 Railway Data Engineering Pipeline using PySpark

<p align="center">

<b>PySpark</b> • <b>Python</b> • <b>Pandas</b> • <b>Matplotlib</b> • <b>Seaborn</b> • <b>Plotly</b> • <b>Google Colab</b>

</p>

<p align="center">

End-to-end railway data engineering and analytics project using PySpark for data processing, transformation, analysis, visualization, and reporting.

</p>

---

## 📌 Project Overview

This project demonstrates an end-to-end **Data Engineering and Analytics workflow using PySpark**.

The railway dataset is analyzed to identify:

- 🚆 Train operation patterns
- 🚉 Major source and destination stations
- 🛤️ High-frequency railway routes
- 📅 Day-wise train distribution
- 📊 Weekday vs weekend services
- 🔍 Station-level trends
- 💡 Operational insights and recommendations

The complete workflow transforms raw railway CSV data into meaningful analytical insights.

---

## ⚙️ Architecture / Workflow

```text
🚆 Railway CSV Dataset
          ↓
⚡ Data Loading using PySpark
          ↓
🔍 Data Exploration
          ↓
🧹 Data Cleaning
          ↓
⚙️ Data Transformation
          ↓
📊 Aggregation & Analysis
          ↓
📈 Visualization
          ↓
📋 Automated Reporting
          ↓
💡 Business Insights

---

## 📂 Dataset

The project uses railway train service information.

### Dataset Columns

| Column | Description |
|---|---|
| `Train_No` | Train number |
| `Train_Name` | Train name |
| `Source_Station_Name` | Starting station |
| `Destination_Station_Name` | Destination station |
| `days` | Operating day |

### Dataset Size

**11,113 railway records**

---

# 🔍 Level 1 — Data Exploration

## Task 1.1 — Load and Inspect Data

The railway dataset was loaded using PySpark.

Performed:

- Loaded the CSV dataset
- Displayed the first 10 records
- Inspected schema
- Checked data types
- Checked missing values

## Task 1.2 — Basic Statistics

Calculated:

- Total number of trains
- Unique source stations
- Unique destination stations
- Most common source station
- Most common destination station

## Task 1.3 — Data Cleaning

Performed:

- Missing-value identification
- Missing-value handling
- Station-name standardization
- Uppercase conversion
- Whitespace removal

---

# ⚙️ Level 2 — Data Transformation

## Task 2.1 — Data Filtering

Filtered railway data based on:

- Operating day
- Source station

Examples:

- Saturday trains
- Trains starting from `MADGOAN JN.`

## Task 2.2 — Grouping and Aggregation

Performed:

- Train count by source station
- Average trains per operating day
- Source-destination route aggregation

## Task 2.3 — Data Enrichment

Created a new `Train_Category` column.

```text
Monday - Friday   → Weekday
Saturday - Sunday → Weekend

---

# 📊 Level 3 — Advanced Data Analysis

## Task 3.1 — Pattern Analysis

Analyzed:

- Day-wise train distribution
- Frequent railway routes
- Major source stations
- Source-destination patterns
- Train operation trends

## Task 3.2 — Correlation Analysis

Calculated the correlation between day number and train count.

### Correlation Result

**0.3806**

This indicates a positive relationship between the day number and train count in the analyzed dataset, although the relationship is not strong.

---

# 📈 Level 4 — Visualization & Reporting

## Task 4.1 — Visualizations

Visualizations were created using:

- Matplotlib
- Seaborn
- Plotly

### 📊 Top 10 Source Stations

<img src="visualizations/top_source_stations.png" width="700">

### 📈 Day-wise Train Distribution

<img src="visualizations/day_wise_distribution.png" width="700">

### 🔥 Station vs Day Heatmap

<img src="visualizations/station_day_heatmap.png" width="700">

---

# 📋 Task 4.2 — Automated Reporting

A PySpark-based automated report was created containing:

- Dataset summary
- Station-level insights
- Day-wise train distribution
- Weekday vs weekend analysis
- Route analysis
- Correlation analysis
- Key insights
- Business recommendations
- Executive summary

### 📄 Detailed Report

[View Railway Data Engineering Report](reports/Railway_Data_Engineering_Report.md)

---

# 📊 Key Results

| Metric | Result |
|---|---:|
| Total Records | **11,113** |
| Total Unique Trains | **11,113** |
| Unique Source Stations | **921** |
| Unique Destination Stations | **924** |
| Top Source Station | **CST-MUMBAI** |
| Top Source Services | **513** |
| Top Destination Station | **CST-MUMBAI** |
| Top Destination Services | **514** |
| Weekday Services | **7,918** |
| Weekend Services | **3,195** |
| Most Frequent Route | **TAMBARAM → CHENNAI BEACH** |
| Top Route Services | **137** |
| Day/Train Correlation | **0.3806** |

---

# 🚉 Station Insights

### 🥇 Top Source Station

**CST-MUMBAI — 513 train services**

### 🥇 Top Destination Station

**CST-MUMBAI — 514 train services**

CST-MUMBAI acts as a major railway hub within the analyzed dataset.

---

# 🛤️ Route Analysis

### Most Frequent Route

**TAMBARAM → CHENNAI BEACH**

**137 services**

Other high-frequency routes identified include connections involving:

- CST-MUMBAI
- PANVEL
- RAVLI JN
- CHENNAI BEACH
- TAMBARAM

---

# 📅 Day-wise Train Distribution

| Day | Train Services |
|---|---:|
| Monday | 1,503 |
| Tuesday | 1,628 |
| Wednesday | 1,612 |
| Thursday | 1,526 |
| Friday | 1,649 |
| Saturday | 1,593 |
| Sunday | 1,602 |

### Highest

**Friday — 1,649 trains**

### Lowest

**Monday — 1,503 trains**

---

# 📊 Weekday vs Weekend

| Category | Train Services |
|---|---:|
| Weekday | **7,918** |
| Weekend | **3,195** |

The dataset shows significantly more train services during weekdays compared with weekends.

---

# 💡 Key Insights

- 🚉 **CST-MUMBAI** is the most frequent source station.
- 🚉 **CST-MUMBAI** is also the most frequent destination station.
- 🛤️ **TAMBARAM → CHENNAI BEACH** is the most frequent route identified.
- 📅 Train services are more concentrated during weekdays.
- 🚆 Major railway hubs account for a significant portion of train services.
- 📊 Day-wise analysis provides useful operational patterns.
- 🔄 Several high-frequency routes operate in both directions.
- 📈 The calculated day/train correlation is **0.3806**.

---

# 📌 Business Recommendations

### 1. Optimize Major Railway Hubs

Focus scheduling and infrastructure planning on high-traffic stations.

### 2. Improve Capacity Planning

Use day-wise train patterns for better resource and capacity planning.

### 3. Analyze High-Frequency Routes

Monitor high-frequency routes for potential scheduling optimization.

### 4. Evaluate Weekend Demand

Analyze passenger demand before increasing or reducing weekend services.

### 5. Support Infrastructure Planning

Use station-level and route-level analytics to identify locations that may require additional infrastructure.

---

# 🧰 Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming and analysis |
| PySpark | Data processing and transformation |
| Pandas | DataFrame conversion for visualization |
| Matplotlib | Bar and line charts |
| Seaborn | Heatmap visualization |
| Plotly | Interactive visualization |
| Google Colab | Development environment |

---

# 📁 Project Structure

```text
railway-data-engineering-pyspark/
│
├── 📁 data/
│   └── Railway_info.csv
│
├── 📁 notebooks/
│   └── Railway_Data_Engineering.ipynb
│
├── 📁 visualizations/
│   ├── top_source_stations.png
│   ├── day_wise_distribution.png
│   └── station_day_heatmap.png
│
├── 📁 reports/
│   └── Railway_Data_Engineering_Report.md
│
├── 📄 README.md
└── 📄 requirements.txt
