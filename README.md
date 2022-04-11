# Bike Sharing using Multiple Linear Regression
> A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. A US bike-sharing provider BoomBikes has decided to come up with a mindful business plan to be able to accelerate its revenue.

## Table of Contents
* [General Info](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Business Goal:
The purpose is to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demand varies with different features.

Data Definition
- instant: record index
- dteday : date
- season : season (1:spring, 2:summer, 3:fall, 4:winter)
- yr : year (0: 2018, 1:2019)
- mnth : month ( 1 to 12)
- holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
- weekday : day of the week
- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
+ weathersit : 
    - 1: Clear, Few clouds, Partly cloudy, Partly cloudy
    - 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
    - 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
    - 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
- temp : temperature in Celsius
- atemp: feeling temperature in Celsius
- hum: humidity
- windspeed: wind speed
- casual: count of casual users
- registered: count of registered users
- cnt: count of total rental bikes including both casual and registered


## Conclusions
### Equation obtained from final model:

Y = 782.79 + 2029.01(yr) - 753.31(holiday) + 4938.9(temp) - 1264.48(windspeed) + 705.35(season_summer) + 1095.77(season_winter) + 777.92(mnth_sep) - 2203.34(weathersit_light_rain) 

We can see there are a few that contribute positively towards the demand and some variables that negatively influence the demand.

### Variables that contribute positively and their coefficients

- temp --> 4938.90
- yr --> 2029.01
- season_winter --> 1095.77
- mnth_sep --> 777.92
- season_summer --> 705.35

### Variables that contribute negatively and their coefficients

- weathersit_light_rain --> -2203.34
- windspeeed --> -1264.48
- holiday --> -753.31


## Technologies Used
- Python - version 3.0
- Pandas
- Numpy
- Seaborn


## Contact
Created by [@Vedakashyap7] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
