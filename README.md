# Google-Data-Analytics-Capstone-Case-Study
Cyclistic Ride-Sharing Case Study

Google Data Analyst Capstone Project


This case study is for Google Data Analysis Capstone Project on Coursera. 

In this case study, I will be taking the role of a junior data analyst for a fictional bike-sharing company called Cyclistic to answer the key business questions. I will follow the steps of the Data Analysis Process: Act, Prepare, Process, Analyse, Share, and Act.

1. Ask: The description of the business task.

We are using the data trip from 2019 Q2 to 2020 Q1 from Cyclistic to answer questions like how casual riders (non-subscribed users) and members (subscribed users) use the bike-riding service to identify a strategy to entice casual riders to become members, or to use our services during identified casual off-peak times. We also wanted to identify the peak times of the year to spend our advertising budget efficiently. We will consolidate the data into one data frame using R and Rstudio.

2. Prepare: Prepare the data.
   
I used the 12 months of Cyclistic trip data (2019 Q2 to 2020 Q1) to perform the analysis. This data is split into 4 different files for each of the different financial quarters. The data is available for public use by Motivate International Inc and can be downloaded through this link. 
I used R and RStudio to have the data collected, wrangled, cleaned, stacked, manipulated and combined to perform my analysis. I will outline the steps with code samples to show my steps of the Data Analysis Process.

3. Process: Cleaning data for better management.

Here is what I did to clean the data during this phase:

I imported the Excel files Divvy_Trips_2019_Q2.csv, Divvy_Trips_2019_Q3.csv, Divvy_Trips_2019_Q4.csv & Divvy_Trips_2020_Q1.csv as data frames q2_2019, q3_2019, q4_2019 q2_2019, and q1_2020.

I renamed columns in the q2_2019, q3_2019, and q4_2019 data frame to match the most up to date data frame q1_2020 

I converted the datatypes of the columns so the data frames would be consistent.

I removed unwanted columns so that the data would stack correctly when the dataframes are combined. I also removed identifying information such as names and birthdays.

I renamed the labels in member_casual column from “Subscriber” to “member” and “Customer” to “casual” so that the member_casual column can be consolidated for consistency.

I added columns of data (date, month, day, year, day of week) that provide additional opportunities to gather data.

I added a field through calculations for a length of a ride.

I deleted ride durations that were in the negatives.

I deleted all values that were null or empty. 

I aggregated all the data to show the mean , median, max and min for casual and member riders for the analysis. 

4. Analyse

Please find the visualisations in the repository.

![Number of rides by rider type](https://github.com/Hudeal/Google-Data-Analytics-Capstone-Case-Study/assets/79075880/da368797-9721-45cc-9e91-e2cbca4f8427)


5. Share

As one can see from the “Number of rides by rider type” graph, Members use Cyclistic much more that Casual riders during weekdays, most likely to get to and from work. And while Member usages are reduced significantly during weekend, there is a notable uptick in casual riders during the weekends. This most likely happens because most Members do not work weekends and Causals use the service more for transport to relaxation or relaxation.

It is notable in the “average duration” graph that that Casual riders will, on any day of the week, significantly use their bikes for longer durations than members. One can deduce that, since most members use our bikes to and from work, they just want to get from point A to B as quickly as possible, while Casual riders are more likely to go to multiple points throughout the day.

The inference that most members are work commuters is reinforced when one looks at the “Total Number of Rides Per Hour of the Day of Member & Casual” graph. The graph shows that members use the service mostly between 6:00 and 9:00 (the time in which most commuters travel to work) and 16:00 and 19:00 (the time in which most workers return home from work).

The “Total Number of Rides Per Month of Member & Casual” graph shows a major increase of usage by Members from April to August (mid-spring to late summer) with a major increase of Casual usage from May to June (late-spring to late-summer.) This usage starts to decline, for members and casuals, in September (early autumn), followed by major drop-off during November (late autumn). From the above, one can conclude that riders of both groups prefer ride bikes during the warmer spring and summer months and seek other means of transport during the colder autumn and winter months.

6. Act

We can see that casual riders use our service less during weekdays than members riders. We can perhaps increase casual riders’ trips during weekdays by advertising in commuter hours (06:00 - 09:00 and 16:00 - 17:00).  

We also see a major uptick in use during the mid-spring & summer months. We could increase usage even further during these months by advertising our services more during this period.
