# Demand Forecasting - Bike Rentals

### Project Overview
---
The growing awareness of the importance of exercise alongside the increasing recognition of the impacts of global warming has prompted a notable surge in individuals opting for bicycle commutes whenever feasible.
However, not everyone willing to partake in bicycle commuting either owns or desires to own a bicycle.
This has led to the creation of several bike-sharing enterprises, facilitating convenient and affordable bike rentals for users.

Since the bicycle commuting culture is still evolving, accurately estimating the demand for bikes on any given day presents a formidable challenge for bike-sharing companies.
**The primary objective of this project is to gain comprehensive insights into the complexities associated with forecasting bike demand, while also comparing the performance of the following forecasting methods -**

- [x] **XGBoost**
- [x] **ARIMA**
- [x] **SARIMA**
- [ ] **RNN**

Baseline has been established using two methods -

- **Naïve Forecasting Method**: Since we intend to provide short-term forecasts, our first baseline model will assume that the predicted value at time `t` will be equal to the actual value of demand at time `t-1`.
- **Seasonal Decomposition**: In our second baseline model we extract the trend and seasonalities from our training data and use them to forecast demand.

The Jupyter Notebooks in this repository have been labelled stepwise and should be followed in order -

- step_1_data_preparation.ipynb
- step_2_exploratory_data_analysis.ipynb
- step_3_modeling.ipynb


### Dependencies
---
**OS**: macOS Ventura 13.4.1

**Python Version**: 3.8.10

**Python Libraries** (please refer requirements.txt):
- pandas
- numpy
- statsmodels
- scipy
- scikit-learn
- matplotlib
- seaborn
- plotly
- xgboost
- joblib


### Dataset Description
---
This has been moved under the "Data" folder.


### Results
---
- **Baseline Model 1 (Naïve model)**
	- MAPE = 0.278 %
	- RMSE = 2710

- **Baseline Model 2 (Seasonal decomposition based)**
	- MAPE = 0.304 %
	- RMSE = 2672

- **XGBoost**
	- MAPE = 0.178 %
	- RMSE = 1970

- **ARIMA**
	- MAPE = 
	- RMSE = 

- **SARIMA**
	- MAPE = 
	- RMSE = 

### Next Steps
---


### Licensing, Authors, Acknowledgements
---
The data for this analysis has been curated from the following sources:

- [Capital Bike Share](https://www.capitalbikeshare.com/system-data): this includes the bike demand data for the metro DC area
- [NOAA's National Climatic Data Center](https://www.ncdc.noaa.gov/cdo-web/search): this includes the weather data for the metro DC area
- [DC Department of Human Resources](https://edpm.dc.gov/issuances/legal-public-holidays-2023/): this includes the holiday data for Washington, D.C.




