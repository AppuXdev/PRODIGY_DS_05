# Task 5: US Traffic Accidents Analysis

## Objective
Analyze US traffic accident data to identify patterns related to road conditions, weather, time of day, and visualize accident hotspots and contributing factors.

## Dataset
- **Source**: Kaggle - US Accidents Dataset
- **Download Link**: [US Accidents Dataset - Kaggle](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents)
- **File Used**: US_Accidents_March23.csv
- **Records**: 100K+ accidents analyzed
- **Key Columns**: Severity, Start_Time, Weather_Condition, State, City, Sunrise_Sunset, Road Features

> **Note**: The dataset file is too large for GitHub (>100MB). Please download it from Kaggle using the link above and place `US_Accidents_March23.csv` in the project folder before running the notebook.

## Files in Repo
- `accident.ipynb` - Complete EDA notebook with all analysis and visualizations
- 'accident.py'
- `README.md` - Project documentation

## Methodology
1. **Data Preprocessing**
   - Converted Start_Time to datetime, extracted Hour/Day/Month features
   - Handled missing values in critical columns
   
2. **Exploratory Analysis**
   - **Time Patterns**: Accidents by hour, day of week, day vs night
   - **Geographic Hotspots**: Top states and cities by accident count
   - **Weather Impact**: Accident frequency and average severity by condition
   - **Road Features**: Impact of Junction, Crossing, Roundabout, Traffic_Signal on severity

3. **Visualization**
   - Bar charts for hotspots and weather conditions
   - Time series patterns for hourly/daily trends
   - Feature impact analysis showing severity difference

## Key Results

### Accident Hotspots
- **Top State**: California (CA) - highest accident count by large margin
- **Top Cities**: Los Angeles, Sacramento, San Diego, San Jose

### Time Patterns
- **Peak Hours**: 7-9 AM and 4-6 PM during commute times
- **Day of Week**: Weekdays show higher volume than weekends

### Weather & Severity
- **Most Frequent**: Clear weather - most driving occurs in clear conditions
- **Highest Severity**: Fog, snow, rain correlate with increased average severity

### Contributing Road Features
**Increase Severity:**
- Junction: +0.154 avg severity
- Railway: +0.062 avg severity
- No_Exit: +0.033 avg severity

**Decrease Severity:**
- Roundabout: -0.448 avg severity
- Give_Way: -0.436 avg severity
- Traffic_Signal, Stop, Amenity: All reduce severity

## Tech Stack
`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn` `Jupyter Notebook`

## How to Run
1. **Download Dataset**: Get `US_Accidents_March23.csv` from [Kaggle](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents)
