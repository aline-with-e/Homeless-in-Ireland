# Homeless-in-Ireland
The data on Homelessness in Ireland was collected from gov.ie from 2016 to 2022. This is a projected created for the Real Time Data Analytics module from the Higher Diploma in Data Analytics  in DKIT.
On this project was performed descriptive analysis, analysis of Homeless in Ireland using a time series model and predictions for 2003, hypothesis testing using Kruskal test and prescreptive analysis by crossing the homeless figures with house prices data and unemplyment data.

Everything you need to know about the proje ct and the dataset:

**** This projected was created in R-Studio

Data Source: 
mydata: Homelessness data
Source: gov.ie 
Link: https://www.gov.ie/en/collection/80ea8-homelessness-data/

mydata2: Homelessness data
Source: gov.ie 
Link: https://www.gov.ie/en/collection/80ea8-homelessness-data/

mydata3: Residential Property Price Index
Source: cso.ie 
Link: https://data.cso.ie/table/HPM09

mydata4: Seasonally Adjusted Monthly Unemployment
Source: cso.ie 
Link: https://data.cso.ie/table/MUM01

*

Libraries Needed:                                                   

library(tidyverse)
library(lubridate)
library(scales)
library(dplyr)
library(ggplot2)
library(leaflet)
library(fpp2)                      

How to install those Libraries in R-Studio:  

install.packages("packagename")               *usually the package and library name are the same
library(libraryname)

* 
Data User Guide: 

mydata: Homelessness data
Male +	Female= Homeless adults
Ages 18-24 + Ages 25-44	+ Ages 45-64	+Ages 65 = Homeless adults
PEA +	STA	+TEA+	Other = Homeless adults
*
Definitions
PEA: Private Emergency Accommodation: this may include hotels, B&Bs and other residential 
facilities that are used on an emergency basis. Supports are provided to services users on a visiting 
supports basis. 

STA: Supported Temporary Accommodation: accommodation, including family hubs, hostels, with 
onsite professional support. 

TEA:  Temporary Emergency Accommodation: emergency accommodation with no (or minimal) 
support 

mydata3: Residential Property Price Index
% over 1,3,12 months: Percentage change in Property price over the previous month, previous 3 months, previous year
Base Jan 2005 = 100: Use as base the property price index from January in 2005

mydata4: Seasonally Adjusted Monthly Unemployment
Unemployment_thousand: Unemployment in thousand 
Unemployment_percentage_rate: Unemployment rate in percentage



