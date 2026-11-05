Report and analysis of the case: Climate watch <br> Author: Sander van Dam <br> Date: 05/11/2026 <br>\
The goal of the case was to analyze trends in global temperature changes over time and to visualise this data using tools like python, JupyterNotebook, SQL and MS Power BI. The case was analyzed by importing the provided csv files into an SQL Database using MySQL. Empty values were transformed into NULL (or NaN in python) to prevent unforeseen skewing in the dataset if data were to be transformed into 0. Additionally, a subset of the data was created using all entries from 1980 onward.
For the global temperature on land and sea a table was made to inspect the global statistics of temperature with the following results:

![Global temperature Descriptives](https://github.com/SanderVD1999/case-climate-watch-sander/blob/main/assets/Screenshot%202026-11-05%20151427.png)

This table describes the basic information of the dataset but cannot show many meaningful results. What can be observed in the table is the average global temperature throughout the entire database (from 1743 until 2015) and the standard deviation of this temperature. 
The next step was to analyze global temperature averages by year, first by descriptions in a table, then visualised as a line graph:

![Line Graph globaltemperatures](https://github.com/SanderVD1999/case-climate-watch-sander/blob/main/assets/linegraph.png)

The above line graph inspects global land temperature trends throughout the years. The first point that stands out is a decreasing variety throughout the years. At the start of the graph at 1750 the lines are consistently far apart from each other, this would signify that global temperature was rapidly changing up and down around this time, sometimes even changing 2-2.5 degrees in only a couple of years. In later years the variety in temperature throughout the years reduces significantly. though this seems like a strange observation, temperature records before 1850 was analysed by so called "proxy-data". proxy data is measured by things as coral growth, ice cores, icotope variations and tree rings. temperature records before 1850 also had less coverage and consisted largely of measures in the northern hemisphere and were also read manually. Since 1850 the world developed more reliable ways to measure global temperature with globally distributed electronic sensors, mercury or alcohol thermometers. This change in methodology improved validity and reliability of global temperature measurements.  

To clarify the variety between pre 1850 and post 1850 trends the following comparison graph has been developed:

![Pre and post 1850 comparisons](https://github.com/SanderVD1999/case-climate-watch-sander/blob/main/assets/1850comparison.png)
