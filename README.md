# Exploring the Migration and Population Distribution in Post-Katrina NOLA
*Sinduri Soundararajan | Professor Marynia Kolak | Geographic Information Sciences III | Spring 2021*

## Background
  Hurricane Katrina is remembered as one of the most destructive and influential storms in United States history. The city of New Orleans faced catastrophic damage and faced by residents before, during, and after the storm due to negligence towards infrastructure flaws, willful ignorance towards the disproportionate impacts of the storm on communities of color, and mismanaged efforts to rebuild and address property damage. The extreme flooding and physical destruction when several levees and other flood prevention features guarding the city exemplifies the man-made and natural forces that caused the magnitude of destruction during Katrina. For my final project, I chose to explore just one aspect of the many social impacts left by Katrina through a spatial analysis and visualization that displays the migration and population distribution patterns that occurred after the storm. Using the available datasets and wrangled data, I created  a map of New Orleans’ population changes by neighborhood/region of the city and an origin-destination dataset and model that grounds anecdotal/ethnographic research of displacement caused by the hurricane and potentially. Although Hurricane Katrina occurred 16 years ago, such data visualizations can be relevant by proving the potential for migration patterns to be triggered by environmental catastrophes and how the shifts in population impact a city’s makeup. Especially as extreme storm patterns continue during the ongoing climate crisis, such understandings of displacement and movement can be useful in preparing for future population shifts and potential environmental justice concerns.

## Goals and Objectives
•  The use of geocomputational operations to wrangle the American Community Survey (ACS) and the Puerto Rico Community Survey as a data set – this survey asks  ask respondents age whether they lived in the same residence 1 year ago and their location of their previous residence is collected if they have moved. Using this as an access points, flows of former-New Orleans-residents can be collected in order to gather origin-destination data (where origin is New Olreans) from 2006. 
• The use of geocomputational operations to wrangle data from The Data Center of Southern Louisiana and US Census Bureau to measure the change in total population preceding the storm and shortly thereafter, as well as changes in total population of each ward or planning district of the city.  
• Application of wrangled data in order to create visualizations of displacement and migration due to Hurricane Katrina, using PostGreSQL through Carto and/or Keplr.Gl softwares

## Data Sources, Spatial and Temporal Scale
• The United States Census Bureau provides [State-to-State migration flow](https://www.census.gov/data/tables/time-series/demo/geographic-mobility/state-to-state-migration.html) data that could be used in order to visualize the displacement of populations living in New Orleans and other areas affected by the storm and map out where communities fled to in the months/years following Katrina. 
    Temporal scale of dataset used: 2005-2007 migration flows
• The [Data Center of Southern Louisiana](https://www.datacenterresearch.org/data-resources/who-lives-in-new-orleans-now/) has compiled US Census data and available state resources that is relevant to the effects of Hurricane Katrina. In particular, they source information regarding the US Census-collected population prior to and after the Storm. This can be used to show the change in total population preceding the storm and shortly thereafter.
    Temporal scale of dataset used: 2000 and 2019 population distributions 
• [Planning district geometry](https://portal-nolagis.opendata.arcgis.com/datasets/planning-districts?geometry=-90.354%2C29.907%2C-89.401%2C30.115) sourced from City of New Orleans' open data portal. Data was downloaded as shp file and transformed into GeoJSON (usable through keplr.gl software) during spatial joins of data with population data from The Data Center. 

## Methods 
![NOLA Planning Districts – Population Distribution](https://github.com/sindu-ri/gis3final/blob/main/GISIIIFinal%20Methods%201.png)
![Post-Katrina Louisiana Migration Patterns](https://github.com/sindu-ri/gis3final/blob/main/GISIIIFinal%20Methods%202.png)

 
## Limitations 
Timespan of census data on population – I used a dataset of 2019 and 2000 population
Difficult to make causal inferences and claims for migration data, and to connect population movement to Katrina when so many other confounding variables may impact decisions to move  
