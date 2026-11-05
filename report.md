Report and analysis of the case: Climate watch
Author: Sander van Dam, Date: 05/11/2026
The goal of the case was to analyze trends in global temperature changes over time and to visualise this data using tools like python, JupyterNotebook, SQL and MS Power BI. The case was analyzed by importing the provided csv files into an SQL Database using MySQL. Empty values were transformed into NULL (or NaN in python) to prevent unforeseen skewing in the dataset if data were to be transformed into 0. Additionally, a subset of the data was created using all entries from 1980 onward.
For the global temperature on land and sea a table was made to inspect the global statistics of temperature with the following results:
Land_avg_temp	Land_avg_temp_uncertainty	Land_max_temp	Land_max_temp_unc	Land_min_temp	Land_min_temp_unc	Land_and_oceanavgtemp	Land_and_oceanavgtemp_unc
count	3192.000000	3192.000000	3192.000000	3192.000000	3192.000000	3192.00000	3192.000000	3192.000000
mean	8.343247	0.934940	8.955638	0.299413	1.712169	0.26950	9.493556	0.080212
std	4.403004	1.095883	7.740712	0.515985	3.541556	0.40962	7.437984	0.085181
min	-2.080000	0.000000	0.000000	0.000000	-5.407000	0.00000	0.000000	0.000000
25%	4.261750	0.185000	0.000000	0.000000	0.000000	0.00000	0.000000	0.000000
50%	8.584500	0.389000	9.354000	0.123000	0.000000	0.13500	13.859000	0.060000
75%	12.538750	1.413250	16.749000	0.306250	4.669000	0.32700	15.819500	0.131000
max	19.021000	7.880000	21.320000	4.373000	9.715000	3.49800	17.611000	0.457000

The next step was to analyze global temperature averages by year, first by descriptions in a table, then visualised as a line graph:
![image](Downloads/linegraph.png)
