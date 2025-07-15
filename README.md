NYC Taxi Demand Prediction using Machine Learning
This project aims to forecast hourly taxi demand across New York City by leveraging historical Yellow Taxi trip data and hourly weather conditions from January to March 2023. By combining trip-level data with weather variables, we train and evaluate several machine learning models to uncover patterns in ride demand. The goal is to support efficient fleet management, reduce passenger wait times, and enable data-driven decisions in urban transportation planning.

🚀 Project Objective
Build a machine learning-based forecasting system to predict taxi ride demand for the next hour across NYC boroughs, incorporating:
Historical trip data (from NYC Yellow Taxi records)
Hourly weather conditions (temperature, wind, precipitation, visibility)

📊 Datasets Used
Taxi Trip Data: Yellow Taxi trip records from the NYC Taxi & Limousine Commission (TLC)
Weather Data: Hourly NYC weather data sourced from Visual Crossing

🧹 Data Preprocessing
Filtered invalid records (e.g., trips lasting over 12 hours or speeds exceeding 60 mph)

Merged weather data with trip records at an hourly resolution
Engineered relevant features such as:
Trip metrics: duration, average speed
Temporal features: hour of day, weekday, month
Weather summaries: temperature, wind speed, precipitation

🧠 Model Architectures
The following machine learning models were trained and evaluated:

LightGBM
CatBoost
XGBoost
AdaBoost

Each model predicts the target variable: rides_next_hour (i.e., number of trips in the upcoming hour).

📏 Evaluation Metrics
Models are evaluated using standard regression metrics:
MAE: Mean Absolute Error
MSE: Mean Squared Error
RMSE: Root Mean Squared Error
