# Taxi Trip Data Analysis & Operational Insights

## Project Overview
This project analyzes NYC taxi trip data containing 100,000+ trip records to uncover operational patterns, detect anomalies, and generate business insights that can improve fleet operations and revenue strategies.

The analysis covers the complete analytics pipeline including:
- Data cleaning
- Exploratory data analysis
- Operational insights
- Anomaly detection
- Vendor comparison
- Route analysis

## Business Objective
Taxi companies rely heavily on operational data to optimize driver allocation, improve revenue, and enhance customer experience. 

The goal of this project was to analyze trip-level data and answer critical business questions such as:
- When is the fleet busiest?
- Do payment methods influence tipping behavior?
- Which pickup locations generate the most revenue?
- Are there anomalies or corrupted records affecting analysis?

## Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SQL concepts
- Jupyter Notebook

## Dataset
The dataset contains taxi trip records including:

- Pickup & Dropoff time
- Trip distance
- Passenger count
- Fare amount
- Tip amount
- Payment type
- Vendor ID
- Pickup & Dropoff locations

## Phase 1: Data Cleaning (Dirty Data Audit)

Identified and handled several data quality issues:

- Trips with `trip_distance = 0`
- Negative fare and total amounts affecting revenue calculations
- Trips with `passenger_count = 0`
- Trips where dropoff time occurred before pickup time

After cleaning, 3–5% of corrupted records were removed or corrected to ensure accurate analysis.

## Phase 2: Operational Insights (EDA)

Key operational insights discovered:

- Identified peak demand hours using trip frequency analysis
- Analyzed passenger distribution to understand solo vs group travelers
- Compared tipping behavior between credit card and cash payments
- Evaluated airport trip fares compared to city trips

## Phase 3: Strategic Business Insights

Key recommendations include:

- Evaluating the impact of congestion surcharge on trip demand
- Identifying top 3 pickup locations generating the highest revenue
- Suggested optimal driver allocation zones for peak demand hours

## Phase 4: Advanced Data Engineering

Created additional features:

- Trip duration calculation
- Average speed per trip

Detected and removed unrealistic trips such as:
- Trips with negative duration
- Trips exceeding 100 mph average speed

## Phase 5: Vendor Comparison

Compared two taxi system vendors:

- Vendor 1 (VeriFone)
- Vendor 2 (Creative Mobile)

Analysis showed differences in average tip behavior between the two vendor systems, suggesting UI differences may influence tipping behavior.

## Phase 6: Data Investigation

Investigated 64 unusual records with RateCodeID = 99, which were isolated and analyzed to identify whether they represented:

- `RateCodeID = 99`

These records were isolated and analyzed to identify potential data errors or special trip categories.

## Phase 7: Route Analysis

Created a new route feature (Pickup → Dropoff) and analyzed the most frequent routes.

Key results:

Identified Top 5 most common routes

Determined whether trips were long cross-city journeys or short commuter hops

Provided recommendations for fleet deployment optimization

## Key Insights

- Peak taxi demand occurs during specific hours of the day.
- Credit card users tend to tip more than cash users.
- Certain pickup locations generate significantly higher revenue.
- A small portion of trips contain corrupted data that can distort operational metrics.

## Business Impact

The analysis helps taxi companies:

- Optimize driver allocation
- Improve revenue strategy
- Detect fraudulent or corrupted trip records
- Identify high-value pickup locations

## Vizualization

<img width="600" height="700" alt="Screenshot 2026-03-13 152938" src="https://github.com/user-attachments/assets/742c951e-6394-4fad-9d76-18b3e0c829b6" />
<img width="600" height="700" alt="Screenshot 2026-03-13 152902" src="https://github.com/user-attachments/assets/e82ba473-d682-4082-9c06-e4ced0d519cf" />
<img width="600" height="700" alt="Screenshot 2026-03-13 152834" src="https://github.com/user-attachments/assets/9def9722-f08b-4a17-8384-7a05c1cec136" />
<img width="600" height="700" alt="Screenshot 2026-03-13 152820" src="https://github.com/user-attachments/assets/e66f962f-616c-4e4b-b240-51e9592972ef" />
<img width="600" height="700" alt="Screenshot 2026-03-13 152750" src="https://github.com/user-attachments/assets/f71a681f-82fc-421e-b6f3-9e186e193523" />





















