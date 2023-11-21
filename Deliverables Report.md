# Deliverables Report

Index
1. A clear statement of the business task
2. A description of all data sources used
3. Documentation of any cleaning or manipulation of data
4. A summary of your analysis
5. Supporting visualizations and key findings

## 1. A clear statement of the business task
The business task is answering the question on how subscribers and customers use Cyclistic bikes differently. By finding out how their usage differs, we can more accuratly target our marketing efforts. The end goal of the marketing strategy is to convert casual riders into annual members. 
Key stakeholers for this task are the Cyclistic analytics team, marketing team, and executive team, as well as their customers. 

## 2. A description of all data sources used
The data analyzed is company data about the usage in the four quarters of 2019. The data consits of trip details on every single bike ride in 2019. The base file has the following columns, though naming is slightly different in the file of Q3:

trip_id	--> The ID number of the trip <br>
start_time	--> The start time of the trip<br>
end_time	--> The end time of the trip<br>
bikeid --> The ID number of the bike used	<br>
tripduration --> How long the trip was in seconds<br>	
from_station_id	 --> Starting station ID number<br>
from_station_name	--> Starting station name<br>
to_station_id	--> End station ID number<br>
to_station_name	-> End station name<br>
usertype --> Type of user, either a customer or subscriber<br>	
gender --> User gender, either male or female	<br>
birthyear --> User birthyear<br>

As this data is from the company itself, it is determined to be reliable. It seems to be complete, consistent and mostly acccurate. 
There is no private information about the user, so there are no privacy conserns. The data was downloaded and stored on a secured laptop. 

## 3. Documentation of any cleaning or manipulation of data. 
These are all the steps we took in cleaning and preparing the data:
1. Change the column names in the Q2 to match the rest of the Q1,3,4 files.
2. We merge the datasets
3. We convert the date-time columns to the right format
4. We look for missing values
5. We clean up tripduration, and cap it at 24 hours.
6. We clean up birthyears, and remove instances before 1900.
7. We adjust the ride length to the right format.
8. We create a day of the week column.
9. We remove the negative ride times.
    
 ## 4. A summary of your analysis
We analyse the following: 
1. We want to know which days of the week are the most popular for each type of user. We create a dataframe of the weekly totals by group. Then we calculate the proportions. Finally we plot it.
2. We calculate the time of the days, and calculate this proportianlly to the total respective number of rides.
3. We calculate the difference in tripduration.
4. We calculate the most popular start and end station by user type.
5. We analyse the genders and their distribution by user type.
6. We analyse the ages and their distribution by user type.
7. We extract the month from the start time and calculate seasonal usage pattersn
8. We check the standard devitiation across user types.

 ## 5. Supporting visualizations and key findings
 1. Relative Ride Proportion by Day of the Week.png shows the relative ride proportion by user tyupe. We can see that subscribers have more bike rides during the week and customers more during the weekend.
 2. Relative Ride Proportion by Hour of the Day.png shoes the relative ride distribution by hour. We can see that subscribers use more bike rides during rush hour times and customers are more spread out through the day. Combining this with the finding in 1 we can deduct that subscribers use the bikes more for commuting and customers use it more for leisure.
 3. Average and Median Ride Duration by User Type.png shows the duration of the trips, both average and median. We can see that customers take longer bike trips than subscribers.
 4. Top 10 Start Stations by User Type.png & Top 10 End Stations by User Type.png show the most popular start and end station. We can see that there is very little overlap between the stations that are being used. Customers start and end at different stations then subscribers.
 5. Relative Gender Distribution by User Type.png shows the distribution by gender. We can see t hat in both user types there are more males that females. We can also see that the proportion is closer together in the customer type than it is in the subscriber type.
 6. Relative Age Distribution by User Type.png shows the age distribution by user type. We can see that customers tend to be a bit younger and more concentrated in certain age ranges. Subscribers are a little older and are more spread out age-wise.
 7. Seasonal Ride Proportion by User Type.png sgiws the proportial bike rides by user type. We can see that both user types ride more bikes in the summer. This is logical because summer has better weather. Subscribers however, ride relatively more throughout the year, as they use the servicer to commute to work. Customers use it more leisurely in the summer.
 8. Ride Time Predictability by User Type.png shows that customers deviate more in their ride times and subscribers are more conistent. This makes sense as subscribers often go the same route to commute.

There are still remaining questions for some of the why's. Why do use men this service more, for example. What are the routes that people take? We had no information on the coordinates of the stations. Are there any other selling points for subscribers, different from commuting? 

Bringing the key findings back to our original question and purpose, we can deduct that our marketing efforts should focus on pushing customers to use the bikes to commute to work. We can target older customers in their late twenties, as they are most likely to be a subscriber. We can also target men more. As people use the service more in the summer, our marketing efforts should look at late spring to be a good time to increase marketing. There are also geographical implications, as it might be good to target customers near the most popular stations for subscribers. 

These recommendations can be a guide to increase the succes of the marketing efforts. 


