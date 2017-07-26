# Crime Analytics: Visualization of Incident Reports
## Overview

In this notebook, I analyze criminal incident data from Seattle or San Francisco to visualize patterns and contrast and compare patterns across the two cities.

I produce a blog-post-style visual narrative consisting of a series of visualizations interspersed with sufficient descriptive text to make a convincing argument.

## Project Ideas

- For either city, how do incidents vary by time of day? Which incidents are most common in the evening? During what periods of the day are robberies most common?
- For either city, how do incidents vary by neighborhood? Which incidents are most common in the city center? In what areas or neighborhoods are robberies or thefts most common?
- For either city, how do incidents vary month to month in the Summer 2014 dataset?
- For either city, which incident types tend to correlate with each other on a day-by-day basis?
- **Advanced**  What can we infer broadly about the differences in crime patterns between Seattle and San Francisco? Does one city tend to have more crime than the other, per capita? Do the relative frequencies of types of incidents change materially between the two cities? (NOTE: The two datasets do not have the same schema, so comparisons will require some work and some assumptions.)
- **Advanced**  For either city, do certain crimes correlate with environmental factors such as temperature? (To answer this kind of question, I use external data sources )

## Data

This project uses the real crime data from Summer 2014 one or both of two US cities: Seattle and/or San Francisco.

**Seattle Data**

[**Seattle Summer 2014 dataset used for code development**](https://github.com/uwescience/datasci_course_materials/blob/master/assignment6/seattle_incidents_summer_2014.csv)

_Other Seattle data:_

[_Seattle Data Portal_](https://data.seattle.gov/)

[_Full Seattle incident dataset_](https://data.seattle.gov/Public-Safety/Seattle-Police-Department-Police-Report-Incident/7ais-f98f)

**San Francisco Data**

[**San Francisco Summer 2014 dataset used for code development**](https://github.com/uwescience/datasci_course_materials/blob/master/assignment6/sanfrancisco_incidents_summer_2014.csv)

_Other San Francisco Data:_

[_San Francisco Data Portal_](https://data.sfgov.org/)

[_Full San Francisco incident dataset_](https://data.sfgov.org/Public-Safety/SFPD-Incidents-from-1-January-2003/tmnf-yvry)

All datasets are provided through their respective cities data portals, all powered by  [Socrata](https://www.socrata.com/). The three portals and the links to the original datasets are

**Integration**  
Inter-city comparisons of crime data 
* These datasets do NOT agree on schema, and they do NOT agree on categories or descriptions for specific crimes. 
* To draw comparisons and contrasts across cities, I need to make some assumptions about correspondences. For example, LARCENY/THEFT is a category in San Francisco, but Seattle uses codes of the form THEFT-CARPROWL or THEFT-BUILDING.
* Need to make some reasonable assumptions to compare these data, and explain and justify these assumptions.

**Scale**  
* The full Chicago dataset covering 2001 to present has 5M records and is about 1.3GB as a csv file
* Develop and test with subsets of all three datasets during the period Summer 2014 
* Expand analysis to the full datasets

### Tools
Python with  [Bokeh](http://bokeh.pydata.org/en/latest/) or  [matplotlib](http://matplotlib.org/), R with ggplot2
