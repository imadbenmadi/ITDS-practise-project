# WWII Weather Data Analysis Notebook

## Introduction

In this project, I embarked on an exciting journey to analyze simulated World War II weather data. The goal was to explore historical weather patterns, uncover insights, and build predictive models. This notebook showcases my step-by-step approach, from data preparation to advanced machine learning techniques, and even an interactive user interface for predictions.

---

## What I Did

### 1. **Data Loading and Exploration**
I started by creating synthetic weather data for the WWII era (1939–1945) across five major European cities: London, Berlin, Paris, Warsaw, and Moscow. The dataset includes daily weather attributes like temperature, pressure, humidity, wind speed, and weather conditions. I explored the dataset to understand its structure and characteristics, ensuring it was ready for analysis.

---

### 2. **Data Cleaning and Preprocessing**
To ensure the data was clean and usable:
- I combined date and time into a single `datetime` column for time series analysis.
- Missing values were handled using interpolation for numerical data and mode imputation for categorical data.
- I standardized numerical values to ensure they fell within reasonable ranges.
- Additional features like `year`, `month`, `day`, and `season` were derived from the `datetime` column.

---

### 3. **Exploratory Data Analysis (EDA)**
This was the fun part! I visualized the data to uncover patterns:
- **Temperature Analysis:** I plotted temperature distributions and seasonal variations.
- **Weather Conditions:** I analyzed the frequency of weather conditions and their seasonal trends.
- **Time Series Plots:** I created time series plots for average temperatures, marking significant WWII events like D-Day and VE Day.
- **Relationships:** I explored how temperature, pressure, humidity, and wind speed interacted with each other.

---

### 4. **Feature Engineering**
To enhance the dataset, I engineered new features:
- **Temperature Range:** The daily difference between max and min temperatures.
- **Pressure Tendency:** Whether pressure was rising, steady, or falling.
- **Extreme Weather Indicators:** Flags for unusually high or low temperatures.
- **Dew Point and Heat Index:** Calculated using weather formulas.
- **Season-Normalized Temperature:** Z-scores of temperature within each season.
- **Weather Severity Index:** A simplified score based on weather conditions and wind speed.

---

### 5. **Time Series Analysis**
I dove deeper into the temporal aspect of the data:
- **Stationarity Testing:** Using the Augmented Dickey-Fuller test, I checked if the time series was stationary.
- **Decomposition:** I broke down the time series into trend, seasonality, and residual components.
- **Autocorrelation:** I used ACF and PACF plots to understand lagged relationships in the data.

---

### 6. **Correlation Analysis**
I investigated relationships between weather variables:
- **Heatmaps:** I created correlation heatmaps to visualize dependencies.
- **Seasonal Correlations:** I analyzed how correlations varied across seasons.
- **Scatter Plot Matrix:** I visualized pairwise relationships between key variables.

---

### 7. **Geospatial Visualization**
To add a spatial dimension to the analysis:
- **Interactive Maps:** Using Folium, I created maps to visualize weather conditions across Europe.
- **Temperature Heatmaps:** I highlighted temperature variations geographically.
- **Markers:** Each location had detailed weather information displayed interactively.

---

### 8. **Weather Pattern Classification**
I applied clustering algorithms to identify distinct weather patterns:
- **K-Means Clustering:** I determined the optimal number of clusters using the elbow method and grouped weather data into clusters.
- **PCA Visualization:** I reduced the data to two dimensions for easy visualization of clusters.
- **Cluster Analysis:** I analyzed the characteristics of each cluster and assigned descriptive labels like "Cold and Humid" or "Warm and Dry."

---

### 9. **Predictive Modeling**
I built machine learning models to predict next-day temperatures:
- **Lagged Features:** I created lagged variables for temperature, pressure, humidity, and wind speed.
- **Random Forest and Gradient Boosting:** I trained and compared these models, evaluating them using metrics like RMSE, MAE, and R².
- **Feature Importance:** I identified the most influential features for temperature prediction.
- **Error Analysis:** I visualized prediction errors to understand model performance.

---

### 10. **Interactive User Interface**
To make the project more engaging, I built an interactive UI using `ipywidgets`:
- Users can select a location and input weather data (manually or randomly).
- The interface predicts next-day temperatures using both Random Forest and Gradient Boosting models.
- It provides an interpretation of the forecast, such as whether the temperature is expected to rise or fall.

---

## Conclusion

This notebook is a comprehensive demonstration of my data science skills, covering everything from data cleaning and visualization to advanced machine learning and interactive applications. It was an incredible learning experience, and I hope it inspires others to explore the fascinating world of weather data analysis!