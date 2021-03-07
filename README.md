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

