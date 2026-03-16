# Uber Ride Demand Analysis

## Project Overview

In today’s dynamic urban transportation systems, ride-hailing services like **Uber** play a critical role in providing flexible mobility solutions. However, even popular services face operational challenges, particularly during high-demand hours.

This project analyzes Uber ride request data to identify patterns related to **trip cancellations, driver unavailability, and peak-time inefficiencies**.

The analysis combines **Exploratory Data Analysis (EDA) using Python** and **insight extraction using SQL queries** to uncover operational bottlenecks and suggest data-driven improvements.

---

## Problem Statement

Uber faces frequent **trip cancellations and unavailability of cars during peak hours**, especially for **airport pickups**.  

The objective of this project is to analyze ride request data to identify demand patterns, supply shortages, and the key causes of trip failures.

---

## Tools & Technologies

- Python (Pandas, Seaborn, Matplotlib)
- Jupyter Notebook
- MySQL
- Excel

---

## Dataset Overview

The dataset contains **6,745 Uber ride request records** with the following key fields:

- Request Timestamp
- Pickup Point (City or Airport)
- Status (Trip Completed, Cancelled, No Cars Available)
- Trip Duration

Additional derived features were created for deeper analysis:

- Request Hour
- Day
- Time Slot

The dataset was initially cleaned using **Excel**, then analyzed using **Python libraries** in Jupyter Notebook. SQL queries were executed after importing the data into **MySQL**.

---

## Data Cleaning & Preparation

Data preprocessing included:

- Converting timestamps into usable datetime formats
- Extracting request hour and day for time-based analysis
- Creating time slots for demand pattern analysis
- Handling missing or inconsistent values

These steps ensured accurate analysis of ride demand patterns.

---

## Exploratory Data Analysis (Python)

EDA was conducted using **Pandas, Seaborn, and Matplotlib** to identify ride demand patterns.

### Demand Peaks During Office Hours
Ride requests show clear spikes during:

- **Morning commute:** 5 AM – 9 AM
- **Evening commute:** 5 PM – 9 PM

These hours consistently show the highest demand across both city and airport pickup points.

---

### Airport Cancellations

Airport pickup requests experienced **significantly higher cancellation rates**, particularly during morning hours.

This indicates operational challenges in serving airport trips during peak demand.

---

### Trip Duration Patterns

The **average trip duration increases during evening hours**, likely due to heavy traffic conditions.

---

### No Cars Available During Rush Hours

A large number of ride requests resulted in **"No Cars Available"** during peak commute hours.

This indicates a significant **supply-demand gap**, where available drivers cannot meet passenger demand.

---

## SQL-Based Insights

SQL queries were used to validate patterns identified during Python EDA.

Key insights include:

- Only **~40% of total ride requests were successfully completed**
- More than **50% of airport pickup requests during peak morning hours were cancelled**
- Average trip duration during evening hours was **20–25% higher than morning trips**

These insights confirm operational inefficiencies during peak demand periods.

---

## Key Findings

- Ride demand peaks during **morning and evening commute hours**
- Airport pickups experience **higher cancellation rates**
- Driver availability is insufficient during **rush hours**
- Evening trips take longer due to **traffic congestion**

---

## Recommendations

Based on the analysis:

- Increase **driver availability during peak commute hours**
- Implement **airport-specific driver allocation strategies**
- Introduce **dynamic incentives for drivers during high-demand periods**
- Improve demand forecasting using historical ride data

---

## Conclusion

This analysis highlights major operational challenges in Uber’s ride request system, particularly during peak hours and airport pickups. By identifying supply-demand mismatches and ride cancellation patterns, the project provides insights that can help ride-hailing platforms optimize driver allocation and improve service reliability.

---

## Repository Structure

- README.md
- dataset
- uber_analysis.ipynb
- SQL_queries.sql
- visualizations
