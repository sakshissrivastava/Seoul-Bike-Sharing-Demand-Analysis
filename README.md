# 🚴 Seoul Bike Sharing Demand Analysis

## 📊 Project Overview
This project analyzes the **Seoul Bike Sharing System (Ddareungi)** to identify key factors influencing hourly bike rental demand. Using a comprehensive dataset of 8,760 records, the analysis explores weather conditions, temporal patterns, and operational variables to develop predictive models for demand forecasting. The findings aim to optimize resource allocation and improve user satisfaction.

The project demonstrates expertise in:
- *Data preprocessing:* Cleaning, transformation, encoding, and feature engineering.
- *Exploratory Data Analysis (EDA):* Visualization of trends and correlations.
- *Statistical modeling:* Hypothesis testing and regression analysis.
- *Machine learning:* Predictive modeling for demand forecasting.

---

## 🗂️ Dataset Description
The dataset contains hourly records of bike rentals from December 2017 through November 2018 in Seoul. It includes 14 variables:

| Variable              | Description                                                  |
|-----------------------|--------------------------------------------------------------|
| `Date`                | Day/Month/Year                                              |
| `Rented Bike Count`   | Count of bikes rented per hour                              |
| `Hour`                | Hour of the day (0–23)                                      |
| `Temperature (°C)`    | Temperature in Celsius                                       |
| `Humidity (%)`        | Humidity percentage                                          |
| `Wind Speed (m/s)`    | Wind speed in meters per second                              |
| `Visibility (10m)`    | Visibility score (in 10-meter units)                         |
| `Dew Point Temperature` | Dew point temperature in Celsius                           |
| `Solar Radiation (MJ/m²)` | Solar radiation in megajoules per square meter           |
| `Rainfall (mm)`       | Rainfall in millimeters                                      |
| `Snowfall (cm)`       | Snowfall in centimeters                                      |
| `Seasons`             | Season of the year (`Winter`, `Spring`, `Summer`, `Autumn`) |
| `Holiday`             | Whether it is a holiday (`Holiday`, `No Holiday`)           |
| `Functioning Day`     | Whether the system was operational (`Yes`, `No`)            |

Source: [Seoul Open Data Portal](http://data.seoul.go.kr/)

---

## 🚀 Key Objectives
1. **Understand demand drivers**: Analyze the impact of weather conditions, time of day, seasons, and holidays on bike rentals.
2. **Develop predictive insights**: Build machine learning models to forecast hourly bike rental demand.
3. **Optimize operations**: Provide actionable recommendations for dynamic bike redistribution and resource planning.

---

## 🛠️ Methodology
### 1. **Data Preprocessing**
- Handled missing values and duplicates.
- Feature engineering:
  - Derived variables like weekday/weekend indicators and seasonal encodings.
  - Log-transformed skewed data for better model performance.
- Normalized continuous variables for consistency.

### 2. **Exploratory Data Analysis (EDA)**
- Visualized trends using heatmaps, line plots, and bar charts.
- Identified strong correlations:
  - Positive: Temperature, visibility, solar radiation.
  - Negative: Rainfall, snowfall, humidity.
- Observed clear temporal patterns:
  - Higher rentals during rush hours on weekdays.
  - Seasonal peaks in summer and troughs in winter.

### 3. **Statistical Analysis**
- Conducted hypothesis tests:
  - Significant differences in rentals between holidays and non-holidays.
  - Weather conditions significantly impact demand (e.g., ANOVA results).
- Built multiple linear regression models:
  - Key predictors: Temperature (+), rainfall (-), holidays (-).

### 4. **Predictive Modeling**
- Developed a regression model with log-transformed target variable (`Rented Bike Count`):
  - \( R^2 = 57.7\% \): Explained variance in bike rentals.
  - Significant predictors: Hour of the day, temperature, humidity, solar radiation.

---

## 📈 Results & Insights
1. **Temporal Trends**:
   - Peak rentals during commuting hours (7–9 AM and 5–7 PM).
   - Weekend usage is more evenly distributed compared to weekdays.

2. **Weather Impact**:
   - Rentals increase with higher temperatures but decrease with rainfall or snowfall.
   - Clear skies (higher solar radiation) positively influence demand.

3. **Holidays vs Non-Holidays**:
   - Rentals are significantly lower on holidays (-45%).

4. **Seasonal Patterns**:
   - Summer sees the highest rentals; winter experiences a sharp decline.

---

## 💡 Recommendations
1. **Dynamic Bike Redistribution**:
   - Increase fleet availability during peak hours and favorable weather conditions.
   - Reduce operations during adverse weather (e.g., heavy rainfall).

2. **Operational Efficiency**:
   - Schedule maintenance during low-demand periods (e.g., late nights).
   - Implement preventive maintenance before peak summer months.

3. **Pricing Strategies**:
   - Introduce dynamic pricing: Premium rates during high-demand hours; discounts during low-demand periods or adverse weather.

4. **Future Analytics Scope**:
   - Predict station-specific shortages using geospatial data.
   - Explore customer segmentation for targeted promotions.

---

## 🔮 Future Directions
1. Incorporate real-time data for dynamic forecasting.
2. Explore deep learning models for improved accuracy.
3. Integrate external datasets like traffic or public transport schedules.

---

## 💼 Skills Demonstrated
- Python libraries: Pandas, NumPy, Matplotlib, Seaborn, Statsmodels, Scikit-learn.
- Data cleaning & preprocessing techniques.
- Advanced visualization for storytelling.
- Statistical modeling & hypothesis testing.
- Machine learning for regression analysis.

---