# Project_1_Hurricanes
Members: Kelsea Thayer, Lakia White, Cory Parker
Goal:
Our project was to identify long-term trends and patterns in hurricane severity. By examining data, we can determine if there are any significant changes in storm intensity over the years.
Questions:
We asked:
1)   What is the overall trend in the number of hurricanes over time?
2)   Is there a correlation between the number of hurricanes vs high desert temperatures combined with lower ocean temperatures?
3)   Do higher desert temperatures produce more named storms, hurricanes, and major hurricanes?
4) How does wind and evapotranspiration contribute to storm creation and what correlations will we see?   
Hypothesis:
Our hypothesis is that we would see strong correlations between temperature and number of storms as well as wind and number of storms. We also thought some of the storms may be in cycles due to what is publicized about climate change.
Process:
   Collected Data
OpenWeather API - One Call API 3.0
Used to collect 72 years of data including desert temperatures, ocean temperatures, wind speed and direction, and evapotranspiration 
https://api.openweathermap.org/data/3.0/onecall?lat={lat}&lon={lon}&exclude={part}&appid={API key}
	
Kaggle Data Set (Hurricanes Recorded by Year by BRYAN SOUZA)
Used to gather over 100 years of data including the year, named storms, total hurricanes, and major hurricanes. Original Data is from The Deadliest, Costliest, and Most Intense United States Hurricanes 1900-2000
   Cleaned and Merged
We used the api key to pull 72 years, which is as far back as they go, to pull the weather data for a coordinate in the ocean off the coast as well as a coordinate in the desert. This included max and min temperature every day for those years. We took an average of each september and deleted the rest of the data. We chose September because that is when most hurricanes occur. The three were merged together into a single data frame. 
  Data
  
              Year  Named Storms  Hurricanes  MajorHurricanes  \
count    73.000000     73.000000   73.000000        73.000000   
mean   1981.000000     11.205479    6.205479         2.712329   
std      21.217131      4.143130    2.640280         1.889146   
min    1945.000000      4.000000    2.000000         0.000000   
25%    1963.000000      8.000000    4.000000         1.000000   
50%    1981.000000     11.000000    6.000000         2.000000   
75%    1999.000000     13.000000    8.000000         4.000000   
max    2017.000000     28.000000   15.000000         8.000000   
Used various charts to find any correlation between our metrics. 
  Analysis and Conclusion:
The number of storms and hurricanes have shown an increasing trend over the last 72 years. 
Higher desert temperatures in September increase the likelihood of observed storms, hurricanes, and major hurricanes for that year. The data showed a positive correlation of 0.31 for desert temperatures and negative correlation of -0.10 ocean temperatures. 
The ocean evapotranspiration rate for each September had little correlation with an r-value of 0.27 for the observed storms. 

