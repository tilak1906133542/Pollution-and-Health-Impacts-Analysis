# Pollution-and-Health-Impacts-Analysis
This project analyzes the relationship between air pollution levels and their impacts on public health across various countries. By examining AQI (Air Quality Index) values and pollutants like CO, Ozone, NO2, and PM2.5, we explore their effects on respiratory diseases, cardiovascular diseases, and mortality rates.
# Pollution and Health Impacts Analysis

## Project Overview
This project analyzes the relationship between air pollution levels and their impacts on public health across various countries. By examining AQI (Air Quality Index) values and pollutants like CO, Ozone, NO2, and PM2.5, we explore their effects on respiratory diseases, cardiovascular diseases, and mortality rates. The aim is to identify high-risk regions and provide actionable insights to guide environmental and healthcare policies.

## Datasets
1. **Global Air Pollution Dataset (`global_air_pollution_dataset.csv`)**:
   - Contains air quality data for cities and countries, including overall AQI values and individual pollutant levels.
   - **Columns**: `Country`, `City`, `AQI Value`, `CO AQI Value`, `Ozone AQI Value`, `NO2 AQI Value`, `PM2.5 AQI Value`.

2. **Countries Data (`countries_data.json`)**:
   - Provides health impact data such as respiratory and cardiovascular disease statistics and mortality rates across countries.
   - **Fields**: `Country`, `RespiratoryDiseases`, `CardiovascularDiseases`, `MortalityRate`, `Population`.

## Key Features

### 1. **Data Cleaning and Preprocessing**:
- Removed rows with missing values to ensure data completeness.
- Normalized AQI values for consistency in comparisons.
- Extracted and aggregated health data into distinct metrics: `RespiratoryDiseases`, `CardiovascularDiseases`, and `MortalityRate`.

### 2. **Data Merging**:
- Merged the pollution and health datasets on the `Country` column using an inner join to create a comprehensive dataset.

### 3. **Feature Engineering**:
- Calculated average AQI and pollutant levels for each country.
- Categorized countries into `Good`, `Moderate`, and `Unhealthy` air quality levels based on AQI thresholds.
- Derived health impact scores for comparative analysis.

### 4. **Exploratory Data Analysis (EDA)**:
- Analyzed correlations between air pollution and health metrics.
- Identified top high-risk countries based on AQI and health impact data.

### 5. **Visualizations**:
- **Bar Charts**: Top 10 countries by AQI and pollutant levels.
- **Scatter Plots**: Relationships between AQI and health metrics (e.g., respiratory and cardiovascular diseases).
- **Category Distribution**: Proportion of countries in each AQI category (`Good`, `Moderate`, `Unhealthy`).

## Visualizations

### **Top 10 Countries by Average AQI and Pollutants**
- **Description**: Bar plot showing AQI and pollutant levels (CO, Ozone, NO2, PM2.5) for the top 10 most polluted countries.
- **Insight**: Identifies regions with the worst air quality and the dominant pollutants.

### **Top 10 Countries by Aggregated Health Impacts**
- **Description**: Bar plot visualizing the top 10 countries with the highest rates of respiratory and cardiovascular diseases, as well as mortality.
- **Insight**: Highlights countries needing targeted health interventions.

### **AQI Categories Distribution**
- **Description**: Pie chart depicting the percentage of countries falling under `Good`, `Moderate`, and `Unhealthy` air quality categories.
- **Insight**: Provides an overview of global air quality conditions.

### **Scatter Plot: AQI vs. Respiratory Diseases**
- **Description**: Examines the correlation between AQI values and respiratory disease cases.
- **Insight**: Confirms a positive relationship, indicating higher respiratory disease rates with increasing pollution.

### **Scatter Plot: AQI vs. Cardiovascular Diseases**
- **Description**: Displays the relationship between AQI values and cardiovascular disease cases.
- **Insight**: Reveals the health risks posed by poor air quality on cardiovascular health.

## Tools and Technologies
- **Languages**: Python  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn  
- **Data Sources**: CSV and JSON files for pollution and health statistics  

## Key Insights
1. **High Pollution, High Risk**:
   - Countries with the highest AQI values, such as those dominated by CO and PM2.5, report significantly higher rates of respiratory and cardiovascular diseases.

2. **Health Impacts by Region**:
   - Regions with persistent `Unhealthy` AQI levels show a strong correlation with higher mortality rates.

3. **Actionable Interventions**:
   - Encouraging cleaner energy sources and stricter emissions standards in high-risk countries could significantly reduce pollution-related health impacts.

## Conclusion
This project provides a comprehensive analysis of air pollution and its health impacts across countries. By combining pollution metrics and health data, it highlights the critical need for targeted public health and environmental strategies to mitigate risks. The findings support data-driven decision-making to address global pollution challenges.

