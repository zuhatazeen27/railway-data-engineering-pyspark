# 🚆 Railway Data Engineering Pipeline using PySpark

## 📌 Project Overview

This project is an end-to-end **Railway Data Engineering and Analytics project** built using **PySpark**.

The project analyzes railway operational data to identify train patterns, major railway hubs, high-frequency routes, day-wise train distribution, and weekday versus weekend operations.

The complete workflow covers data loading, data quality checking, cleaning, transformation, aggregation, advanced analysis, visualization, and automated reporting.

---

## 🛠️ Technologies Used

- 🐍 Python
- ⚡ PySpark
- 🐼 Pandas
- 📊 Matplotlib
- 🎨 Seaborn
- 📈 Plotly
- ☁️ Google Colab

---

## 🏗️ Project Workflow

```text
Railway CSV Dataset
        ↓
Data Loading using PySpark
        ↓
Data Exploration
        ↓
Data Quality & Null Checking
        ↓
Data Cleaning
        ↓
Data Transformation
        ↓
Aggregation & Analysis
        ↓
Pattern Analysis
        ↓
Visualization
        ↓
Automated Reporting
        ↓
Business Insights

---

## 📂 Dataset

The dataset contains railway train service information.

### Dataset Columns

| Column | Description |
|---|---|
| `Train_No` | Train number |
| `Train_Name` | Train name |
| `Source_Station_Name` | Starting station |
| `Destination_Station_Name` | Destination station |
| `days` | Operating day |

---

# 🔍 Level 1: Data Exploration

### Task 1.1 – Load and Inspect Data

- Loaded the railway CSV dataset using PySpark.
- Displayed the first 10 records.
- Inspected schema and data types.
- Checked missing values.

### Task 1.2 – Basic Statistics

Calculated:

- Total number of trains
- Unique source stations
- Unique destination stations
- Most common source station
- Most common destination station

### Task 1.3 – Data Cleaning

- Checked for missing values.
- Handled missing values.
- Standardized station names using uppercase formatting.
- Removed unnecessary spaces from station names.

---

# ⚙️ Level 2: Data Transformation

### Task 2.1 – Data Filtering

Filtered trains based on:

- Operating day
- Source station

Example:

- Saturday trains
- Trains starting from MADGOAN JN.

### Task 2.2 – Grouping and Aggregation

Performed:

- Train count by source station
- Average trains per operating day
- Source-destination route aggregation

### Task 2.3 – Data Enrichment

Created a new `Train_Category` column:

```text
Monday-Friday → Weekday
Saturday-Sunday → Weekend

---

# 📊 Level 3: Advanced Data Analysis

### Task 3.1 – Pattern Analysis

Analyzed:

- Day-wise train distribution
- Frequent railway routes
- Major source stations
- Train operation patterns

### Task 3.2 – Correlation Analysis

Calculated the correlation between the day number and train count.

**Correlation: 0.3806**

This indicates a moderate positive relationship between the day number and train count in this dataset.

---

# 📈 Level 4: Visualization & Reporting

## Task 4.1 – Visualizations

Created visualizations using Matplotlib, Seaborn, and Plotly.

### 📊 Top Source Stations

![Top Source Stations](visualizations/top_source_stations.png)

### 📈 Day-wise Train Distribution

![Day-wise Distribution](visualizations/day_wise_distribution.png)

### 🔥 Station vs Day Heatmap

![Station Day Heatmap](visualizations/station_day_heatmap.png)

An interactive Plotly visualization was also created for the top source stations.

---

# 📋 Task 4.2 – Automated Reporting

Created an automated PySpark-based report containing:

- Dataset summary
- Station-level insights
- Day-wise train distribution
- Weekday vs weekend analysis
- Route analysis
- Correlation analysis
- Key insights
- Business recommendations
- Executive summary

📄 **Detailed Report:**  
`reports/Railway_Data_Engineering_Report.md`

---

# 📊 Key Results

| Metric | Result |
|---|---:|
| Total Records | 11,113 |
| Total Unique Trains | 11,113 |
| Unique Source Stations | 921 |
| Unique Destination Stations | 924 |
| Top Source Station | CST-MUMBAI |
| Top Source Services | 513 |
| Top Destination Station | CST-MUMBAI |
| Top Destination Services | 514 |
| Weekday Services | 7,918 |
| Weekend Services | 3,195 |
| Most Frequent Route | TAMBARAM → CHENNAI BEACH |
| Top Route Services | 137 |
| Day/Train Correlation | 0.3806 |

---

# 💡 Key Insights

- **CST-MUMBAI** is the most frequent source and destination station.
- **TAMBARAM → CHENNAI BEACH** is one of the highest-frequency routes.
- Train services are more concentrated on weekdays.
- Major railway hubs account for a significant portion of train services.
- Day-wise analysis helps identify operational patterns.
- Several high-frequency routes operate in both directions.

---

# 📌 Business Recommendations

- Optimize scheduling at high-traffic railway stations.
- Use day-wise trends for better capacity planning.
- Analyze high-frequency routes for service optimization.
- Evaluate weekend demand before increasing services.
- Prioritize infrastructure planning around major railway hubs.

---

# 📁 Project Structure

```text
Railway_Data_Engineering_Project/
│
├── data/
│   └── Railway_info.csv
│
├── notebooks/
│   └── Railway_Data_Engineering.ipynb
│
├── visualizations/
│   ├── top_source_stations.png
│   ├── day_wise_distribution.png
│   └── station_day_heatmap.png
│
├── reports/
│   └── Railway_Data_Engineering_Report.md
│
├── README.md
└── requirements.txt```


# 🚀 How to Run

### 1. Install the required libraries

```bash
pip install -r requirements.txt
### 2. Open the notebook

Open:

`notebooks/Railway_Data_Engineering.ipynb`

The notebook can be executed using Google Colab or another PySpark-compatible environment.

---

# 🎯 Project Objective

The objective of this project is to demonstrate an end-to-end **PySpark data engineering workflow** using railway data, from data loading and cleaning to transformation, analysis, visualization, and reporting.

---

## 👩‍💻 Skills Demonstrated

- PySpark
- Python
- Data Cleaning
- Data Transformation
- Data Aggregation
- Data Analysis
- Data Visualization
- Statistical Analysis
- Automated Reporting
- Business Insights

---

## ⭐ Project Highlight

Built an end-to-end PySpark data engineering pipeline processing **11,113 railway records**, performing data quality checks, transformations, aggregations, pattern analysis, visualizations, and automated reporting to derive actionable railway operational insights.