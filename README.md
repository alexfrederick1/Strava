🏃‍♂️Running Pace Prediction
This project uses real Strava running logs from our own runs to analyze training behavior and build a model that predicts each person’s next run. The system forecasts both how far the next run will be and the pace that runner is likely to maintain.
🔧Approach
Data Preparation: Strava exports were cleaned, standardized, and enhanced with additional engineered features such as pace metrics, recency effects, and run history context.
Exploratory Analysis: Trends in mileage, pace progression, consistency, and feature correlations were visualized to understand patterns in running behavior.
Two-Stage Modeling (Ridge Regression):
Predict the next run distance for each runner.
Use that predicted distance plus additional features to estimate the expected minutes-per-mile pace for that run.
🎯 Results
Model performance was evaluated against simple baselines (such as previous run distance or average pace) using metrics like MAE and MSE, along with visual inspection to assess prediction accuracy and behavior.
