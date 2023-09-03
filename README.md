# Minimizing Road Accidents on Rainy Days

A research that investigates the impact of rainy days on road accidents and how to minimize it


### Introduction

On a global scale, Singapore ranked **fifth** in the estimated road traffic death rate per 100,000 vehicles (OECD, 2019). 

<img src= "Images/global_stats.jpg" width="800" height="400">

This ranking is alarming, considering Singapore's figure is much higher than that of geographically enormous countries like the USA, Canada and Australia. 

Within Singapore, **50% of overall road fatalities are motorcyclists and pillion riders**, and **50% of pedestrian fatalities are the elderly**. 

<img src= "Images/national_stats.jpg" width="600" height="300">

These statistics emphasize the urgent need for Singapore to address road safety comprehensively.



### Problem Statement

Rainy weather can impede our navigation skills on the road, either due to reduced visibility or more slippery surfaces. 

To what extent does weather play a part in road safety? How can we minimize road accidents stemmed from rainy weather?


### Purpose

As a leader in the climate research space, *DSI 39* spearheaded this research to explore the **relationship between rainy days and the number of road accident casualties**. Recommendations are proposed to the relevant goverment organizations based on the findings of the research. This research aims to discover:

* The effect of **rainy days** on the **number of road accident casualties** (correlation between number of rainy days vs casualties per month)
* Whether rainy weather **aggravates** road accidents (correlation between number of rainy days vs fatalities, number of rainy days vs injured per month)
* The **vehicle types** that are more prone to road accidents (rank number of casualties by vehicle types)


### Methodology

* The research analysis spanned a ten-year period from January 2010 to December 2019.
* Data sets were aggregated on a monthly basis over this ten-year period to neutralize the effect of irregular weather phenomena, such as the El Niño event in 2015-2016,  and instances of intense rainfall/flooding in Jun 2010, Jan 2011, and Jan 2018.
* Data from 2020 onwards were excluded due to the effects of the COVID-19 pandemic.
* Data related to Personal Mobile Devices (PMD) were excluded since PMDs came into existence in Singapore only from 2017 onwards.


### Data sets used
To investigate the correlation between rainy days and road accidents, we utilized the following datasets (click on the hyperlinks to access):

#### <a href= "Data sources/raindays_by_mth.csv"> Number of Rainy Days per Month (Jan 2010 - Dec 2019) </a>

* 121 rows, 2 columns; illustrates the no. of rainy days per month from Jan 2010 to Dec 2019

* We chose to use the number of rainy days rather than the specific amount of rainfall because it provides a better indication of how road accidents may be affected by the frequency of rain.

#### <a href= "Data sources/road_acc_by_mth.csv"> Number of Casualties: Fatalities and Injuries (Jan 2010 - Dec 2019) </a>

* 120 rows, 29 columns; illustrates the no. of road accident casualties fatalities and injured, as well as a breakdown of those by vehicle type 

* The total number of casualties (the sum of fatalities and injuries) was used as a relative measure of road accidents.

* We also examined the total fatalities and total injuries to assess the severity of accidents.

* To identify which vehicle types are more susceptible to road accidents, we tabulated the total number of casualties across each vehicle type.

### Data dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|total_rainfall|float|rainfall-monthly-total|Total rainfall in mm|
|date|object|raindays_by_mth & road_acc_by_mth|Date in YYYY-MM format|
|yr|integer|raindays_by_mth & road_acc_by_mth|Year in YYYY format|
|mth|integer|raindays_by_mth & road_acc_by_mth|Month in MM format|
|rain_days|integer|raindays_by_mth|No. of rainy days in a month|
|log_raindays|float|raindays_by_mth|Log (base-10) of rain_days|
|total_deaths|integer|road_acc_by_mth|Total road accident casualties fatalities|
|total_injured|integer|road_acc_by_mth|Total road accident casualties injured|
|total_cas|integer|road_acc_by_mth|Sum of total_deaths and total_injured|
|log_deaths|float|road_acc_by_mth|Log (base-10) of total_deaths|
|log_injured|float|road_acc_by_mth|Log (base-10) of total_injured|
|log_cas|float|road_acc_by_mth|Log (base-10) of total_cas|
|buses, cyclists_&_ pillions, goods_vans, lorries, motor_cars_and_station_wagons, motor_cyclists_&_ pillion_riders, pedestrians, pick_ups, tipper_trucks, trailers, others|integer|road_acc_by_mth|Number of casualties of the respective vehicle type|
 
 ### Conclusion
 
 * The correlation between the number of rainy days and total casualties was **0.72** (after removing the outlier, Feb 2014). This implies that rainy days have a **significant impact** on the number of road accident casualties.
 
 * The correlation of rainy days vs fatalities, and rainy days vs injured were -0.03 and 0.65 respectively. This shows that rainy days have a greater effect on **injuries but not fatalities**.
 
 * Fatalities were likely affected by **other factors**, such as drink driving, failure to adhere to traffic rules, jaywalking etc (Motorist.sg, 2020).
 
 * **Jan, Mar and Apr** (Northeast Monsoon season with the exception of Feb being the dry period) consistently had high number of casualties with relatively high number of rainy days. Though articles on Singapore road accident causes stated only human error reasons (Direct Asia, 2022; Motorist.sg, 2018), **the strong correlation suggests that rainy weather might have elevated those human error and resulted in road accident injuries**.  
 
 * The top three vehicle types that had apparently higher number of casualties were **1. motorcyclists and pillion riders, 2. motor cars and station wagons and 3. pedestrians**.
 
 * During the **Northeast Monsoon**, the respective **government organizations** should practise more stringent road safety measures tailored to **motorcyclists and pillion riders, motor cars and station wagons and pedestrians**

### Recommendations
The table below proposes some targeted road safety measures:

<img src= "Images/recommendations.jpg">

### Limitations
1. Accuracy of research
	As this research uses an aggregated number of rainy days per month, there was no clear indication of which road accidents occurred on a rainy day. For a more accurate analysis, the total number of casualties on rainy days should be used.

2. Limited analysis on other factors
	With a focus on analysing the impact of wet weather on road accidents, this research does not take into account other factors that could be the primary reason of road accidents. A seperate research looking into the common human errors should be conducted in order to implement more comprehensive road safety measures.

3. Lack of geolocation data
	There is a lack of updated geolocation data that illustrates areas in Singapore that are more susceptible to road accidents. This is another variable worth investigating into to refine those road safety measures.

### References
- https://www.budgetdirect.com.sg/car-insurance/research/road-accident-statistics-in-singapore
- https://www.directasia.com/blog/reduce-risk-road-accidents-singapore
- https://www.motorist.sg/article/173/the-5-most-common-causes-for-road-accidents-in-singapore
- https://msgt.com.sg/accident-hotspots-in-singapore-to-watch-out-for/
- http://www.smj.org.sg/article/geospatial-analysis-severe-road-traffic-accidents-singapore-2013%E2%80%932014
- https://tablebuilder.singstat.gov.sg/
- https://www.weather.gov.sg/wp-content/uploads/2020/03/Annual-Climate-Assessment-Report-2019.pdf


