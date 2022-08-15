# Ford GoBike System Data Exploration
## by Emmanuel Jonah


## Dataset
This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area from 1st to 28th February 2019. It contains about 183,000 individual trip records. The attributes include: duration, start and end times, start and end stations, membership type and gender and id of the bike used.

Before the analysis, some wrangling (gathering, assessing and cleaning) of the data was done.
* The data was retrieved from a link https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv
* No records were removed
* The following attributes were created:
>* duration_min: minutes of the _duration_sec_ column
>* start_day_name: day of the _start_time_ column
>* end_day_name: day of the _end_time_ column
>* start_day: day value of the _start_time_ column
>* age: calculated age of from the _member_birth_year_ column
>* social_generation: social_generation based on article from Wikipedia https://en.wikipedia.org/wiki/Generation#List_of_social_generations

## Summary of Findings
>* Trip duration has a long-tailed distribution, with a lot of trip on the low price end, and few on the high price end. When plotted on a log-scale, the trip duration in seconds distribution is unimodal, with the peak between 500 and 1000.
>* There is very little difference in the number of trips that start and end within an hour. Also, the maximum of the start and end number of trips occur at 8-9 AM and 4-5 PM
>* Most bike users under this project have subscribed to the project, that is 158,386 persons representing 90.53% of all users.
>* From this visualization, it can be noted that most of the bikers are males, representing 74.59% as compared to Females and Others
>* Weekdays have the largest proportions which translate into number of trips (sum of 83.5%) as compared to the weekends
>* Generation Y that is persons born between 1981 and 1996 patronize the bike services more that all other generations.
>* The Customer user type tends to conform with the office hours trend where there is peak activity at 8-9 AM and 4-5 PM on weekdays. On the other hand, the Subscriber user type only conforms to the office hours trend for the afternoon (that is 4-5 PM) on Tuesday, Wednesday, Thursday and Friday only.
>* Bikers between the ages of 20 and 50 have the longest trips in minutes
>* Trips with duration greater than 200 minutes are completed by bikers between the ages of 20 and 60
>* Bikers older than 80 years do not ride bikes more than 100 minutes



## Key Insights for Presentation

>* Generation Y that is persons born between 1981 and 1996 patronize the bike services more that all other generations.
>* The Customer user type tends to conform with the office hours trend where there is peak activity at 8-9 AM and 4-5 PM on weekdays. On the other hand, the Subscriber user type only conforms to the office hours trend for the afternoon (that is 4-5 PM) on Tuesday, Wednesday, Thursday and Friday only.
>* Bikers between the ages of 20 and 50 have the longest trips in minutes
>* Trips with duration greater than 200 minutes are completed by bikers between the ages of 20 and 60
>* Bikers older than 80 years do not ride bikes more than 100 minutes