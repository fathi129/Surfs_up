# Surfs_up
An analysis is performed on the weather dataset of Oahu, Hawaii island, to open a surf and shake shop, serving surfboards and icecreams to locals and tourists using advanced data storage.

## Overview of the Analysis
In this analysis, we have used SQLite, a version of SQL which lives on the computer or phone, so it's smaller, faster, and doesn't have users. It is a widely used database engine. It is prevalent because it can be stored locally instead of on a database server. Local databases support quick testing and easy prototyping. To achieve the benefits of SQLite, we use SQLAlchemy, which is a query tool designed for SQLite and the integration of statistical analysis with data frame analysis. Finally, we use Flask, a Python web framework, to build web pages to share our analysis.

## Purpose of the Analysis
W. Avy, the investor, wants us to collect more information about temperature trends before opening the surf shop. Specifically, he wants temperature data for June and December in Oahu to determine if the surf and ice cream shop business is sustainable year-round.

## Resources Used
*DataSources*: [hawaii.sqlite](https://github.com/fathi129/Surfs_up/blob/master/hawaii.sqlite)<br>
*Software used*: Jupyter notebook, Flask, SQLite,<br> 
*Libraries used*: Pandas, SQlAlchemy <br>
*Language*: Python <br>

## Deliverable 1: Determine the Summary Statistics for June 
Using Python, Pandas functions and methods, and SQLAlchemy, I have filtered the date column of the Measurements table in the hawaii.sqlite database to retrieve all the temperatures for June. Then converted those temperatures to a list, created a DataFrame from the list, and generated the summary statistics; the summary statistics image is below.<br>
<img src = "https://github.com/fathi129/Surfs_up/blob/master/Screenshots/June_temps.png" width = 200><br>

## Deliverable 2: Determine the Summary Statistics for December 
Using Python, Pandas functions and methods, and SQLAlchemy, I have filtered the date column of the Measurements table in the hawaii.sqlite database to retrieve all the temperatures for December. Then converted those temperatures to a list, created a DataFrame from the list, and generated the summary statistics; the summary statistics image is below.<br>
<img src = "https://github.com/fathi129/Surfs_up/blob/master/Screenshots/Dec_temps.png" width = 200><br>

## Results
- The average recorded temperature in June is about 75 degrees F, 4 degrees higher than the average temperature in December, 71 degrees F.
- The frequency of temperatures recorded in June tends to have a normal distribution; The temperature ranges from 85 degrees F to a minimum of 64 degrees F.
- The December temperatures seem to be more variable than those in June, comparing the maximum temperature to 83 degrees F, whereas the minimum temperature is 56 degrees F.
- When looking at the plotted distribution of temperatures in June and December, we can see that the median temperature is more in line with the average, there are not many outliers in both the months.
- In addition, both June and December had roughly similar standard deviations. June's standard deviation of 3.26 and December's standard deviation of 3.75 tells that their temperature records are concentrated around both of their average temperatures.
- Lastly, June and December had a 75th percentile of 77°F and 74°F, respectively, which indicates that these two seasons had relatively warm temperatures.

|    ***June Temperature Histogram***       |    ***December Temperature Histogram*** |
|  ---------------------------------------      |    --------------------------------------|
|  <img src = "https://github.com/fathi129/Surfs_up/blob/master/Screenshots/june_temp_query.png" width = 350><br >              |  <img src = "https://github.com/fathi129/Surfs_up/blob/master/Screenshots/dec_temp_query.png" width = 350><br> |

## Summary

- Overall, the weather in December and June are very similar, although December has a broader range of results, with its high being close to June but low well below June. June and December will be appropriate months to open surfing and ice cream shops as the average temperature difference between both the months are 4 degrees F. 
**Additional queries that could be run include**: 
- We could calculate the Precipitation difference between June and December to determine which one has more rainy weather. We could see the average rainfall is 14% in June and in December it was 22% by seeing the precipitation results.<br>

|    ***June Precipitation Histogram***          |    ***December Precipitation Histogram***   |
|  --------------------------------------------  |    -----------------------------------------| 
|  <img src = "https://github.com/fathi129/Surfs_up/blob/master/Screenshots/june_prcp_query.png" width = 350><br >               |  <img src = "https://github.com/fathi129/Surfs_up/blob/master/Screenshots/Dec_prcp_query.png" width = 350><br> |
|  <img src = "https://github.com/fathi129/Surfs_up/blob/master/Precipitation%20images/june_prcp-describe.png" width = 200><br >               |  <img src = "https://github.com/fathi129/Surfs_up/blob/master/Precipitation%20images/Dec_prcp_describe.png" width = 200><br> |

When performing this analysis, we calculated the precipitation for the whole year, and we could see the average rainfall throughout the year was 17%. The distribution of temperature for the whole year for particular station was also calculated, and we can see that it ranges between 60 to 80 degrees F.<br>

<img src = "https://github.com/fathi129/Surfs_up/blob/master/Precipitation%20images/rainfall.png" width = 350> <br>
<img src = "https://github.com/fathi129/Surfs_up/blob/master/Precipitation%20images/prcp_year_describe.png" width = 200> <br> 
<img src = "https://github.com/fathi129/Surfs_up/blob/master/Precipitation%20images/temp_year_Around.png" width = 350><br>


- As well as a comparison by the weather station, we may see higher, lower temperatures and precipitation levels at different locations. We would be primarily interested in the weather station closest to our location, narrowing the results and providing the best data for us to consider.
- We could also calculate the wind condition near the location in June and December to help decide about the surfing.











