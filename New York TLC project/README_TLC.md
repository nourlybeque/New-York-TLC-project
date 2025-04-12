# New York TLC project

## Project Overview
This project focuses on predicting taxi fares before a ride using **Multiple Linear Regression**. The goal is to analyze various trip-related features to estimate the fare cost. 

Data team (Automatidata) works with its clients to transform their unused and stored data into useful solutions, such as performance dashboards, customer-facing tools, strategic business insights, and more. They specialize in identifying a client’s business needs and utilizing their data to meet those business needs. 
Automatidata is consulting for the New York City Taxi and Limousine Commission (TLC). New York City TLC is an agency responsible for licensing and regulating New York City's taxi cabs and for-hire vehicles. The agency has partnered with Automatidata to develop a regression model that helps estimate taxi fares before the ride, based on data that TLC has gathered. 
The TLC data comes from over 200,000 taxi and limousine licensees, making approximately one million combined trips per day. 


## Dataset
- The dataset includes trip details such as:
  - Pickup and drop-off locations
  - Trip distance
  - Time of day
  - Number of passengers
- Data preprocessing steps included:
  - Handling missing values
  - Converting categorical data into numerical form
  - Feature engineering

## Methodology
### Multiple Linear Regression Model
- Chosen as the primary predictive model due to its interpretability.
- Key features used in the model:
  - mean_distance (traveled)
  - mean_duration (of each trip)
  - Pickup and drop-off locations (IDs)
- Model evaluation:
  - R² Score: **0.8682583641795454**
  - MAE: **2.1336549840593864**
  - MSE: **14.326454156998944**
  - RMSE: **3.785030271609323**

## Challenges Faced
- Understanding **Multiple Linear Regression**, especially feature engineering and model interpretation.

## Results
- The **Multiple Linear Regression model** provides reasonable predictions for taxi fares.
- Example output (Predicted vs. Actual fares):
  
|           | Actual Fare | Predicted Fare | Residual  |
|-----------|-------------|----------------|-----------|
| 5818      | $14.0       | $12.356503     | 1.643497  |
| 18134     | $28.0       | $16.314595     | 11.685405 |
| 4655      | $5.5        | $6.726789      | -1.226789 |
  
- Visualizations: (see visuals_TLC folder)

## Conclusion
✅ Successfully built a **Multiple Linear Regression model** for taxi fare prediction.
✅ Processed and cleaned real-world data.



