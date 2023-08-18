# Demand Forecasting - Bike Rentals

### Project Overview
---
The growing awareness of the importance of exercise alongside the increasing recognition of the impacts of global warming has prompted a notable surge in individuals opting for bicycle commutes whenever feasible.
However, not everyone willing to partake in bicycle commuting either owns or desires to own a bicycle.
This has led to the creation of several bike-sharing enterprises, facilitating convenient and affordable bike rentals for users.

Since the bicycle commuting culture is still evolving, accurately estimating the demand for bikes on any given day presents a formidable challenge for bike-sharing companies. The primary objective of this project is to gain comprehensive insights into the complexities associated with forecasting bike demand, while also comparing the efficacy of diverse machine learning-based forecasting methodologies.

By accurately predicting the demand for bikes on any given day, bike-sharing companies can optimize their operations, ensuring an adequate supply of bicycles at high-demand locations and periods. This proactive approach eliminates the frustration of potential riders facing unavailability, thus enhancing overall user experience and satisfaction.

This would ultimately serve as a catalyst for the growing trend of bicycle commuting, advancing the global movement towards sustainability.



### Dependencies
---
OS: macOS Ventura 13.4.1
Python Version: 3.8.10
Python Libraries (please refer requirements.txt):
- pandas
- numpy
- statsmodels
- scipy
- scikit-learn
- matplotlib
- seaborn
- plotly


### Getting Started
---


### Dataset Description
---
This is what each variable in our dataset means:

**Capital Bikeshare Data**
- ride_id -  includes ID number of the ride
- rideable_type - indicates whether the type of bike was "classic", "docked" or "electric"
- started_at - includes start date and time
- ended_at - includes end date and time
- start_station_name - includes starting station name
- start_station_id - includes starting station number
- end_station_name - includes ending station name
- end_station_id - includes ending station number
- start_lat - includes starting station latitude
- start_lng - includes starting station longitude
- end_lat - includes ending station latitude
- end_lng - includes ending station longitude
- member_casual -  indicates whether user was a "registered" member or a "casual" rider

**Weather Data**
- station - station ID
- name - name of weather station
- date - date of obseravtion
- avg_wind_speed - average wind speed
- num_days_multiday_prcp - number of days included in the multiday precipitation total 
- multiday_prcp - multiday precipitation total
- peak_gust_time - peak gust time
- prcp - precipitation
- snowfall - snowfall
- snowdepth - snow depth
- temp_avg - average temperature
- temp_max - maximum temperature
- temp_min - minimum temperature
- temp_obs - temperature at the time of observation
- dir_fastest_2min_wind - direction of fastest 2-minute wind
- dir_fastest_5min_wind - direction of fastest 5-minute wind
- speed_fastest_2min_wind - fastest 2-minute wind speed
- speed_fastest_5min_wind - fastest 5-minute wind speed
- wt: weather type
	- wt_fog - fog, ice fog, or freezing fog (may include heavy fog)
	- wt_heavy_fog - heavy fog or heaving freezing fog (not always distinguished from fog)
	- wt_thunder - thunder
	- wt_sleet - ice pellets, sleet, snow pellets, or small hail
	- wt_hail - hail
	- wt_glaze - glaze or rime
	- wt_smoke - smoke or haze
	- wt_drift_snow - blowing or drifting snow
	- wt_high_winds - high or damaging winds
	- wt_mist - mist
	- wt_drizzle - drizzle
	- wt_freeze_drizzle - freezing drizzle
	- wt_rain - rain (may include freezing rain, drizzle, and freezing drizzle)
	- wt_freeze_rain - freezing rain
	- wt_snow - snow, snow pellets, snow grains, or ice crystals
	- wt_ground_fog - ground fog
	- wt_freeze_fog - ice fog or freezing fog

**Holiday Data**
- date - date
- weekend - indicates whether it was a weekend
- holiday - indicates whether it was a holiday
- weekend_holiday - indicates whether it was either a weekend or a holiday



### ML Forecasting Methods
---
**Baseline Models**
- Our first baseline model is a Naive model. Since we intend to provide short-term forecasts, our first baseline model will assume that the predicted value at time `t` will be equal to the actual value of demand at time `t-1`.
- In our second baseline model we extract the trend and seasonalities from our training data and use them to forecast demand.



### Results
---
- Baseline Model 1: MSE = 5,933,717
- Baseline Model 2: MSE = 11,349,103

### Limitations
---


### Licensing, Authors, Acknowledgements
---
The data for this analysis has been curated from the following sources:

- [Capital Bike Share](https://www.capitalbikeshare.com/system-data): this includes the bike demand data for the metro DC area
- [NOAA's National Climatic Data Center](https://www.ncdc.noaa.gov/cdo-web/search): this includes the weather data for the metro DC area
- [DC Department of Human Resources](https://edpm.dc.gov/issuances/legal-public-holidays-2023/): this includes the holiday data for Washington, D.C.




