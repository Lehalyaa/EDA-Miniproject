# 🌫️ AQI & Weather Dashboard

## Objective:
To develop an interactive geospatial dashboard for multi-city air quality analysis and comparative weather profiling, utilizing machine learning to provide data-driven AQI and climate forecasts.

## Tools used:
VS Code or Jupyter Notebook

## Functions used

<img width="985" height="516" alt="image" src="https://github.com/user-attachments/assets/217c5ae0-f6ed-4068-9a7b-2be69683df97" />

## Introduction:

This project presents an interactive AQI & Weather Dashboard built using Streamlit, designed to analyze, compare, and predict environmental conditions across multiple cities.

The application integrates Exploratory Data Analysis (EDA) with machine learning to provide both descriptive and predictive insights. It transforms raw environmental datasets into an intuitive, multi-tab dashboard that supports real-time interaction and decision-making.

**dashboard.py** reads **EDA_Main_Dataset_Weather_Enriched.csv** and launches a browser-based
dashboard with three independent tabs — each serving a different analytical purpose.
No internet connection is required after setup. All charts are interactive (zoom, hover,
export) via Plotly.

## Key Features:

1. General Visualization
* Identifies most and least polluted cities
* Highlights seasonal air quality patterns
* Displays:
    --> Top 10 most polluted cities (Average AQI)
    --> AQI distribution across seasons
    --> KPI-based summary cards for quick insights

2. City Comparison
* Side-by-side comparison between any two cities
* Dynamic filtering based on:
   --> Season
   --> Environmental metrics (AQI, Temperature, Humidity, Wind Speed, Rainfall)
* Visualizations include:
   --> Distribution plots (Histogram + Violin)
   --> Time-series trend analysis

3. Future Prediction
* Machine learning-based forecasting using Random Forest Regression
* Predicts:
   --> AQI
   --> Temperature
   --> Humidity
* User inputs:
   --> City
   --> Future date
* Intelligent classification of air quality:
   --> Good / Satisfactory / Moderate / Poor

## Dashboard Review

**Tab 1:General Visualization**

* Displays AQI trends and key pollution insights

* Helps identify critical environmental hotspots

<img width="1918" height="1074" alt="1,2,3 - Output" src="https://github.com/user-attachments/assets/554af059-26db-420a-bfed-9030a2e73194" />

**Tab 2:City Comparison**

* Enables detailed comparative analysis between cities

* Reveals distribution differences and seasonal variations

<img width="1919" height="1078" alt="4 - output part 1" src="https://github.com/user-attachments/assets/5b6225a4-18a0-4f2b-ac36-4171f26b1c75" />

<img width="1894" height="623" alt="4 - output part 2" src="https://github.com/user-attachments/assets/713eeaf6-b17d-4af5-9583-bbd6448f4a1e" />

**Tab 3: Future Prediction**

* Provides forward-looking environmental insights
  
* Useful for planning and awareness

<img width="1916" height="1076" alt="5,6 - output" src="https://github.com/user-attachments/assets/53781064-851a-49b9-8eb9-e3f316a7f9ed" />

## Key Insights:

* Certain cities consistently exhibit high AQI levels, indicating persistent pollution sources

* Winter season shows significantly higher AQI due to atmospheric conditions

* Monsoon season generally improves air quality due to pollutant dispersion

* Predictive results align with historical seasonal trends

## Limitations:

* Model accuracy depends on historical data quality

* External factors like sudden weather changes or policy interventions are not included

* City encoding may limit generalization to unseen regions

## Future Enhancements:

* Integration with live AQI APIs

* Advanced models (LSTM / Time Series Forecasting)

* Deployment on cloud platforms (Streamlit Cloud / AWS)

* Real-time alert system for hazardous AQI levels
