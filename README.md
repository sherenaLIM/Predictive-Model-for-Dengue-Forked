<img src="./images/GA-logo.png" style="float: left; margin: 20px; height: 55px">

# Predictive Model for Dengue

<br>

    
**Primary Objectives:**

1. yada yada
2. yada yada

----

## Background & External Research

Introduction <br>

Dengue virus is most commonly spread to humans through infected mosquitos. Dengue can range from asymptomatic infection or mild illness to severe disease. An estimated 1 in 4 dengue virus infections are symptomatic. Symptomatic dengue virus infection most commonly presents as a mild to moderate, nonspecific, acute febrile illness. Approximately 1 in 20 patients with dengue virus disease progress to develop severe, life-threatening disease called severe dengue. The second infection with DENV is a risk factor for severe dengue. Severe dengue can be life-threatening within a few hours and often requires care at a hospital.

Singapore launched a comprehensive nationwide programme in 1968 targeting the Aedes mosquito, the main mosquito vector of dengue. This control programme combines environmental management, source reduction, public health education and law enforcement. Since then, the number of homes found to be breeding Aedes mosquito fell sharply and remains low.

However, Dengue remains endemic in Singapore. Since the 1990s, there have been periodic spikes in cases occurring in five- to six-year cycles. The spike in 2019 and 2020 could be a case in point, coming after the epidemics in 2013 and 2014, which saw over 22,000 and 18,000 cases respectively. 

Several theories have been proposed to explain this cyclical pattern. <br> 
> 1. The dengue virus has four different serotypes, and a switch in the predominant virus serotype has been a historical precursor of dengue epidemics in Singapore. For example, two large epidemics, each stretching over two years in 2004–2005 and 2013–2014, were associated with a switch in the main dengue virus serotype from serotype 2 to serotype 1.
> 2. Dengue in Singapore typically rises in warmer months, from April, peaking in July or August, before declining in September or October. Abnormal climate changes, such as the El Niño weather phenomenon, may affect the mosquito breeding environment, accelerate the life-cycle of Aedes mosquito, shorten the incubation period of the dengue virus and drive up cases. El Nino, a recurring weather pattern related to the warming of surface waters in the Pacific Ocean, last occurred in 2015 and 2016. It is slated to resume in 2023. 
> 3. Population factors also contribute to this endemic. The decrease in dengue transmission due to the successful implementation of the Aedes control programme in the 1970s and 1980s reduced incidence of dengue infection in the population. As herd immunity to dengue is consequently low, a large proportion of the Singapore resident population today remains susceptible to infection by any of the four dengue serotypes.

----

## Problem Statement

Problem Statement <br>

Given weather, location, and infection data, you have been tasked to predict when and where different species of mosquitos will test positive for DENV virus. A more accurate method of predicting outbreaks of Dengue virus in mosquitos will help MOH allocate resources more efficiently and effectively towards preventing transmission of this potentially life-threatening virus.

Stakeholders <br>

Primary stakeholders: Ministry of Health, Singapore (MOH) <br>
Secondary stakeholders: General Public for Awareness, Manufacturer of Mosquito Traps / Airborne Pesticides.

----
## Dataset

#### Provided Data

There are 8 weather datasets included in the [`data`](./data/) folder for this project. These correponds to rainfall, sunshine, humidity, and temperature information. 

* [`rainfall-monthly-highest-daily-total.csv`](./data/rainfall-monthly-highest-daily-total.csv): Monthly highest total daily rainfall from 1982 to 2022, measured in milimeters(mm).
* [`rainfall-monthly-number-of-rain-days.csv`](./data/rainfall-monthly-number-of-rain-days.csv): Monthly number of rain days from 1982 to 2022. A day is considered to have “rained” if the total rainfall for that day is 0.2mm or more.
* [`rainfall-monthly-total.csv`](./data/rainfall-monthly-total.csv): Monthly total rain recorded in mm(millimeters) from 1982 to 2022.
* [`sunshine-duration-monthly-mean-daily-duration`](./data/sunshine-duration-monthly-mean-daily-duration.csv): Mean sunshine hours per month from 1982 to 2022, measured in hours (hrs).
* [`relative-humidity-monthly-mean`](./data/relative-humidity-monthly-mean.csv): Mean relative humidity per month from 1982 to 2022, measured in percentage(%).
* [`surface-air-temperature-annual-mean-daily-minimum`](./data/surface-air-temperature-annual-mean-daily-minimum.csv): Mean daily minimum surface air temperature per year from 1982 to 2022, measure in degrees Celsius(°C).
* [`surface-air-temperature-monthly-mean-daily-minimum`](./data/surface-air-temperature-monthly-mean-daily-minimum.csv): Mean daily minimum surface air temperature per month from 1982 to 2022, measure in degrees Celsius(°C).
* [`wet-bulb-temperature-hourly.csv`](./data/wet-bulb-temperature-hourly.csv): Hourly wet bulb temperature in degrees Celcius(°C) at 100% relative humidity.

#### Additional Data

* insert location data - limitation: 
* insert infection (flu, dengue) data - limitation: 2012 - 2022

----
## Technical Report

The technical report is split into X parts in the `code` folder.

1.
2.
3.
4.

In addition to the Jupyter notebooks, there are X python scripts that contain user-defined functions to aid in the data cleaning and analysis.

1.
2.

----
## Findings and Conclusions

yada yada
