📈 Time Series Forecasting of Daily Demand
🧩 Project Overview

This project focuses on forecasting daily demand using various time series forecasting models.
The goal is to compare traditional and statistical forecasting approaches based on their accuracy and interpretability.

⚙️ Models Implemented

Naive Forecasting: Uses the last observed value as the forecast.

Moving Average: Predicts future demand as the average of previous observations.

Linear Regression: Uses date-based features (day, month, year, weekday) for supervised learning.

ARIMA (AutoRegressive Integrated Moving Average): Captures temporal patterns and autocorrelations.

📊 Dataset

The dataset contains historical order data with:

Date: The order date.

Unit quantity: Number of units ordered per day.

The data was preprocessed to aggregate daily totals and ensure chronological forecasting.

🧼 Preprocessing Steps

Converted Order Date to datetime format.

Aggregated total demand per day.

Split dataset into train (80%) and test (20%) chronologically.

Generated date-based features (day, month, year, dayofweek) for regression models.

🔮 Forecasting & Evaluation

Each model predicts future demand over the test period.
Performance is evaluated using:

MAE (Mean Absolute Error)

RMSE (Root Mean Squared Error)

📉 Visualization

The forecast comparison plot shows:

Black line: Actual demand (Test set)

Orange dashed line: Naive forecast

Purple dashed line: Moving Average

Green dashed line: Linear Regression

Brown dashed line: ARIMA

Each model’s trend and deviation from actual demand are clearly visualized.

📈 Sample Results
Model	MAE	RMSE
Naive	215.4	276.8
Moving Average	198.7	250.5
Linear Regression	170.9	230.4
ARIMA	155.3	205.8

(Note: Replace with your actual results after running the code.)

🧰 Tech Stack

Python 3.10+

Libraries: pandas, numpy, matplotlib, scikit-learn, statsmodels

📚 Learnings

How to perform chronological train-test splits for time series.

Implementing and comparing baseline, regression, and ARIMA models.

Visualizing multiple forecasts effectively.

Evaluating models using quantitative metrics.

🧠 Future Improvements

Implement LSTM/GRU for capturing long-term dependencies.

Include seasonal decomposition and exogenous features (e.g., promotions, holidays).

Automate model selection with AutoARIMA.
