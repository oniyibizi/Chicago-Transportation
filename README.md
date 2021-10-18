# Chicago Method of Public Transportation Analysis
Final Project for Data Engineering Course from Masters of Science in Analytics Program 


## Executive Summary:
The usage of e-scooters is quickly emerging as a popular method of transportation in various metropolitan cities. In the summer of 2019 the city of Chicago launched their own pilot program to track rider usage. With the growing interest in this method of transportation, it is important for the city to determine if they want to invest and allow companies to operate these e-scooters in Chicago. 



## Business Case:
Analyze the E-scooter pilot program in addition to other methods of transportation and their impacts to better prepare governmental agencies when planning transportation infrastructure for their communities.


## Data Source:
https://data.cityofchicago.org/ 

## Data Model:

![image](https://github.com/oniyibizi/Chicago-Transportation/blob/main/images/DataModel.png)


## Dashboards & Viszulations from Tableau:

![image](https://github.com/oniyibizi/Chicago-Transportation/blob/main/images/DivvyDashboard.png)

![image](https://github.com/oniyibizi/Chicago-Transportation/blob/main/images/EScooterDashboard.png)

![image](https://github.com/oniyibizi/Chicago-Transportation/blob/main/images/Comparision.png)


## Data Preparation & Platforms:

●	Extract: Given that we needed to extract data from various data sets, as a team we used both **R** and **Python** to extract the data using the API key that was provided. This also allowed us to leverage the API call to extract the specific data that we needed based on the year.   

●	Transform: Using various tools including, **R**, **Python**, and **OpenRefine**, we were able to remove unnecessary attributes, merge datasets, and create a additional to determine fare charges if they were not there.  

●	Load: Using the storage and SQL modules on **Google Cloud Platform** we were able to store our datasets on the Google cloud which alleviated the need for storage space on our local machines and allowed for group member to access the datasetes. We were then able to push said datasets from storage directly into a **MySql** server on the cloud in an effective manner given the size of our large datasets




## Data Cleaning & Profiling:
●	Due to the pilot program only running at certain times we looked at data from June 15,2019 to October 15,2019 and June 15, 2018 to October 15, 2018.  
●	Leverage GCP to store data while also building necessary tables in MySql.  
●	Use SQL to combine similar data sets for Divvy Ridership and E-Scooter Ridership.  
●	As we were extracting data we realized that the datasets we were collect were rather large and made it difficult to extract the information with just one run, as a result, we did the extract in chunks. However given the time constraints we had with in this project, we concluded that we did not have enough storage, time, processing power etc. to extract rideshare data. As a result, while we did have it in our initial scope we did have to exclude from our insights and conclusion.  
●	Given that we no longer were looking at rideshare data, we decided to look at Divvy bike information as it is more applicable and comparable to the short-form trips that we expect from E-Scooter riders.  
●	In the Divvy dataset, we treated all riders as "Customers" rather than also have "Subscribers".  
●	Created a cost column, with the hope of being able to provide additional insights on which option is the most cost efficient for customers.  

## Recommendations & Lessons Learned: 
●	Recommendations:E-scooters averaged 34,405 rides for the duration of the program (June 15th to Oct 15th 2019), which shows there is demand for these modes of transportation, although other types of transportation have been around longer, including metro and bus. Another extremely viable option is the divvy bikes and it may be interesting to conduct a deeper analysis on the differences in user-ship between self-operated short-form transportation methods.    
●	From analysis such as this, we can also begin to make recommendations to the city of Chicago about where to place and/or remove the divvy stations and e-scooters.  
●	Lessons Learned: Do a thorough data check before using the data.  We did some spot checks, it wasnt't until we began to pull the data that we realized size and storage would quickly become an issue  
●	Duplicated data can indicate missing data.  
●	In an ideal world, I would have loved more time to work on this project. We would like to have included rideshare data however, the datasets were too large given the scope of the project with limited time and resources  
●	Ultimately, using the this current data, in addition to rideshare, CTA train, and CTA Bus data, we could help develop a platform to help consumers know which method of transportation would be most efficient for them.
