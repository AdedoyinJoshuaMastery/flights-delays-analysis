# ✈️ Flight Delays and Cancellations Analysis

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-green)
![Status](https://img.shields.io/badge/Project-Complete-success)

## Project Overview
Unlock the secrets of flight delays and cancellations with data analysis!  
This project dives into aviation data from the Pacific Northwest to identify key factors and airlines most affected by disruptions. Using **data wrangling**, **data visualization**, and **exploratory data analysis**, we uncover insights that benefit both airlines and passengers.

---

## Dataset
The analysis uses the `pnwflights2022` dataset provided by the ModernDive team, exported as CSV files:

- **flights2022.csv**  
  Contains flight-level information:
  - `dep_time`: Departure time (hhmm format, NA = cancelled flight)  
  - `dep_delay`: Departure delay in minutes (negative = early)  
  - `origin`: Origin airport (SEA or PDX)  
  - `airline`: Carrier/airline name  
  - `dest`: Destination airport (IATA code)  

- **flights_weather2022.csv**  
  Contains flight information plus weather conditions:
  - `visib`: Visibility (miles)  
  - `wind_gust`: Wind gust speed (mph)  

---

## Key Questions
1. Which airlines and routes (e.g., "PDX-SFO") are most affected by flight delays?  
2. What impact does wind have on departure delays?  

---

## Project Instructions
- Load the two CSV files into separate DataFrames.  
- Create new columns where necessary to support analysis.  
- For **routes**: calculate average departure delays and number of cancellations → `routes_delays_cancels`.  
- For **airlines**: calculate average departure delays and number of cancellations → `airlines_delays_cancels`.  
- Visualizations:
  - `top9_route_cancels_bar`: Top 9 routes with highest cancellations.  
  - `top9_airline_delays_bar`: Top 9 airlines with highest average delays.  
- Determine if wind gusts ≥ 10 mph increase average departure delays at SEA and PDX → `wind_response`.

---

## Folder Structure
flight-delays-analysis/
│
├── data/                  # Raw datasets
│   ├── flights2022.csv
│   └── flights_weather2022.csv
│
├── notebooks/             # Jupyter notebooks
│   └── flight_delays_analysis.ipynb
│
├── images/                # Saved plots
│   ├── top9_route_cancels_bar.png
│   └── top9_airline_delays_bar.png
│
├── README.md              # Project overview
└── requirements.txt       # Python dependencies


---

## Technologies Used
- Python (Pandas, NumPy)
- Matplotlib
- Jupyter Notebook (Google Colab)

---

## How to Run
1. Clone the repository.  
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt

3.Open the notebook in Jupyter/Colab.

4.Run the cells to reproduce the analysis.

##Results
1.Identified airlines and routes most prone to delays and cancellations.

2.Visualized top 9 routes with cancellations and top 9 airlines with delays.

3.Determined wind gusts ≥ 10 mph impact departure delays differently at SEA and PDX.