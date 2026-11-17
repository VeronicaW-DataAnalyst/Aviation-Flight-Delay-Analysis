# Aviation Flight Delay Analysis

## Project Overview

This project analyzes departure delays at Dallas/Fort Worth International Airport (DFW) using 2026 flight data from the Bureau of Transportation Statistics (BTS).

The analysis examines delay patterns across airlines, destinations, departure times, and reported delay causes to identify operational trends and areas where airport or airline teams could focus improvement efforts.

## Business Objective

The primary objective was to answer:

- Which destinations experience the greatest delay impact?
- Which airlines have the highest departure-delay rates?
- How do delays vary throughout the day?
- What are the primary reported causes of departure delays?
- Where could operational resources be prioritized to reduce delays?

## Tools & Technologies

- **Tableau** — Data visualization, interactive dashboards, geographic analysis
- **SQL / MySQL** — Data querying and analysis
- **Excel** — Data validation, cleaning, and preparation
- **Bureau of Transportation Statistics (BTS)** — Primary flight data source
- **OurAirports** — Airport geographic coordinates used for route mapping

## Data

The primary dataset consists of 2026 flight records for DFW International Airport obtained from the Bureau of Transportation Statistics.

Key fields used in the analysis include:

- Flight date
- Airline / carrier
- Origin airport
- Destination airport
- Scheduled departure time
- Actual departure time
- Departure delay
- Delay cause categories
- Flight status

Airport latitude and longitude data from OurAirports were incorporated to support geographic route visualization.

## Data Preparation

The data preparation process included:

1. Reviewing the dataset for missing, inconsistent, and invalid values.
2. Standardizing airport and airline identifiers.
3. Validating airport coordinates used for geographic analysis.
4. Creating calculated fields for delay metrics and departure-time analysis.
5. Validating calculated results against the underlying flight records.
6. Preparing the final dataset for analysis and visualization in Tableau.

## Analysis & Methodology

The analysis focused on several operational dimensions:

### Delay Performance
Calculated the number and percentage of delayed flights, along with total and average departure delay.

### Destination Analysis
Compared destinations based on delayed-flight volume and total delay minutes to identify routes with the greatest overall delay impact.

### Airline Analysis
Compared departure-delay performance across carriers while considering differences in flight volume.

### Time-of-Day Analysis
Analyzed departure delays by scheduled departure hour to identify periods associated with higher average delays.

### Delay Causes
Examined reported causes of delays, including operational and weather-related factors.

### Geographic Analysis
Created a route map connecting DFW with destination airports to provide a geographic view of flight activity and delay performance.

## Key Findings

- **Chicago O'Hare (ORD)** had the highest number of delayed flights among the destinations analyzed, with **1,857 delayed flights** and approximately **107,788 total delay minutes**.
- **LaGuardia (LGA)** ranked fourth in delayed-flight volume but second in total delay minutes, demonstrating that delay impact is not determined by flight volume alone.
- **American Airlines** recorded the highest observed departure-delay rate among the carriers analyzed at approximately **55.95%**. This result should be interpreted alongside American's substantially larger share of flights in the dataset.
- **United Airlines** recorded the lowest observed departure-delay rate among the larger-volume carriers analyzed at approximately **31.68%**.
- Later scheduled departure hours generally showed higher average departure delays, with the **10–11 PM period** among the more delayed periods observed.
- Airline-level results were evaluated alongside flight volume to avoid drawing conclusions from carriers with relatively small sample sizes.

## Business Recommendations

Based on the analysis, aviation operations teams could:

- Prioritize high-impact routes based on total delay minutes rather than delayed-flight count alone.
- Investigate operational conditions affecting late-evening departures.
- Evaluate airline-specific delay patterns while accounting for differences in traffic volume.
- Monitor recurring delay causes to identify opportunities for operational improvement.
- Combine flight-delay data with additional operational and weather data for more comprehensive root-cause analysis.

## Dashboard

The completed Tableau dashboards provide interactive views of:

- Overall delay performance
- Delay by destination
- Airline performance
- Airline × destination performance
- Delay causes
- Delay by time of day
- DFW route activity and geographic distribution

**Tableau Dashboard:** [Insert Tableau Public Link]

**Portfolio Case Study:** [Insert Notion Portfolio Link]

## Project Structure

```text
Aviation-Flight-Delay-Analysis/
│
├── data/
│   └── README.md
│
├── sql/
│   └── analysis.sql
│
├── tableau/
│   └── Aviation_Flight_Delay_Analysis.twbx
│
├── documentation/
│   └── project_documentation.md
│
└── README.md
<img width="768" height="333" alt="UA" src="https://github.com/user-attachments/assets/cf633f10-d29e-4316-a491-2368dab5e5a7" />
<img width="768" height="333" alt="F9" src="https://github.com/user-attachments/assets/8a4826ef-c1fb-49bc-ba8d-38607cbda1c4" />
<img width="768" height="333" alt="DL" src="https://github.com/user-attachments/assets/4b98e920-cd92-4442-b5b1-ee66cf3e9f0b" />
<img width="768" height="333" alt="B6" src="https://github.com/user-attachments/assets/df5614ab-e2fd-4216-ab47-53bd0f854c5b" />
<img width="768" height="333" alt="AA" src="https://github.com/user-attachments/assets/26d106a7-74d0-449f-af86-4f0bddda721e" />
