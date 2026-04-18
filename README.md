# Agricultural Pest Risk Analysis System

This project implements a Machine Learning pipeline to predict pest risk levels and provide optimized irrigation and pest management suggestions based on environmental factors like Temperature, Humidity, and Soil Moisture.

## Features
- **Data Cleaning:** Handles complex range-based strings and percentage formatting.
- **Feature Engineering:** Includes interaction features (Temperature × Humidity, etc.) to improve model accuracy.
- **Clustering:** Uses KMeans to group weather patterns and crop types.
- **Predictive Modeling:** Compares **Random Forest Regressor** and **XGBoost Regressor** for Pest Risk prediction.
- **Recommendation Engine:** Provides real-time suggestions for irrigation and specific pesticides.

## Model Performance
The XGBoost model outperformed the Random Forest model with the following metrics:
- **R² Score:** 0.99
- **RMSE:** 0.53
- **MAE:** 0.38

## Visualizations
The project includes:
- KMeans Clustering plots for weather data.
- Correlation Heatmaps of agricultural features.
- Model performance comparison charts (RMSE, MAE, R2).

## How to Use
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`
3. Run the notebook or script to train the model.
4. Use the `predict_pest_risk_with_suggestions()` function to get management advice for specific crops.
