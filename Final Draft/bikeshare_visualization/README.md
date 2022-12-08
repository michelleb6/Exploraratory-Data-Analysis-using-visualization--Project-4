# Bay Wheels Bike Sharing System Usage Pattern 2018
## by Michelle Bleyl


## Dataset

> Bay Wheels (Ford GoBike System Data) stores information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. It's bike sharing rental service company with nearly 500,000 rides since the launch in 2017 and had about 10,000 annual subscribers in January 2018. The dataset is used for exploratory analysis that includes daily usage time and information about the customers.

> Data wrangling process:
* Drop rows that have null values. Columns: station id, station name, end_station_id, end_station_name, member_birth_year, member_gender.
* Correct multiple columns of their data types: 1) start_time and end_time should be datetime type,2) user_type and member_gender should be categorical data type 3)change station id, member id, and bike id into a string 4)Change member's birth year and age into integer, etc
* Add new columns for trip duration in minute, trip start date in yyyy-mm-dd format, trip start hour of the day, and day of week 
* Add a new column that calculates member's age from 'member_birth_year'
* Filter out the outlier ages 
* Filter out outlier trip records where the duration is very long


## Summary of Findings

> The number of trips peaked around 7-9am and 16-18pm which are during rush hours. There are more riders in weekdays(Mon-Fri) compared to weekends. The riding trips tend to be shorter on weekdays compared to weekends. This shows that riders who uses on weekdays during rush hours have more stable efficient use than casual weekend users. 

> The majority riders were male subscribers who did not use bike share for all trips. Most member's age were around 25 to 40 years old. Subscribers are slightly older than customers. Also, male riders are slightly shorter than femal riders. 

> There are a lot more subscriber usage than customers overall. Riding habits of subscribers are more likely to use in weekday during rush hours indicates that they are using for commuting to work. Whereas  customers tend to ride for fun in the afternoon over weekends. This is shown in the plot that subscribers usage peaks out during rush hours when people go to work in the morning and getting off work in the evening, which strengthened their usage purpose and goal of riding. Customers pattern is not similar with subscribers which they don't have a significant peaks rather they don't have much difference between weekdays and weekends. This is also shown when they use which they don't have a significant peaked time on usage. 


## Key Insights for Presentation

> As mentioned above, there were different patterns and habits between subscribers and customers. Subscribers uses heavily on work days during rush hours whereas customers ride a lot on weekends, especially in the afternoon. Many trips concentrated around 7-9am and 16-18pm on work days for subscribers. On the other side, customers tend to use more in the afternoon during weekdays. Subscribers using efficient/short period and high concentration on rush hours during weekdays, indicates that their primarily purpose is for commuting to work. For customers, they have a more relaxing and flexible pattern and use on afternoon during weekends, indicates that they're taking advantage of the bike sharing system. Thus, the two type of riders have quite different habits.