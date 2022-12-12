# Introduction

```{figure} https://upload.wikimedia.org/wikipedia/commons/5/57/Concord_Pacific_Master_Plan_Area.jpg
---
height: 300px
name: vancouver_skyline
---
Vancouver skyline with street trees pictured in foreground.
```
Vancouver is a city located on the west coast of Canada, perched between the North Shore Mountains and the Pacific Ocean. Known for its spectacular natural environment, it has been consistently ranked one of the most livable cities in the world throughout the last decade.

Climate modeling conducted by the Pacific Climate Impacts Consortium in 2016 predicts that the average temperature in the Vancouver region will increase by 3°C by the 2050s and a dramatic increase in days in which the temperature exceeds 25°C will be seen, from an average of 22 days per year to 55 (Climate Projections for Metro Vancouver, 2016). Between June 25th and July 1st of 2021, temperatures rose above 40°C throughout the Province of British Columbia, resulting in 99 deaths in the City of Vancouver (CBC News).

In 2014, the City of Vancouver adopted the Urban Forest Plan as part of its goal to become the greenest city in the world by 2020. The goal of the Urban Forest Plan is to "protect, plant, and manage trees to create a diverse, resilient, and beautiful urban forest on public and private lands across the city." (Urban Forest Plan, 2018). 

The urban forest plays one of many key roles in the City of Vancouver's climate adaptation strategy. Trees in the urban environment mitigate the urban heat island effect which is an increase in temperature in urban areas due to lower tree canopy cover and a high density of heat-absorbing structures such as roads and buildings (Urban Forest Plan, 2018). Approximately 30% of the Vancouver tree population consisted of street trees at the time of the adoption of the Urban Forest Plan in 2014 (Urban Forest Plan, 2018). As such, street trees are central to the urban forest and play an important role in its effort to aid in climate change adaptation.

Understanding the composition of the Vancouver street tree population is vital to its stewardship. We will examine the street tree population through importance value, which is a calculation that takes into account both abundance and size (in the form of dominance) when determining a group's contribution to the overall population, as used by McPherson and Rowntree (1989) in their characterization of various street tree populations at the species level. We will apply the following formulas at the genus level to the Vancouver street tree population:

```{math}
:label: relative_abundance_analysis
relative\ abundance\ =\ \frac{number\ of\ individuals\ of\ genus\ X}{total\ individuals\ in\ population}\cdot100\\
```
```{math}
:label: basal_area_analysis
basal\ area\ =\pi\cdot(\frac{diameter}{2})^2\\
```
```{math}
:label: relative_dominance_analysis
relative\ dominance\ =\ \frac{total\ basal\ area\ of\ genus\ X}{total\ basal\ area\ of\ population}\cdot100\\
```
```{math}
:label:  importance_value_analysis
importance\ value\ =\ relative\ abundance + relative\ dominance
```
```{math}
:label: relative_importance_analysis
relative\ importance\ =\ \frac{total\ importance\ value\ of\ genus\ X}{total\ importance\ value\ of\ population}\cdot100\\
```

<b>Using these calculations, we hope to answer the following questions:</b>
* <i>How do the various genera in the Vancouver street tree population compare to one another in terms of importance to the total population?
* How do the different size classes of the top 3 genera contribute to each genus' importance in the population, and is there a difference in this distribution between these genera?
* How do Vancouver neighbourhoods compare in terms of importance value density of the street tree population?
* How is the importance value of the various street tree genera distributed throughout Vancouver?</i>

We will be using a subset of the Vancouver street trees dataset available through the [City of Vancouver's Open Data Portal](https://opendata.vancouver.ca/explore/dataset/street-trees/information/?disjunctive.species_name&disjunctive.common_name&disjunctive.height_range_id). The subsetted data can be found in the UBC Exploratory Data Visualization [GitHub Data Repository](https://raw.githubusercontent.com/UBC-MDS/exploratory-data-viz/main/data/vancouver_trees.csv).
Land area for each neighbourhood was obtained from the [City of Vancouver Website](http://vancouver.ca/news-calendar/areas-of-the-city.aspx) and uploaded to a [GitHub Data Repository](https://raw.githubusercontent.com/Daniel-J-Stevens/data-science-toolbox_assignment-8/main/van-trees_book/data/neighbourhood_demographics.csv)