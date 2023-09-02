# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Rainy Days and Road Accident Casualties Analysis

A research that investigates the impact of rainy days on road accidents and how to minimize it

### Introduction

On a global scale, Singapore ranked fifth in the estimated road traffic death rate per 100,000 vehicles (OECD, 2019). 

<img src= "Images/global_stats.jpg">

This ranking is alarming, considering Singapore's figure is much higher than that of geographically enormous countries like the USA, Canada and Australia. 

Within Singapore, 50% of overall road fatalities are motorcyclists and pillion riders, and 50% of pedestrian fatalities are the elderly. 

<img src= "Images/national_stats.jpg">

These statistics emphasize the urgent need for Singapore to address road safety comprehensively.


### Problem Statement

Rainy weather can impede our navigation skills on the road, either due to reduced visibility or more slippery surfaces. 

To what extent does weather play a part in road safety? How can we minimize road accidents stemmed from rainy weather?

### Purpose

As a leader in the climate research space, DSI 39 spearheaded this research to explore the relationship between rainy days and the number of road accident casualties. This research aims to discover:

> * The effect of **rainy days** on the **number of road accident casualties** (correlation between number of rainy days vs casualties per month)
> * Whether rainy weather **aggravates** road accidents (correlation between number of rainy days vs fatalities, number of rainy days vs injured per month)
> * The **vehicle types** that are more prone to road accidents (rank number of casualties by vehicle types)


### Data Sources
To investigate the correlation between rainy days and road accidents, we utilized the following datasets:

#### Number of Rainy Days per Month (Jan 2010 - Dec 2019)

Link to Dataset
> * We chose to use the number of rainy days rather than the specific amount of rainfall because it provides a better indication of how road accidents may be affected by the frequency of rain.

#### Number of Casualties: Fatalities and Injuries (Jan 2010 - Dec 2019)

Link to Dataset

> * The total number of casualties (the sum of fatalities and injuries) was used as a relative measure of road accidents.

> * We also examined the total fatalities and total injuries to assess the severity of accidents.

> * To identify which vehicle types are more susceptible to road accidents, we tabulated the total number of casualties across each vehicle type.

### Methodology
> * The research analysis spanned a ten-year period from January 2010 to December 2019.
> * Data sets were aggregated on a monthly basis over this ten-year period to mitigate the impact of irregular weather phenomena, such as the El Niño event in 2015-2016 and instances of intense rainfall/flooding in June 2010, January 2011, and January 2018.
> * Data from 2020 onwards were excluded due to the disruptive effects of the COVID-19 pandemic.
> * Data related to Personal Mobile Devices (PMD) were excluded since PMDs came into existence in Singapore only from 2017 onwards.

### Outlier

<img src= "Images/outlier.jpg">