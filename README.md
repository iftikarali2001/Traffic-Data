# California Traffic Collision Data Analysis (ETL Project)

## Project Overview

This project analyzes California traffic collision data using **Apache Spark** to process large-scale datasets.
The goal was to build a complete **ETL pipeline**, clean the data, and perform exploratory analysis to identify patterns in accident severity, time trends, geographic hotspots, and contributing factors.

The analysis reveals important traffic safety insights such as collision severity distribution, high-risk times, weather conditions, and demographic patterns.

---

## Dataset

The analysis uses four datasets:

* `case_ids`
* `collisions`
* `parties`
* `victims`

These datasets were originally provided as CSV files and processed using Spark DataFrames.

⚠️ **Note:**
The datasets are too large to upload to GitHub.
You can access them here:

**Dataset Link:** *(Add your Google Drive link here)*

---

## Project Workflow

### 1. Data Preparation

* Loaded CSV files into Spark DataFrames
* Enabled schema inference and headers
* Organized tables for easier processing

### 2. Data Cleaning

* Checked missing values across all tables
* Removed columns with excessive missing data
* Handled missing values using different strategies
* Removed duplicate records

### 3. Outlier Detection

Outliers were identified using the **IQR method**.

Examples of fixes:

* Invalid negative values removed
* Unrealistic ages capped
* Impossible vehicle years corrected
* Extremely large distance values capped

The goal was to **remove data entry errors while keeping realistic extreme events**.

### 4. Exploratory Data Analysis

Several analyses were performed, including:

* Collision severity distribution
* Weather conditions during collisions
* Victim age distribution
* Collision severity vs victims
* Lighting conditions impact
* Weekday collision trends
* Geographic distribution by county
* Collision trends over time

The visualizations highlight important traffic safety patterns.

---

## Key Findings

Some important insights from the analysis:

* Most collisions result in **property damage only**, but injury counts are still significant.
* **Young adults (20–30 years)** are the most affected age group.
* **Clear weather** has the most collisions due to higher traffic volume.
* **Friday** has the highest number of collisions.
* **5 PM (evening rush hour)** is the most dangerous time of day.
* High-population counties like **Los Angeles** show the highest collision counts.

---

## Business Insights

The analysis identifies several areas for improvement:

* Increased safety awareness during clear weather conditions
* Driver safety programs targeting younger drivers
* Better traffic management during weekday rush hours
* Improved lighting in high-risk areas
* Infrastructure improvements in high-collision counties

---

## Technologies Used

* Apache Spark (PySpark)
* Python
* Pandas
* Matplotlib / Visualization tools
* ETL Data Processing
* Big Data Analysis

---

## Project Structure

```
traffic-collision-analysis
│
├── report
│   └── ETL_Traffic_Data_Analysis_IFTIKAR_ALI.pdf
│
├── notebooks
│   └── analysis_notebook.ipynb
│
├── images
│   └── charts
│
└── README.md
```

---

## Author

**Iftikar Ali**

ETL / Data Analysis Project
California Traffic Collision Dataset
