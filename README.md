# Bikesharing

# Overview of the Analysis
In this project, I am tasked with analyzing the bike-sharing business in New York City. Specifically, I will work with the data provided by the bike-sharing company, CitiBike. Based on the observed data, I aim to find common trends and create clear and easy-to-grasp visualizations. The dashboard built in this project will be useful to investors who want to invest in a bike-sharing business, whether in New York or another city. However, it is important to understand that some patterns might be specific only to New York and might not be applied to other cities. 

## Data 
- The dataset used in this project is the Citi Bike bike-sharing data for August 2019 in a CSV format.
- The dataset "201908-citibike-tripdata" was extracted from [here](https://ride.citibikenyc.com/system-data).
- There are 2,344,224 rows corresponding to individual rides.
- There are 15 columns for trip duration, start and end times, start and end stations, latitude and longitudes for start and end locations, bike ID, user type, user age, and gender. 

## Tools and Languages
* Tableau visualizations and dashboard
* Python and Pandas functions

# Results

## Deliverable 1
Using Python and Pandas functions, the data type of the ```tripduration``` column was converted from an integer to a datetime format of the time in **hours, minutes, and seconds**. The code is available [here](https://github.com/Aigerim-Zh/Bikesharing/blob/main/NYC_CitiBike_Challenge.ipynb). 

## Deliverable 2 and 3
Tableau dashboard for this project is saved [here](https://public.tableau.com/app/profile/aigerim.zhanibekova5544/viz/Book1_16530886055830/NYCStory?publish=yes).

### Basic Overview 
![](https://github.com/Aigerim-Zh/Bikesharing/blob/main/Visualizations/Basic_Overview.png)

Knowing the breakdown of customer types and their gender will help us understand the customer base. Figuring out the peak usage hours will help us understand how many bikes are needed during a particular hour of the day.

### Checkout Times for All Users
![](https://github.com/Aigerim-Zh/Bikesharing/blob/main/Visualizations/Checkout_Times_for_Users.png)

The graph below shows that most of the checkout times are under one hour in length. 

### Checkout Times by Gender
![](https://github.com/Aigerim-Zh/Bikesharing/blob/main/Visualizations/Checkout_Times_by_Gender.png) 

From the graph, we can see all three genders tend to checkout in less than one hour. It also illustrates that male-identifying users have significantly more bike trips than female and unknown genders.

## Trips by Weekday for Each Hour

![](https://github.com/Aigerim-Zh/Bikesharing/blob/main/Visualizations/Trips_by_Weekday_per_Hour.png)

The heatmap illustrates bike hourly usage patterns for each weekday. Several observations can be made from the heatmap:
- From Monday to Friday, the heaviest bike usage is during the regular commute hours:  
    - From 6:00 am to 9:00 am with the busiest time at 8 AM during all weekdays.
    - From 5:00 pm to 7:00 pm. 
- The highest traffic is observed on Thursdays during morning and evening commute hours. 
- During the weekends, the bike usage is spread throughout the middle of the day, and more so on Saturday. 
- One peculiar observation is the lowest bike usage on Wednesday during after-work hours. The reason behind this should be investigated further.

## Trips by Gender by Weekday per Hour

![](https://github.com/Aigerim-Zh/Bikesharing/blob/main/Visualizations/Trips_by_Gender_by_Weekday_per_Hour.png)

The same trend as above is observed when divided by gender. The heatmap above also confirms that males tend to bike substantially more than female and unknown genders. 

## User Trips by User Type by Gender by Weekday

![](https://github.com/Aigerim-Zh/Bikesharing/blob/main/Visualizations/Trips_by_UserType_Gender_by_Weekday.png)

The visualization below demonstrates that there are more subscribers than short-term customers. It also further shows that the subscriber count is dominated by males.  

## Top Starting Locations 

![](https://github.com/Aigerim-Zh/Bikesharing/blob/main/Visualizations/Top_Starting_Locations.png)

It is useful to know in which areas the bike traffic is the heaviest. The most popular starting locations are marked by larger symbols on the map above. For example, most rides happen in this location: 125 Park Avenue, New York, NY. In general, most bike riders are concentrated in the area of Lower Manhattan, which is known for the highest number of tourists and limited parking spaces.

## Trips by Age

![](https://github.com/Aigerim-Zh/Bikesharing/blob/main/Visualizations/Trips_by_Age.png)

In general, the number of trips increases with age until 1990, after which it significantly decreases with age. This trend is expected since the people born after 1990 might not have yet started working and, therefore, use bikes less. 

# Summary
Based on the analysis above, I can make the following high-level summary:
- Most bike users are subscribing male-identifying customers. I think it is important to investigate why it is the case and make efforts in attracting female customers.
- The traffic is heavily concentrated in areas with limited parking spaces and a large number of tourists.
- The busiest hours from Monday to Friday are morning and evening commute hours. 
- The busiest hours during weekends are in the middle of the day. 

I would suggest the following additional visualizations for future analysis: 
1. Average Trip Duration by Age;
2. Average Trip Duration Gender; 
3. Average Trip Duration by Age by Gender; 
4. Top Start and End Station Locations by Weekday per Hour.