# Flight Delays and Cancellations – Summary of Findings

## Overview
This analysis investigates flight delays and cancellations in 2022 using two datasets:
- **flights2022.csv** – flight performance data (departure delays, cancellations, routes, airlines).
- **flights_weather2022.csv** – weather conditions (wind gusts, departure delays by airport).

The primary research question was:  
**Which airlines and routes are most affected by flight delays, and what impact does wind have on departure delays?**

---

## Key Findings

### 1. Routes Most Impacted
- Calculated average departure delays and total cancellations for each route.
- **Top 9 routes with the highest cancellations** are visualized in `images/top9_route_cancels_bar.png`.
- Routes with the **highest mean departure delays** were also identified, showing that certain connections consistently experience longer delays.

### 2. Airlines Most Impacted
- Grouped data by airline to measure average departure delays and cancellations.
- **Top 9 airlines with the highest mean departure delays** are visualized in `images/top9_airline_delays_bar.png`.
- Airlines with the highest cancellations were also identified, highlighting operational differences across carriers.

### 3. Weather Impact (Wind Gusts ≥ 10 mph)
- Compared departure delays at **Portland (PDX)** and **Seattle (SEA)** under different wind conditions.
- Findings:
  - At **PDX**, average departure delay increased from ~6.7 minutes (<10 mph) to ~9.1 minutes (≥10 mph).
  - At **SEA**, average departure delay increased from ~7.9 minutes (<10 mph) to ~9.2 minutes (≥10 mph).
- Conclusion: **Wind gusts of 10 mph or more are associated with higher average departure delays at both airports.**  
  (Result stored in `wind_response = True`.)

---

## Conclusions
- Certain **routes and airlines** are disproportionately affected by delays and cancellations, suggesting operational or logistical challenges.
- **Weather conditions**, specifically wind gusts ≥10 mph, contribute to longer delays at major airports like SEA and PDX.
- The analysis provides actionable insights for airlines, airports, and passengers:
  - Airlines can target operational improvements on high-delay routes.
  - Passengers may anticipate longer delays when traveling through wind-prone airports.



