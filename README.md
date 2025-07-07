# Traffic Accident Analysis

This project presents an **Exploratory Data Analysis (EDA)** of traffic accident data to uncover key patterns related to **weather**, **road conditions**, **time of day**, and **contributing factors**. The analysis aims to support data-driven decision-making for improving traffic safety and reducing accident risks.

---

## Objective

To identify temporal and environmental conditions most associated with traffic accidents, examine contributing factors, and provide actionable insights using visualizations and aggregated data summaries.

---

## Data Cleaning

- Replaced unknown/unavailable values (`'UNKNOWN'`, `'UNAVAILABLE'`, etc.) with `NaN`
- Dropped rows with missing values in key columns (`weather_condition`, `lighting_condition`, `roadway_surface_cond`, `crash_hour`, `prim_contributory_cause`)
- Filled remaining missing values in select features with `'UNKNOWN'`
- Converted `crash_date` to datetime format for time-based analysis

---

## Visualizations

EDA was conducted using Python libraries like **Pandas**, **Seaborn**, and **Matplotlib**, including:

- **Barplots**: Distribution of accidents by:
  - Weather condition
  - Lighting condition
  - Roadway surface condition
  - Crash hour (time of day)
  - Traffic control devices
  - Primary contributory causes
- **Grouped Barplots**: Visualizing top causes under specific conditions (e.g., rain, dark lighting, wet road)
- **Attempted Geospatial Plot**: Accident hotspots (latitude/longitude data unavailable in this dataset)

---

## Summary

This project analyzed traffic accident data to uncover how **environmental conditions**, **time of day**, and **traffic infrastructure** relate to accident frequency and severity.

### Highlights

- **Saturday (Day 6)** had the highest accident count; **Sunday (Day 1)** had fewer but more **severe** crashes.
- Accidents were more frequent under **rainy weather**, **dark lighting**, and **wet road surfaces**.
- Major contributing factors in these conditions included:
  - `"UNABLE TO DETERMINE"`
  - `"FAILING TO YIELD RIGHT-OF-WAY"`
  - `"IMPROPER TURNING/NO SIGNAL"` (dark lighting)
  - `"FAILURE TO REDUCE SPEED"` (wet surfaces)
- **Traffic signals** and **stop signs** were the most common locations for accidents.
- **School zones**, **no passing zones**, and **pedestrian crossings** had **fewer accidents** but a **higher proportion of severe injuries**.
- **Hotspot visualization** was not possible due to **missing latitude and longitude data** in the dataset.

---

## Key Findings

### Environmental & Road Conditions
- Adverse conditions such as:
  -  Rainy weather  
  -  Dark lighting  
  -  Wet road surfaces  
  are strongly associated with a **rise in accident counts**.
- Frequent primary causes in these conditions:
  - `"UNABLE TO DETERMINE"`
  - `"FAILING TO YIELD RIGHT-OF-WAY"`
  - `"IMPROPER TURNING/NO SIGNAL"`
  - `"FAILURE TO REDUCE SPEED"`

### Time-Based Patterns
- **Day 6 (Saturday)** = highest accident count  
- **Day 1 (Sunday)** = fewer crashes but **higher average injuries**
- Accidents are more frequent in **evening/night hours**, especially under low-light conditions.

### Traffic Control Devices
- Highest number of accidents occurred at:
  - `"TRAFFIC SIGNAL"`
  - `"STOP SIGN/FLASHER"`
- Zones with **fewer accidents but higher injury rates**:
  - `"SCHOOL ZONE"`
  - `"NO PASSING"`
  - `"PEDESTRIAN CROSSING SIGN"`

### Accident Hotspot Mapping
- Hotspot mapping was **not performed** due to the **absence of latitude/longitude** data in the dataset.

---

## Files Included

- `task4.ipynb` – Jupyter Notebook with full EDA and visualizations
- `traffic_accidents.csv` – Input dataset (mounted from Google Drive)
- `README.md` – Project summary and documentation

---
# Dataset Source

The dataset used in this project is publicly available on Kaggle:

🔗 [Traffic Accidents Dataset – by oktayrdeki on Kaggle](https://www.kaggle.com/datasets/oktayrdeki/traffic-accidents?resource=download)

---

## Tools Used

- Python 3
- Pandas
- Seaborn
- Matplotlib
- Google Colab
---

Feel free to use or extend this project to build machine learning models or create interactive dashboards for policymakers!
