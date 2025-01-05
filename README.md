# Data Cleaning and EDA with Time Series Data

# Household Power Consumption Data Analysis

This notebook analyzes household power consumption data, focusing on data cleaning, visualization, and correlation analysis.  The goal is to understand patterns in energy usage and identify potential relationships between different power metrics.

## Data Source

The dataset used in this analysis is the "Individual household electric power consumption" dataset, which can be found at [link to data source if available]


## Data Cleaning and Preprocessing

1. **Datetime Conversion:** Combined 'Date' and 'Time' columns into a 'Datetime' column and converted it to the appropriate datetime datatype.

2. **Data Type Conversion:** Converted all numeric columns to appropriate numeric types using `pd.to_numeric`, handling errors using `errors='coerce'`.

3. **Missing Data Handling:** Addressed missing data points using mean imputation for each numeric column.  Alternative methods like interpolation could be considered depending on the specific insights desired.


## Data Visualization

Several visualizations were created to understand patterns in the data:

* **Line plots of raw data:** Shows the raw power consumption over time but with noise due to missing data.
* **Monthly averages:** Provides a smoothed view of the yearly trend in power consumption, helpful for identifying seasonality and long-term trends.
* **30-day moving averages:** Captures shorter-term trends and fluctuations, smoothing out daily noise.


## Correlation Analysis

A correlation matrix and scatter matrix visualization help to understand the relationships between different power consumption variables. 



## Key Findings

* **Seasonality**: Energy consumption demonstrates clear seasonal patterns, with peaks during winter months (likely due to heating) and dips during summer.
* **Voltage Stability**: Voltage levels remain relatively stable throughout the year, with minimal variations.
* **Correlations**: 'Global_active_power' and 'Global_intensity' show a strong positive correlation.

## Next Steps

* Explore more sophisticated imputation methods (e.g., interpolation or model-based methods).
* Incorporate time-based features (e.g., month, season) in further analysis.
* Consider more advanced time series models for forecasting or anomaly detection.
