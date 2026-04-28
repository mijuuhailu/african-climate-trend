### 🌍 Climate Data Analysis using NASA POWER Dataset
##  Project Overview

This project presents a comprehensive data profiling, cleaning, and exploratory data analysis (EDA) of climate data obtained from the NASA Prediction Of Worldwide Energy Resources database.

The dataset contains daily meteorological observations for five African countries:

Ethiopia
Kenya
Sudan
Tanzania
Nigeria

covering the period January 2015 to March 2026.

The primary goal is to transform raw satellite-derived climate data into a clean and structured format, and to extract meaningful insights related to temperature, precipitation, humidity, and wind patterns.

##  Objectives
Perform data cleaning and preprocessing (handling missing values, duplicates, and outliers)
Convert raw time variables into proper datetime format
Conduct exploratory data analysis (EDA) to identify trends and patterns
Analyze seasonal variations in temperature and rainfall
Examine relationships between key climate variables
Prepare datasets for future predictive modeling
##  Dataset Description

Each dataset contains daily observations with the following key variables:

Column	Description
YEAR	Year of observation
DOY	Day of year (converted to date during preprocessing)
T2M	Mean temperature (°C)
T2M_MAX	Maximum temperature (°C)
T2M_MIN	Minimum temperature (°C)
T2M_RANGE	Temperature range (°C)
PRECTOTCORR	Precipitation (mm/day)
RH2M	Relative humidity (%)
WS2M	Wind speed (m/s)
WS2M_MAX	Maximum wind speed (m/s)
PS	Surface pressure (kPa)
QV2M	Specific humidity (g/kg)

##  Methodology
# 1. Data Cleaning
Replaced -999 with NaN
Removed duplicate records
Handled missing values using forward-fill and row filtering
Converted YEAR and DOY into a proper datetime column
Extracted monthly features for seasonal analysis
# 2. Exploratory Data Analysis (EDA)
- Time Series Analysis
Monthly average temperature trends
Monthly total precipitation patterns
Identification of seasonal cycles
- Correlation Analysis
Heatmaps to identify relationships between variables
Scatter plots to explore key interactions
- Distribution Analysis
Histograms of precipitation (including log transformation)
Bubble charts showing interaction between temperature, humidity, and rainfall
# 3. Outlier Detection
Applied Z-score method (|Z| > 3)
Retained or capped extreme values due to their environmental significance

 # Key Insights
 
* Clear seasonal patterns observed across all countries
* Rainfall distribution is highly skewed, with infrequent extreme events
* Strong correlations exist among temperature variables
* Temperature and humidity exhibit inverse relationships in some regions
* Climate variability differs across countries, highlighting regional diversity

# Cross-Country Climate Vulnerability Analysis

A comparative analysis was conducted across all five countries to evaluate relative climate vulnerability based on:

### Temperature trends
Rainfall variability
Extreme heat frequency
Consecutive dry days
### Key Findings
Sudan recorded the highest average temperature and the greatest number of extreme heat days
Tanzania and Nigeria exhibited the highest precipitation variability
Sudan experienced the highest number of annual dry days, indicating severe drought exposure
Ethiopia showed moderate climate conditions but notable rainfall variability

Statistical testing using one-way ANOVA confirmed that temperature differences across countries were statistically significant (p < 0.05).


##  Tools & Technologies
Python
Pandas
NumPy
Matplotlib
Seaborn
SciPy
Jupyter Notebook
