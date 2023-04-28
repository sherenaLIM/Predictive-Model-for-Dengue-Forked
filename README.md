<img src="./images/GA-logo.png" style="float: left; margin: 20px; height: 55px">

# Predictive Model for Dengue

<br>

    
**Primary Objectives:**

1. yada yada
2. yada yada

----

## Background & External Research

Introduction <br>

Dengue virus is most commonly spread to humans through infected mosquitos. Dengue can range from asymptomatic infection or mild illness to severe disease. An estimated 1 in 4 dengue virus infections are symptomatic. Symptomatic dengue virus infection most commonly presents as a mild to moderate, nonspecific, acute febrile illness. Approximately 1 in 20 patients with dengue virus disease progress to develop severe, life-threatening disease called severe dengue. Severe disease (dengue hemorrhagic fever [DHF] / dengue shock syndrome [DSS]) can be induced by all four dengue virus (DENV) types (DENV-1, DENV-2, DENV-3, and DENV-4).

Singapore launched a comprehensive nationwide programme in 1968 targeting the Aedes mosquito, the main mosquito vector of dengue. This control programme combines environmental management, source reduction, public health education and law enforcement. Since then, the number of homes found to be breeding Aedes mosquito fell sharply and remains low. 

In 2016, Singapore embarked on a multi-phased field study named Project Wolbachia. Project Wolbachia involves the release of male mosquitoes infected with the Wolbachia bacteria. When these specially bred mosquitoes mate with urban female Aedes aegypti that do not carry Wolbachia, their resulting eggs do not hatch.

Despite concerted efforts, Dengue remains endemic in Singapore. Since the 1990s, there have been periodic spikes in cases occurring in five- to six-year cycles. The spike in 2019 and 2020 could be a case in point, coming after the epidemics in 2013 and 2014, which saw over 22,000 and 18,000 cases respectively. 

Several theories have been proposed to explain this cyclical pattern. <br> 
> 1. The dengue virus has four different serotypes, and a switch in the predominant virus serotype has been a historical precursor of dengue epidemics in Singapore. For example, two large epidemics, each stretching over two years in 2004–2005 and 2013–2014, were associated with a switch in the main dengue virus serotype from serotype 2 to serotype 1.
> 2. Dengue in Singapore typically rises in warmer months, from April, peaking in July or August, before declining in September or October. Abnormal climate changes, such as the El Niño weather phenomenon, may affect the mosquito breeding environment, accelerate the life-cycle of Aedes mosquito, shorten the incubation period of the dengue virus and drive up cases. El Nino, a recurring weather pattern related to the warming of surface waters in the Pacific Ocean, last occurred in 2015–2016. It is slated to resume in 2023. 
> 3. Population factors also contribute to this endemic. The decrease in dengue transmission due to the successful implementation of the Aedes control programme in the 1970s and 1980s reduced incidence of dengue infection in the population. As herd immunity to dengue is consequently low, a large proportion of the Singapore resident population today remains susceptible to infection by any of the four dengue serotypes.

The entire lifecycle of an aedes female mosquito spans for about 42-56 days: <br>
<div>
<img src="images/mosquito_chain.png" width="300"/>
</div>

References <br> 
> * Centers for Disease Control and Prevention, National Center for Emerging and Zoonotic Infectious Diseases (NCEZID), Division of Vector-Borne Diseases (DVBD); url: https://www.cdc.gov/dengue/symptoms/index.html
> * National Centre for Infectious Diseases (2023). url: https://www.ncid.sg/Health-Professionals/Articles/Pages/Rise-in-dengue-cases-underscores-need-for-constant-vigilance.aspx#:~:text=Singapore%20is%20in%20the%20midst,the%202%2C772%20cases%20in%202017.
> * Meteorological Service Singapore (2023). url: http://www.weather.gov.sg/climate-el-la/
> * Mosquitos and Mosquito Borne diseases (NEA). url: https://www.nea.gov.sg/docs/default-source/resource/section-a---mosquitoes-amp-mosquito-borne-diseases-pdf-1-41-mb-.pdf
----

