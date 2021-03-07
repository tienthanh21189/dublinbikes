# dublinbikes
DublinBikes Analytics
Tien Thanh Nguyen
L00162305
MSc in Computing in Big Data Analytics

I. Description:
DublinBikes is a public bicycle rental scheme that has operated in Dublin city since 2009. It has played a key role in the development of Dublin’s intelligent transport system. There are some reports on the state of the system, but the majority of the data sets used for analysis are before 2018. Therefore, this study will analyze the current state of the system through the latest data sets from quarter 3 2018 to quater 4 2020. Furthermore, the study focuses on analyzing operational efficiency as well as predicting the development trend in the future.


II. Dataset:
The data sets will be get from https://data.gov.ie/dataset/dublinbikes-api. The data sets save the historic operation of 110 bike stations in Dublin with a 5-minute interval from Q3 2018 to Q3 2020. It means that every 5 minutes, a new row will be recorded in the database to demonstrate the state of a bike station at this time including some fields such as station id, time, bikes available, bike stands available, etc. These records were extracted from the database to 10.csv files relevant to 10 quarters from Q3 2018 to Q4 2020. The total volume of these 9 .csv files is 2.99 GB and the total rows are approximately 26.7 million.

III. Goals:
Analysing the level of traffic on an hourly/daily basis to answer the below questions:
1. What are the usage patterns?
• Compare the traffic between weekdays.
• Compare the traffic between the hours of the day. • Clustering the bike stations based on their traffic. • Upward trends or downward trends.

2. How effective is the system to use?
• The percentage of usage bikes at a certain time.
• Any bike station is overloaded at a certain time due to the lack of available bikes?

3. How can the Department of Transport use this data to improve the system?
• Based on the operational efficiency above, we could propose some solutions such as redistributing the number of bikes at each bike station, buying more bikes or expanding bike stations, etc.

IV. Solution and Methodology
1. Data preparation
• Use Talend Open Studio to combine and clean data.
• Use DataFrame in Python to calculate the level of traffic.
2. Data analytics
• Use Machine Learning techniques such as Linear Regression, K-Means Clus- tering, Support Vector Machines, etc. to analyse the data sets. (by using Matplotlib on Python for Machine Learning)
3. Data visualisation
• Use Seaborn & Matplotlib to visualise data sets.

V. Results/Conclusions:
1. The correlation between bikes IN/OUT a day (using Linear Regression):
The Bikes IN and Bikes OUT per day are quite closely related. There is no significant difference between Bikes IN and Bike OUT. Therefore, it can be assumed that most people take their bikes back for the day instead of leaving them overnight.

2. The number of bikes in use per day:
It can be assumed that due to the Covid-19 pandemic, the level of traffic in 2020 was down nearly 50% compared with a year ago.

3. The average number of bikes in use by weekday:
The number of people using DublinBikes on weekdays is more than that on weekends.

4. The usage percentage:
The average hourly usage percentage is less than 25%.
Most bikes are used during at daytime and the peak hours are from 7AM to 9AM and from 4PM to 6PM. In addition, when considering the details of each 5-minute interval, the times with a high rate of bike usage (greater than 80%) over the past two years are only 0.0046% - very low. It means that the usage percentage of DublinBikes at below a ”Medium” level. In the near future, the Department of Transport don’t need to buy more bikes. Instead, redistributing the bike at each station for more efficiency is a better way.

5. Stations analytics:
This part focuses to find the top and the bottom stations via their level of traffic. The top stations are called ”Crowded stations” (lack of available bikes) and the bottom stations are called ”Quiet stations” (too many available bikes).

While there are 8 ”Crowded stations” with ZERO BIKES PERCENTAGE greater than 25%, the number of ”Quite stations” with ZERO BIKES PERCENTAGE less than 3% is 3. For example, the station ”SMITHFIELD” (ID = 35) has a significant ZERO BIKES PERCENTAGE (at 49%). In this case, the Department of Transport should bring more bikes (get from ”Quiet stations” which have ZERO BIKES PERCENTAGE less than 3%) to this station. And also consider redistributing the bike to the remaining list of ”Crowded stations” with ZERO BIKES PERCENTAGE greater than 25%.
