# Exploring the Migration and Population Distribution in Post-Katrina NOLA
*Sinduri Soundararajan | Professor Marynia Kolak | Geographic Information Sciences III | Spring 2021*

## Background
  Hurricane Katrina is remembered as one of the most destructive and influential storms in United States history. The city of New Orleans faced catastrophic damage and faced by residents before, during, and after the storm due to negligence towards infrastructure flaws, willful ignorance towards the disproportionate impacts of the storm on communities of color, and mismanaged efforts to rebuild and address property damage. The extreme flooding and physical destruction when several levees and other flood prevention features guarding the city exemplifies the man-made and natural forces that caused the magnitude of destruction during Katrina. For my final project, I chose to explore just one aspect of the many social impacts left by Katrina through a spatial analysis and visualization that displays the migration and population distribution patterns that occurred after the storm. Using the available datasets and wrangled data, I created  a map of New Orleans’ population changes by neighborhood/region of the city and an origin-destination dataset and model that grounds anecdotal/ethnographic research of displacement caused by the hurricane and potentially. Although Hurricane Katrina occurred 16 years ago, such data visualizations can be relevant by proving the potential for migration patterns to be triggered by environmental catastrophes and how the shifts in population impact a city’s makeup. Especially as extreme storm patterns continue during the ongoing climate crisis, such understandings of displacement and movement can be useful in preparing for future population shifts and potential environmental justice concerns.

## Goals and Objectives
•  The use of geocomputational operations to wrangle the American Community Survey (ACS) and the Puerto Rico Community Survey as a data set – this survey asks  ask respondents age whether they lived in the same residence 1 year ago and their location of their previous residence is collected if they have moved. Using this as an access point, flows of former-New Orleans-residents can be collected in order to gather origin-destination data (where origin is New Orleans and destination is states throughout the U.S.). 

• The use of geocomputational operations to wrangle data from The Data Center of Southern Louisiana and US Census Bureau to measure the change in total population preceding the storm and shortly thereafter, as well as changes in total population of each ward or planning district of the city.  

• Application of wrangled data in order to create visualizations of displacement and migration due to Hurricane Katrina, using PostGreSQL through Carto and/or Keplr.Gl softwares

## Data Sources, Spatial and Temporal Scale
• The United States Census Bureau provides [State-to-State migration flow](https://www.census.gov/data/tables/time-series/demo/geographic-mobility/state-to-state-migration.html) data that could be used in order to visualize the displacement of populations living in New Orleans and other areas affected by the storm and map out where communities fled to in the months/years following Katrina. 
    Temporal scale of dataset used: 2005-2007 migration flows

• The [Data Center of Southern Louisiana](https://www.datacenterresearch.org/data-resources/who-lives-in-new-orleans-now/) has compiled US Census data and available state resources that is relevant to the effects of Hurricane Katrina. In particular, they source information regarding the US Census-collected population prior to and after the Storm. This can be used to show the change in total population preceding the storm and shortly thereafter.
    Temporal scale of dataset used: 2000 and 2019 population distributions 

• [Planning district geometry](https://portal-nolagis.opendata.arcgis.com/datasets/planning-districts?geometry=-90.354%2C29.907%2C-89.401%2C30.115) sourced from City of New Orleans' open data portal. Data was downloaded as shp file and transformed into GeoJSON (usable through keplr.gl software) during spatial joins of data with population data from The Data Center. 

## Methods 
![NOLA Planning Districts – Population Distribution](https://github.com/sindu-ri/gisiiifinal/blob/main/Methods%20(1).png)
![Post-Katrina Louisiana Migration Patterns](https://github.com/sindu-ri/gisiiifinal/blob/main/Methods%20(2).png)

## Results 
Navigate to respository files to access the resulting datasets and visualizations from this process. 

[NOLA Planning Districts – Population Distribution Visualization ](https://kepler.gl/demo/map/carto?mapId=08482dea-b13e-3083-7845-08bc75a575af&owner=sindu-ri&privateMap=false)

[Post-Katrina Louisiana Migration Patterns Visualization](https://kepler.gl/demo/map/carto?mapId=3e60b03d-27e3-b56a-6eff-822e53e7e347&owner=sindu-ri&privateMap=false)

### Discussion of Results
*Population Redistribution*

Following Katrina, New Orleans faced population changes that can be at least partially attributed to death, destruction, and migration out of NOLA during and after the storm. The visualization created displays percent population changes throughout planning districts in New Orleans. As shown through the map, Planning Districts 8 and 11 faced the most extreme changes in population loss before and after the storm – both districts are home to many of the city’s majority-minority neighborhoods who face a legacy of disinvestment, marginalization, and disenfranchisement due to historical and ongoing discrimination and (as proven by Katrina response and relief) consistent neglect. 

*Migration out of NOLA*

Many surviving residents of New Orleans migrated out of Louisiana following the storm. The created data visualization shows the flow of residents out of New Orleans, through arches from the origin of Louisiana moving outwards to others states in the United States. Katrina is often described to be the biggest climate-driven migration since the Dust Bowl of the 1930s, with over a million people fleeing from the state after the storm. This maps grounds arguments of environmental migration and the impact of climate and weather patterns on displacement by displaying the large-scale migration out of Louisiana in the months/years following Katrina.  Based on the created visual, most migrating survivors moved to states neighboring Louisiana, with a large flow of residents into Texas, Florida, Arkansas, etc. 

 
## Limitations and Future Work 
Narratives and legal categorizations of environmental refugees and climate-driven migrations are often limited by the difficulty of assigning causality to movement and migration flow. While the focus of my project was on migration following Hurricane Katrina, it is challenging to make large-scale causal inferences and claims for migration data, and to connect populatupulation movement to Katrina when so many other confounding variables may impact individuals' decisions to move. The results of this project are further limited by the temporal scale of the datasets used; Because Katrina occured in between census collection years and The Data Centure only carries data from 2000 and 2019, only broad claims regarding the correlation between population loss in certain planning distructs can be made. 

Despite these limitations, this project allowed me to practice skills in data wrangling and visualization creation that I hope to use for future personal work in studying climate-driven migration patterns. From this process, I learned the challenges associated with assigning causality (particular related to environmental causes) to migration patterns and population distribution changes. Future work should involve data analysis of population and migration in years prior to and after the storm and allow for a comparison between a "controlled" year (with no storm influencing movement/population patterns) and a year with trends influenced by the storm. This project also provides an opportunity for a mixed-methods approach to data analysis; the combination of spatial data and alsysis and qualitative material from ethnographies, anecdotes from survivors, etc. can allow for a more complete understanding of the impacts of Hurricane Katrina on migration patterns.
