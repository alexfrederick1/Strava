🏃‍♂️ Running Pace Prediction
This project uses real Strava running logs from our own actual runs to analyze training patterns and build a model capable of predicting each person’s next run before it happens. The goal is to forecast both how far the next run will be and the pace that runner is likely to maintain.
🔧 Approach
Data Preparation: Exported Strava activity data was cleaned, standardized, and enhanced with additional running-related features (pace metrics, recency effects, run-history context, etc.).
Exploratory Analysis: Trends in mileage, pace improvements, consistency, and correlations across training behavior were visualized to better understand running patterns.
Two-Stage Machine Learning Model (Ridge Regression):
Predict the next run distance based on each runner’s historical data.
Predict the next run pace, using the predicted distance and engineered features to estimate minutes per mile.
🎯 Results
The system’s predictions are evaluated against simple baselines (such as using the previous run or average pace) using metrics like MAE and MSE, with visual analysis to understand model accuracy and behavior.
