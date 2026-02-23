# Advanced Weather Temperature Prediction

## Project Overview
This project is an evolution of my initial data science work. While my first project used only humidity to predict temperature, this analysis utilizes **Multiple Linear Regression** to incorporate several weather variables, significantly increasing the model's predictive power and accuracy.

## Dataset
The dataset contains 10 years of hourly weather data from Szeged, Hungary (2006–2016).
- **Source:** [Szeged Weather History on Kaggle](https://www.kaggle.com/datasets/budincsevity/szeged-weather)
- **Features Used:** Humidity, Wind Speed (km/h), and Atmospheric Pressure (millibars).
- **Target Variable:** Temperature (C).

## Technical Workflow
1. **Data Preprocessing:** Handled missing values in precipitation data and filtered atmospheric pressure outliers.
2. **Feature Selection:** Selected multiple independent variables to observe their combined effect on temperature.
3. **Model Training:** Implemented a Multiple Linear Regression model using Scikit-Learn.
4. **Evaluation:** Measured performance using Mean Squared Error (MSE) and R-squared ($R^2$) metrics.

## Key Results
The transition from a single-feature model to a multi-feature model yielded significant improvements:
- **R-squared Score:** 0.42 (An improvement from 0.26 in the basic project).
- **Mean Squared Error (MSE):** 53.0 (Significantly lower than the initial 144.08).

This demonstrates that temperature is a complex variable that is better explained when humidity is combined with wind speed and pressure data.

## How to Setup
1. Clone the repository.
2. Create a virtual environment: `python -m venv venv_szeged`
3. Activate the environment and install dependencies:
   ```bash
   pip install -r requirements.txt
