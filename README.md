# Project Background

New York City TLC is an agency responsible for licensing and regulating New York City's taxi cabs and for-hire vehicles. The agency has requested for developing a regression model that helps estimate taxi fares before the ride, based on data that TLC has gathered. The TLC data comes from over 200,000 taxi and limousine licensees, making approximately one million combined trips per day. This project focuses on predicting taxi fares before a ride using **Multiple Linear Regression**. The goal is to analyze various trip-related features to estimate the fare cost. 


The Python EDA used to inspect and clean the data for this analysis can be found [here.](https://github.com/nourlybeque/New-York-TLC-project/blob/20bc8e16b824efa1e68e0e1b8fec7e558faf3128/New%20York%20TLC%20project/notebooks_TLC/New_York_TLC_1_EDA.ipynb)

The Python A/B testing regarding various business questions can be found [here.](https://github.com/nourlybeque/New-York-TLC-project/blob/20bc8e16b824efa1e68e0e1b8fec7e558faf3128/New%20York%20TLC%20project/notebooks_TLC/New_York_TLC_2_AB_testing.ipynb)

The Python with multiple linear regression model used to report and explore sales trends can be found [here.](https://github.com/nourlybeque/New-York-TLC-project/blob/20bc8e16b824efa1e68e0e1b8fec7e558faf3128/New%20York%20TLC%20project/notebooks_TLC/New_York_TLC_3_MultipleLinearRegression.ipynb)




# Data Structure & Initial Checks

This project uses a dataset called 2017_Yellow_Taxi_Trip_Data. It contains data gathered by the New York City Taxi & Limousine Commission. 

The dataset contains:
22,699 rows - each row represents a different trip
18 columns

  | Column Name            | Description                 |
  |------------------------|---------------------------- |
  | ID                     | Trip identification number  |
  | VendorID               | A code indicating the TPEP provider that provided the record. **1=Creative Mobile Technologies**, **LLC;** **2=VeriFone Inc.**|
  | tpep_pickup_date time  | The date and time when the meter was engaged. |
  | tpep_dropoff_date time | The date and time when the meter was disengaged. |
  | Passenger_count        | The number of passengers in the vehicle. This is a driver-entered value. |
  | Trip_distance          | The elapsed trip distance in miles reported by the taximeter. |
  | PULocationID           | TLC Taxi Zone in which the taximeter was engaged. |
  | DOLocationID           | TLC Taxi Zone in which the taximeter was disengaged. |
  | RateCodeID             | The final rate code in effect at the end of the trip. 1=Standard rate 2=JFK 3=Newark 4=Nassau or Westchester 5=Negotiated fare 6=Group ride |
  | Store_and_fwd_flag     | This flag indicates whether the trip record was held in vehicle memory before being sent to the vendor, aka "store and forward," because the vehicle did not have a connection to the server. Y=store and forward trip N=not a store and forward trip |
  | Payment_type           | A numeric code signifying how the passenger paid for the trip. 1=Credit card 2=Cash 3=No charge 4=Dispute 5=Unknown 6=Voided trip |
  | Fare_amount            | The time-and-distance fare calculated by the meter. |
  | Extra                  | Miscellaneous extras and surcharges. Currently, this only includes the $0.50 and $1 rush hour and overnight charges. |
  | MTA_tax                | $0.50 MTA tax that is automatically triggered based on the metered rate in use. |
  | Improvement_surcharge  | $0.30 improvement surcharge assessed trips at the flag drop. The improvement surcharge began being levied in 2015. |
  | Tip_amount             | Tip amount - This field is automatically populated for credit card tips. Cash tips are not included. |
  | Tolls amount           | Total amount of all tolls paid in trip. |
  | Total amount           | The total amount charged to passengers. Does not include cash tips. |



# Executive Summary

### Overview of Findings

Based on parameters of the newly created multiple linear regression model states that for every 3.57 miles traveled, the fare increased by a mean of $7.13. Or, reduced: for every 1 mile traveled, the fare increased by a mean of $2.00.

- Produced output (Predicted vs. Actual fares):
  
|           | Actual Fare | Predicted Fare | Residual  |
|-----------|-------------|----------------|-----------|
| 5818      | $14.0       | $12.356503     | 1.643497  |
| 18134     | $28.0       | $16.314595     | 11.685405 |
| 4655      | $5.5        | $6.726789      | -1.226789 |

![Actual&Predicted](https://github.com/nourlybeque/New-York-TLC-project/blob/516a672709af9145646477dd8c177ea322c0f527/New%20York%20TLC%20project/visuals_TLC/final_scatterplot_TLC.png)



### Correlations within the multiple linear regression model:

Even though, a target variable is "fare_amount", the other independent variables "mean_duration" and "mean_distance" are both highly correlated with the target variable of fare_amount They're also both correlated with each other, with a Pearson correlation of 0.87.

mean_duration - shows the average number of minutes that each taxi ride took.

mean_distance - that captures the average of trip distances for each trip group that shares pickup and dropoff points.

![correlation heatmap](https://github.com/nourlybeque/New-York-TLC-project/blob/59bd5151af37e190d3d7a11b986dab479f95bad1/New%20York%20TLC%20project/visuals_TLC/correlation_heatmap_TLC.png)
