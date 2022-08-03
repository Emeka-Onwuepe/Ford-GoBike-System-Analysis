# Ford GoBike System Data Analysis
## by ONWUEPE EMEKA

## Dataset

> Our dataset consists on 183412 sample of individual rides made in Ford GoBike bike-sharing system covering the greater San Francisco Bay area trips in february 2019, with 16 features (duration_sec, start_time, end_time, start_station_id, start_station_name, start_station_latitude, start_station_longitude, end_station_id, end_station_name, end_station_latitude, end_station_longitude, bike_id, user_type, member_birth_year, member_gender, bike_share_for_all_trip)

>We cleaned missing values in start_station_id start_station_name end_station_id end_station_name, member_birth_year and member_gender features, corrected a wrong member_birth_yaer entry, converted start_time, end_time, bike_id, start_station_id, end_station_id and member_birth_year to their appropriate datatypes. We also calculated distance from start_station_latitude, start_station_longitude,end_station_latitude and end_station_longitude features and dropped them. We converted duration_sec to duration_hr, member_birth_year to age and created age_group from age.  

## Summary of Findings

In the exploration, we found out that majority of the riders are men from the 18-39years followed 40-60years and most of them were not just members but subscribers. Trips occurred more from Tuesday to Friday with Thursday as the highest and Sunday the lowest while the busiest hours are 7am - 9am and 4pm - 7pm. Bearing in mind that the majority of the users are within the age of 18-39 and 40-60 which could be called the working/business class, one could argue that the busiest hours are actually the time they should be going to work/ventures (7am - 9am) and when they should be returning home (4pm - 7pm).

The first Week, 4 - 10 (first Monday - Sunday) did better than the second week (11-17). We can argue that there was a drawback in the second week making the week 1 high the resistance level. The resistance was broken on the third week (18-24) making it the new resistance level till it got broken on Thursday 28 feb. Generally, our chart started making higher lows and relatively higher highs as from feb 9, which denotes an uptrend. Thus, the business made progress in the month of feb, 2019.

The energetics and subscribers are more likely to embark on long-distance rides. On average all age group travels almost the same distance though the tendency to travel more distance decreases as age increases. Contrary to the initial weak correlation observed between distancce_km and duration_hr, reshape the them under time series reveals that they are actually positively correlated.

(Market St at 10th St) generated the highest start trip while (San Francisco Caltrain Station 2 (Townsend St at 4th St)) generated the highest end trip. One might at first be tempted to conclude that (Market St at 10th St) - (San Francisco Caltrain Station 2 (Townsend St at 4th St)) would be the most travelled route but that's wrong though it made it to top eleven. The most travelled route from our dataset is (Berry St at 4th St) - (San Francisco Ferry Building (Harry Bridges Plaza)). What makes it more interesting is that (Berry St at 4th St) is the third highest start strip station while (San Francisco Ferry Building (Harry Bridges Plaza)) is the fourth highest end trip station.

The missing data we had in birth_year and gender came from stations with high demands. Thus, we can argue that the omissions might be due to rush to attend to high demands

Majority of the rides travelled alone. Customers and those with missing birth_year and gender travelled alone the most.

## Key Insights for Presentation
Our presentation is based on the when( time and days ) with high rates of rides. We first looked at the riders' gender,age_group and user_type distributions. We then look at the the number of rides according to the days of the week throughout the month of feb., the busisest time of the day uing the distance covered and finally looked at the daily distance trend.