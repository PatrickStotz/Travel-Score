Travel Score
=============

**An interactive map that visualizes how much of the world you've already explored**  
A project by Patrick Stotz. Published in 03/2014 on [mappable.info](http://mappable.info)

Idea
--------------
The basic idea behind the map is quite simple. It divides the earth into graticular blocks with a width of 2x2 degrees. By selecting those cells that you've already visited the application calculates:

- how many of the earth's 197 countries you've visited
- the share of the world's population that lives in the selected areas
- the share of the earth's land surface that lies inside the selected cells

The overall travel score is the mean of these three numbers. 

Data Sources
--------------
To build this map the following geographic data sets have been used:

State boundaries by Natural Earth - 1:50m Cultural Vectors - 197 souvereign states, v. 2.0.0 (2012) - [link](http://www.naturalearthdata.com/downloads/50m-cultural-vectors/)

Place labels by Natural Earth -  1:110m Cultural Vectors - Populated places, v. 2.0.0 (2012) - [link](http://www.naturalearthdata.com/downloads/110m-cultural-vectors/)

Population data by CIESIN at Columbia University - Population Count Grid Future Estimates, v3 (2010) - [link](http://sedac.ciesin.columbia.edu/data/set/gpw-v3-population-count-future-estimates/data-download)

Land area data by CIESIN at Columbia University - Land and Geographic Unit Area Grids, v3 (1990, 1995, 2000, 2005, 2010, 2015) - [link](http://sedac.ciesin.columbia.edu/data/set/gpw-v3-land-geographic-unit-area/data-download)

Realization
--------------
I performed a number of geoprocessing steps in QGIS to generate a graticular vector grid with information on state boundaries, population and land area. The resulting data set is the main input for the interactive visualization which is written in D3/Javascript. 

For a more detailed description of the project take a look at our homepage: [mappable.info/projects/travel-score/](http://mappable.info/projects/travel-score/)

A full-sized, interactive view of Travel Score can be found [here](http://travelscore.org)

![alt text](/img/screenshot.jpg "Preview")
