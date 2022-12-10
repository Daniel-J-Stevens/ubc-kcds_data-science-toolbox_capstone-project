# Discussion

In order to create clean visualizations, it is important that we filter the dataset to eliminate data points that, although they may not drastically change the overall conclusions drawn, may be distracting or confuse the audience. We will filter out the diameter outliers that we determined to be invalid, as well as the neighbourhood outliers.

How do the various genera in the Vancouver street tree population rank in relation to one another in terms of importance in the total population?

We will include a bar chart, showing the relative importance value by genus (Fig. 4)
We will include a scatter plot of relative dominance vs relative abundance, encoding relative importance value to size (Fig. 3, relative dominance vs relative abundance facet)
We will add a reference line to the scatter plot which will represent the mean basal area of the population.
We will include only the top 10 genera in this visualization
How do the different size classes of the top 3 genera contribute to each genus' importance in the population, and is there a difference in this distribution between the genera?

We will include a bar chart, binning tree diameters in 5cm size classes, faceting by genus, showing how each size class contributes to each genus' total importance. Each chart will be normalized to the genus' total importance to allow for easy comparison between genera (Fig. 5)
We will include a second plot, showing the cumulative importance value of each genera over its size classes.
We will simplify the visualization by restrictiong to the top 3 genera in terms of importance value, as these are the most prevalent genera in the street tree population.
How do Vancouver neighbourhoods compare in terms of importance value density of the street tree population?

We will include a chloropleth map with importance value density encoded to the color channel. (Fig. 6)
We will add a text overlay to the chlorpleth map of the importance value density values to allow for greater distinction between neighbourhoods (Fig. 7)
We will add a text chart to the right of the chloropleth map, listing neighbourhoods in the order of importance value density rank. These will be linked with the neighbourhood map, and each will be highlighted upon hovering to allow for easy identificaiton of neighbourhood and area.
How is the relative importance of each genera distributed throughout Vancouver? (DASHBOARD)

We will include a heat map of genus vs. neighbourhood, with relative importance encoded to the color channel (Fig. 8)
We will use the heat map as a multi-selection tool, allowing the visualization of the tree distribution of the selected genus in the selected neighbourhood (Fig. 9)
We will include an overview map to indicate the position of the selected neighbourhood within the city of Vancouver.
Will provide a dropdown to allow the user to subset the heatmap to a single genus.
We will include a slider that will allow the user to subset the heatmap by ascending genus ranking.
For the final analysis report, we will use the Altair server, and process data within the Altair module.