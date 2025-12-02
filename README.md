# Running Pace Prediction

This project uses real Strava running logs from our own runs to analyze training behavior and build a model that predicts each person’s next run. The system forecasts both how far the next run will be and the pace that runner is likely to maintain.

## Approach

- **Data Preparation:** Strava exports were cleaned, standardized, and enhanced with engineered features such as pace metrics, recency effects, and run-history context.
- **Exploratory Analysis:** Trends in mileage, pace progression, consistency, and correlations across features were visualized to better understand running patterns.
- **Two-Stage Modeling (Ridge Regression):**
  1. Predict the next run distance for each runner.
  2. Use that predicted distance and additional features to estimate minutes-per-mile pace.

## Results

Model performance was evaluated against simple baselines (such as previous run or average pace) using metrics like MAE and MSE, along with visual inspection to assess accuracy and model behavior.
