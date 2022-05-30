# Surfs_up
An analysis is performed on the weather dataset of Oahu,Hawaii island,to open a surf and shake shop serving surfboards and icecreams to locals,tourists using advanced data storage.

## Overview of the Analysis
In this analysis,we have used SQLite,a version of sql which lives on the computer or phone so its smaller,faster and doesnt have users.It is widely used database engine.It is very popular because it can be stored locally instead of a database server.Local databases support quick testing and easy prototyping.In order to achieve the benefits of SQLite,we use SQLAlchemy,which is a query tool designed for SQLite and the integration of statistical analysis with data frame analysis.Finally to share our analysis we use Flask,a webframework that uses Python to build webpages.

## Purpose of the Analysis
W. Avy,the investor wants us to collect more information about temperature trends before opening the surf shop. Specifically, he wants temperature data for the months of June and December in Oahu, in order to determine if the surf and ice cream shop business is sustainable year-round.

## Resources Used
*DataSources*: [hawaii.sqlite](https://github.com/fathi129/Surfs_up/blob/master/hawaii.sqlite)<br>
*Software used*: Jupyter notebook,Flask,SQLite,<br> 
*Libraries used*: Pandas,SQlAlchemy <br>
*Language*: Python <br>

## Deliverable 1: Determine the Summary Statistics for June 
Using Python, Pandas functions and methods, and SQLAlchemy, I have filtered the date column of the Measurements table in the hawaii.sqlite database to retrieve all the temperatures for the month of June. Then converted those temperatures to a list, created a DataFrame from the list, and generated the summary statistics,the summary statistics image is below.<br>
<img src = "https://github.com/fathi129/Surfs_up/blob/master/Screenshots/June_temps.png" width = 200><br>

## Deliverable 2: Determine the Summary Statistics for December 
Using Python, Pandas functions and methods, and SQLAlchemy, I have filtered the date column of the Measurements table in the hawaii.sqlite database to retrieve all the temperatures for the month of December. Then converted those temperatures to a list, created a DataFrame from the list, and generated the summary statistics,the summary statistics image is below.<br>
<img src = "https://github.com/fathi129/Surfs_up/blob/master/Screenshots/Dec_temps.png" width = 200><br>

## Results
- The average recorded temperature in June is about 75 degrees F, 4 degrees higher than the average temp in December which is 71 degrees F.
- The frequency of temperatures recorded in June tends to have a normal distribution,The temperature ranges from maximum of 85 degrees F and minimum of 64 degrees F.
- The December temperatures seem to be more variable than those in June,comparing the max temp as 83 degrees F and were as min temp is 56 degrees F.
- when looking at the plotted distribution of temperatures in June,December,we can see that the median temperature is more inline with the average, and   there are not many outliers in both the months.
- In addition, both June and December had roughly similar standard deviations. June's standard deviation of 3.26 and December's standard deviation of 3.75 tells that their temperature records are concentrated around both of their average temperatures. 
- Lastly, June and December had a 75th percentile of 77°F and 74°F, respectively, which indicates that these two seasons had relatively warm temperatures.

|    ***June Temperature Histogram***       |    ***December Temperature Histogram*** |
|  ---------------------------------------      |    --------------------------------------|
|  <img src = "https://github.com/fathi129/Surfs_up/blob/master/Screenshots/june_temp_query.png" width = 350><br >              |  <img src = "https://github.com/fathi129/Surfs_up/blob/master/Screenshots/dec_temp_query.png" width = 350><br> |

## Summary

- Overall the weather in December and June are very similar, although December has a wider range of results, with its high being close to June but its low well below June.June and December will be approriate months to open surfing and ice cream shops as the average temperature difference between both the months is 4 degree F.
**Additional queries that could be run include**: 
- Precipation difference between June and December to determine which one has more rainy weather, By seeing the  precipitation results we could see the average rainfall is 14% in June.

|    ***June Precipitation Histogram***          |    ***December Precipitation Histogram***   |
|  --------------------------------------------  |    -----------------------------------------| 
|  <img src = "https://github.com/fathi129/Surfs_up/blob/master/Screenshots/june_prcp_query.png" width = 350><br >               |  <img src = "https://github.com/fathi129/Surfs_up/blob/master/Screenshots/Dec_prcp_query.png" width = 350><br> |
|  <img src = "https://github.com/fathi129/Surfs_up/blob/master/Precipitation%20images/june_prcp-describe.png" width = 200><br >               |  <img src = "https://github.com/fathi129/Surfs_up/blob/master/Precipitation%20images/Dec_prcp_describe.png" width = 200><br> |



When performing this analysis,we have calculated the precipitation for the whole year,and we could see the average rainfall through out the year was 17%.
The distribution of temperature for the whole year for particular station was also calculated and we can see that it ranges between 60 to 80 degree F.<br>

<img src = "https://github.com/fathi129/Surfs_up/blob/master/Precipitation%20images/rainfall.png" width = 350> <br>
<img src = "https://github.com/fathi129/Surfs_up/blob/master/Precipitation%20images/prcp_year_describe.png" width = 200> <br> 
<img src = "https://github.com/fathi129/Surfs_up/blob/master/Precipitation%20images/temp_year_Around.png" width = 350><br>


- As well as a comparison by weather station, as we may see higher,lower temperatures and precipitation levels at different locations. We would be primarily interested in the weather station closest to our location, which would narrow the results and provide the best data for us to consider.
- We could also check the wind in the stations,in the months of June and December so that it would be useful for deciding about the surf shop.











