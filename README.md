# Car-Sales

Car Sales Analysis and Prediction – Project Report
Dataset Overview
File Name: carsales.csv

Total Features: 15

Target Variable: Sales_in_thousands

Key Features: Manufacturer, Model, Vehicle_type, Price_in_thousands, Engine_size, Horsepower, Fuel_efficiency, __year_resale_value, etc.

Objective: Analyze trends and build machine learning models to predict car sales performance based on vehicle attributes.

Data Cleaning Summary
Removed rows with missing values in critical columns.

Converted Latest_Launch to datetime.

Encoded the categorical Vehicle_type column using One-Hot Encoding.

Removed non-predictive columns: Manufacturer, Model, and Latest_Launch.

Exploratory Data Analysis (EDA) Insights
Top Manufacturers by Sales
Top 3: Ford, Chevrolet, Toyota.

Ford led the market with the highest cumulative sales across multiple models.

Vehicle Type vs Price
SUVs had the highest median price.

Passenger cars had the lowest price range, indicating affordability focus.

⚙ Horsepower vs Fuel Efficiency
A negative correlation was observed: higher horsepower typically led to lower fuel efficiency.

SUVs and Sports vehicles clustered at high horsepower, low mileage regions.

Sales Trend Over Time
Some peaks were visible around major launch dates in specific years.

Sales spiked shortly after new launches, then declined — showing the importance of novelty and market timing.

Statistical Insights
Metric	Value
Average Sales	~10.3 thousand units
Average Price	~$25.5k
Average Resale Value	~$14.8k
Best Power-to-Weight Ratio	Achieved by a sports model with highest horsepower-to-curb weight

Machine Learning Models
Target: Predict Sales_in_thousands
Features Used:
Numeric: Price_in_thousands, Engine_size, Horsepower, Fuel_efficiency, etc.

Categorical (encoded): Vehicle_type

Linear Regression Results
RMSE: ~2.81

R² Score: 0.76

Interpretation: Explained ~76% of variance in car sales.

Random Forest Results
RMSE: ~1.89 (better!)

R² Score: 0.89

Interpretation: Highly accurate predictions using ensemble learning.

Top 5 Important Features (by Random Forest):
Price_in_thousands

Fuel_efficiency

Horsepower

__year_resale_value

Engine_size

Visualization – Actual vs Predicted Sales
Predicted values closely follow the actual values.

Minimal under- or over-prediction for most samples — Random Forest showed strong generalization.

Final Conclusion & Business Insights
Vehicle type, price, and efficiency are strong predictors of sales success.

SUVs and sports cars command higher prices but suffer from lower fuel economy.

Manufacturers should balance horsepower and fuel efficiency to appeal to a wider consumer base.

Predictive models can assist in forecasting sales for new launches based on specifications.

Data-driven feature design and pricing can boost profitability and market capture.
