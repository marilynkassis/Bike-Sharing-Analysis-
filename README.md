# Bike-Sharing-Analysis-
This project aims to uncover key patterns, trends, and insights about rental bike usage.

## Project Overview
This project analyzes a bike-sharing dataset to uncover key patterns, trends, and insights about rental bike usage. By performing exploratory data analysis (EDA) and applying machine learning models, the goal is to predict the number of rental bikes under various weather and temporal conditions.

---

## Dataset Description
The dataset contains hourly records of bike-sharing data, with the following key features:
- **instant:** Record index.
- **dteday:** Date of the record.
- **season:** Season (1: Winter, 2: Spring, 3: Summer, 4: Fall).
- **yr:** Year (0: 2011, 1: 2012).
- **mnth:** Month (1 to 12).
- **hr:** Hour of the day (0 to 23).
- **holiday:** Whether the day is a holiday (1: Yes, 0: No).
- **weekday:** Day of the week.
- **workingday:** Whether the day is a working day (1: Yes, 0: No).
- **weathersit:** Weather situation:
  - 1: Clear, Few Clouds, Partly Cloudy.
  - 2: Mist + Cloudy, Mist + Few Clouds.
  - 3: Light Snow, Light Rain.
  - 4: Heavy Rain, Thunderstorms.
- **temp:** Normalized temperature (0-1 scale, max = 41°C).
- **atemp:** Normalized "feels-like" temperature (0-1 scale, max = 50°C).
- **hum:** Normalized humidity (0-1 scale, max = 100%).
- **windspeed:** Normalized wind speed (0-1 scale, max = 67 units).
- **casual:** Count of casual users.
- **registered:** Count of registered users.
- **cnt:** Total count of rental bikes (casual + registered).

---

## Project Structure
### PART I: Exploratory Data Analysis (EDA)
- **Goal:** Explore the dataset to identify patterns and trends in bike-sharing usage.
- **Methods Used:**
  - Descriptive statistics to summarize the dataset.
  - Data visualizations (e.g., histograms, bar charts, heatmaps) to explore relationships between features.

### PART II: Feature Engineering
- **Objective:** Create and transform variables for improved predictive power.
- **Key Transformations:**
  - Encoding categorical variables (e.g., season, weekday, weathersit).
  - Normalizing numerical features for consistency.

### PART III: Predictive Modeling
- **Goal:** Develop machine learning models to predict the total count of rental bikes (`cnt`).
- **Models Explored:**
  - Linear Regression.
  - Random Forest Regression.
  - Gradient Boosting Machines (e.g., XGBoost).
- **Evaluation Metrics:**
  - Mean Absolute Error (MAE).
  - Root Mean Squared Error (RMSE).
  - R-squared (R²).

---

## Tools and Libraries Used
- **Programming Language:** Python.
- **Libraries:**
  - `pandas`: Data manipulation and preprocessing.
  - `matplotlib` and `seaborn`: Data visualization.
  - `scikit-learn`: Machine learning and model evaluation.
  - `numpy`: Numerical computations.
  - `scipy`: Statistical analysis.

---

## Insights and Outcomes
1. **Seasonality and Temporal Trends:**
   - Rental counts peak during summer and fall seasons.
   - Weekends show higher casual user counts, while weekdays have more registered users.
2. **Impact of Weather:**
   - Clear weather significantly boosts bike rentals, while bad weather (e.g., rain, snow) reduces rentals.
3. **Feature Importance:**
   - Temperature and hour of the day are the strongest predictors of bike rentals.
4. **Model Performance:**
   - Random Forest Regression performed the best, with an R² score of 0.85 and low error metrics.

---
