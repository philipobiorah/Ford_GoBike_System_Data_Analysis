# Ford GoBike System Data Exploration

## Dataset

This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. The dataset consisted of 183412 rows and 16 columns.  The dataset can be found [here](https://www.google.com/url?q=https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv&sa=D&source=editors&ust=1662142838313239&usg=AOvVaw3LqBTuVNmAzV169iQzKF9l)

## Data Wrangling
#### Quality 
The following issues where cleaned

Incorrect datatype for start_time, end_time, member_birth, start_station_id, end_station_id, member_birth_year
Missing values in member_gender, member_birth_year, end_station_id, start_station_name, start_station_id and end_station_name
No special column for age, day, and month
Lattitude and longitude are great features but we cannot immediately get insight for them without performing some calculations of the distance covered

##### Feature engineered columns:

* day
* month
* member_age
* distance_km
## Summary of Findings

The highest record of trips occured in 10mins (600 secs). Majority of the distances covered ranged from 0.1 to 2.5 km. This demonstrates that the majority of trips were not long distances. Male riders constituting 75%, Female riders 23% and others 2%.

Thursdays had the highest usage, followed by Tuesdays and Fridays. Saturdays and Sundays saw a significant decrease in usage. This suggests that bikes are mostly used during the week and/or that people prefer to stay at home on weekends, resulting in less use of bikes.Thus, Riders spend more time riding on Sunday, Saturday than on workdays(Mon - Friday)

Most bike riders fall between the ages of 25 to 40 year. Individuals between 30-35 have the heighest number of rides. Subscriber users account for 90.9% of all bike rides, while customer users account for only 9.1% of all bike rides.



## Key Insights for Presentation

For the presentation  focus on  the relationship between gender and user type; the relationship between distance covered and trip duration; what day of the Week do riders spends the most time.
Using a clustered bar chat we demontrate the relationship between gender and user types. We examine the investigate  the different user types (Subscriber and Customer ) across gender spread in relation for the No. of bike rides. 

Afterwards we use a scatterplot with a regression line to show the positive correlation between distance(km) covered and duration(secs). In other to investigate which day of the Week riders spends the most time riding, we used a barplot we to demonstrate the relationship between duration(sec) and day(weekday)
