# Project Background

New York City TLC is an agency responsible for licensing and regulating New York City's taxi cabs and for-hire vehicles. The agency has requested for developing a regression model that helps estimate taxi fares before the ride, based on data that TLC has gathered. The TLC data comes from over 200,000 taxi and limousine licensees, making approximately one million combined trips per day. This project focuses on predicting taxi fares before a ride using **Multiple Linear Regression**. The goal is to analyze various trip-related features to estimate the fare cost. 

Insights and recommendations are provided on the following key areas:

- **Category 1:** 
- **Category 2:** 
- **Category 3:** 
- **Category 4:** 

The Python EDA used to inspect and clean the data for this analysis can be found here [link].

The Python A/B testing  regarding various business questions can be found here [link].

The Python with multiple linear regression model used to report and explore sales trends can be found here [link].

Tableau dashboard is here



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

Explain the overarching findings, trends, and themes in 2-3 sentences here. This section should address the question: "If a stakeholder were to take away 3 main insights from your project, what are the most important things they should know?" You can put yourself in the shoes of a specific stakeholder - for example, a marketing manager or finance director - to think creatively about this section.

[Visualization, including a graph of overall trends or snapshot of a dashboard]




# Insights Deep Dive
### Category 1:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 1]


### Category 2:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 2]


### Category 3:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 3]


### Category 4:

* **Main insight 1.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 2.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 3.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.
  
* **Main insight 4.** More detail about the supporting analysis about this insight, including time frames, quantitative values, and observations about trends.

[Visualization specific to category 4]



# Recommendations:

Based on the insights and findings above, we would recommend the [stakeholder team] to consider the following: 

* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  
* Specific observation that is related to a recommended action. **Recommendation or general guidance based on this observation.**
  


# Assumptions and Caveats:

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

* Assumption 1 (ex: missing country records were for customers based in the US, and were re-coded to be US citizens)
  
* Assumption 1 (ex: data for December 2021 was missing - this was imputed using a combination of historical trends and December 2020 data)
  
* Assumption 1 (ex: because 3% of the refund date column contained non-sensical dates, these were excluded from the analysis)