## Problem Statement

Problem Statement <br>

Given infection and serology, climate, geospatial, and google trends data, you have been tasked to predict the national-level dengue cases 2 weeks into the future. A more accurate method of predicting outbreaks of Dengue virus in mosquitos will help MOH plan when and where to allocate resources for dengue control more effectively. If cases are expected to rise sharply, there is a need to plan for more intensive control and enforcement measures to reduce mosquito breeding and consequentially dengue cases. Also quantify the costs and benefits of such control measures.

Stakeholders <br>

- Primary stakeholder(s): Ministry of Health (MOH), National Environment Agency (NEA), National Center of Infectious Diesease (NCID) <br>
>  * Public Health Prevention Awareness Campaigns 
>  * Mosquito Fogging Services 
>  * Airborne Pesticides
>  * Wolbachia Mosquitos Project
>  *  Mosquito Traps

- Secondary stakeholders: General Public for Awareness, Suppliers of Dengue Prevention Solutions

----
## Dataset

Dengue Infection Rate and Serology Data:  <br>
* [Number of Dengue cases from 2018 to 2020](https://www.moh.gov.sg/resources-statistics/infectious-disease-statistics/2020/weekly-infectious-diseases-bulletin)<br>
* [Number of Dengue cases in 2021](https://www.moh.gov.sg/resources-statistics/infectious-disease-statistics/2021)<br>
* [Number of Dengue cases in 2022](https://www.moh.gov.sg/resources-statistics/infectious-disease-statistics/2022)<br>
* [Number of Dengue cases in 2023](https://www.moh.gov.sg/resources-statistics/infectious-disease-statistics/2023/weekly-infectious-diseases-bulletin)<br>
* [Serology data for Dengue between 2018 to 2023](https://www.nea.gov.sg/dengue-zika/dengue/quarterly-dengue-surveillance-data)<br>

Climate Data (1980 - 2023, planning area included): <br> 
* [Daily historical climate data 1980 to 2023](http://www.weather.gov.sg/climate-historical-daily)<br>

Geospatial Data:  <br> 
* [Weekly geospatial dengue cluster data 2015 to 2020](https://outbreak.sgcharts.com/)

Google Trends Data:  <br>
* [Weekly Google Trends data for dengue 2018 to 2023](https://trends.google.com/trends/explore?date=today%205-y&geo=SG&q=repellent%20%2B%20dengue%20fever%20%2B%20Dengue%20cluster%20%2B%20mosquito%20%2B%20mosquito%20repellent%20%2B%20dengue%20%2B%20aedes&hl=en)

Cost Data: <br> 
(yada
yada) 

## Data Dictionary
**Climate, serology and google search Data Dictionary**
|Variable|Description|Data type|
|--|--|--|
|time|Date of the dengue data, taken at sunday of every week from 2018 to 2023|datetime|
|dengue_cases|Weekly total number of dengue cases in NEA Weekly Infectious Diseases Bulletin|int|
|denv_1|Weekly percentage of dengue cases belonging to serotype DENV_1 obtained by NEA dengue surveillance|float|
|denv_2|Weekly percentage of dengue cases belonging to serotype DENV_2 obtained by NEA dengue surveillance|float|
|denv_3|Weekly percentage of dengue cases belonging to serotype DENV_3 obtained by NEA dengue surveillance|float|
|denv_4|Weekly percentage of dengue cases belonging to serotype DENV_4 obtained by NEA dengue surveillance|float|
|Mean Temperature (°C)|Weekly average temperature in °C in Changi from 1980 to 2023 |float|
|Mean Wind Speed (km/h)|Weekly average wind speed in km/h in Changi from 1980 to 2023 |float|
|Daily Rainfall Total (mm)|Weekly averaged daily total rainfall in millimeters in Changi from 1980 to 2023 |float|
|Maximum Temperature (°C)|Weekly highest temperature in °C in Changi from 1980 to 2023 |float|
|Max Wind Speed (km/h)|Weekly highest wind speed in km/h in Changi from 1980 to 2023 |float|
|Minimum Temperature (°C)|Weekly lowest temperature in °C in Changi from 1980 to 2023 |float|
|google_trends|Weekly number of searches for dengue related terms in Singapore scaled on a range of 0 to 100|int|
    
**Geospatial Data Dictionary**

|Region|latitude|logitude|
|--|--|--|
|CENTRAL REGION|103.8404361073424| 1.354955429489439|
|EAST REGION|103.9633839670078| 1.32796829772857|
|NORTH REGION|103.8371178947091| 1.415039440959387|
|NORTH-EAST REGION|103.8678180616185| 1.365201551765161|
|WEST REGION|103.7049024145101| 1.341611988409421|

<br>

|Variable|Description|Data type|
|--|--|--|
|date|Date of the cluster data from 2015 to 2020 from NEA |datetime|
|recent_cases_in_cluster_central|Weekly sum of average dengue cases (onset in the last 2 weeks) of clusters in central region of Singapore from 2015 to 2020|int|
|recent_cases_in_cluster_east|Weekly sum of average dengue cases (onset in the last 2 weeks) of clusters in East region of Singapore from 2015 to 2020|int|
|recent_cases_in_cluster_north|Weekly sum of average dengue cases (onset in the last 2 weeks) of clusters in North region of Singapore from 2015 to 2020|int|
|recent_cases_in_cluster_north-east|Weekly sum of average dengue cases (onset in the last 2 weeks) of clusters in Nort-East region of Singapore from 2015 to 2020|int|
|recent_cases_in_cluster_west|Weekly sum of average dengue cases (onset in the last 2 weeks) of clusters in West region of Singapore from 2015 to 2020|int|

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

**Cost Benefit Analysis** <br>
There are currently various measures deployed in Singapore to control the dengue cases, which can be categorized into reactive and preventive measures.
* Reactive Measures: Distribution of mosquito repellent, fogging
* Preventive Measures: Home inspections, anti-dengue campaigns, gravi-traps, project wolbachia

For our project, we will be focusing on the cost and benefit of Project Wolbachia.<br>
*Economic Impact of Dengue* <br>
* Over $1 Billion annually between 2010 to 2020
* For years with huge spikes like 2020 and 2022, the expected economic impact is much higher

*Project Wolbachia* <br>
* Nation-wide deployment throughout the year is expected to cost approx. $108 Million
* A reduction of up to 88% of dengue cases is observed before deployment of Project Wolbachia
* Effectiveness of the project is not dependent on people compared to other measures, which replies on the population's due diligence to contain dengue mosquitos
* Requires 3 - 4 months to suppress mosquito population

*Cost Savings from Project Wolbachia* <br>
The expected savings from a year-round deployment of Project Wolbachia is approx. SGD 770 Mil. 

**Conclusion** <br>
1. The model is able to perform well in terms of identifying the trend. Furthermore, its error rate is relatively low, with an RMSE score of 91. 
2. The model will serve well as an early detection tool, where the approximate measure can be implemented based on whether a minor or major spike is predicted. 
    * Minor Spikes: Use existing dengue measures
    * Major Spikes: Deploy Project Wolbachia
3. We would also recommend to deploy Project Wolbachia nationally throughout the year, to reduce the number of dengue cases and help meet NEA's KPI of reducing the weekly case load to under 100. Furthermore, based on our CBA, a cost savings of over $700 Million is achieved.

**Future Improvements** <br>
We would also recommend the following improvements for the future:
1. To increase our data collected
    * Town level dengue cases: By collecting the town level dengue cases, we will be able to be more targeted with the deployment of Project Wolbachia, which would significantly reduce its cost
    * Age group of populations in town: Older generations are more susceptible to severe disease. By having this data, towns with more susceptible populatiosn can be prioritized if resources are lean. 
    * More historical data: Having more historical data would be helpful with training a more accurate model
2. Engage domain experts
    * Domain experts wil be able to use their in-depth knowledge and expertise to assist with feature selection and feature engineering. 
