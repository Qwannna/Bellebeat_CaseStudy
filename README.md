# Bellebeat_CaseStudy
A case study for Bellabeat smart device usage
# Bellabeat Fitbit Analyst 

### By: Anna Ray
  Date: 11/27/2024
  
### Project Overview
I have been asked to analyze smart device usage to gain insight into how customers use Bellabeat Smart devices.

### Case Study of Bellabeat Smart device data
Introduction and Business task.
This is my Case study using on the Bellabeat fit-bit fitness tracker data set using R. Here I will perform real-world tasks of a junior data analyst.
Bellabeat is a high-tech manufacturer of health-focused products for women. Bellabeat is a successful small company founded by, Urska Srsen and Sando Mur, who believe that by collecting data on activity, sleep and stress their technology can inform, inspire and empower women around the world with knowledge about their own health and habits. Founded in 2013 Bellabeat grew rapidly, and by 2016 had offices around the world with multiple products.
I have been asked to analyze smart device usage to gain insight into how customers use non-Bellabeat Smart devices.

The main insights I was asked to find out are as follows:
•	What are 3-6 trends in smart device usage?

•	How could these trends apply to Bellabeat customers?

•	How could these trends help influence Bellabeat marketing strategy?

Using these questions, I will find trends in smart device usage by finding what customers used their devices for the most. I will also look to see if time of day is a factor in usage as well. I will also find trends within the most active users and show how many ways customers can use their smart devices’. Using these findings, I will find ways we can get our customers to be more active and gather new ones.
The data comes from Kaggle(FitBit Fitness Tracker Data) and is license by CC0 :Public Domain By user name Mobius. Using this data I have downloaded from Kaggle, I will run an analysis Over the usage of 30 customers from (4/12/2016) April 12th, 2016, until (5/12/2016) March 12th, 2016.
The data holds daily activity for 30 days following our 33 customers showing us Activity time, Sleep values, Step count, Calories and MET values. This data only has female records.
I will start by bringing the data in to see what we are working with and start cleaning it. I will download packages to start cleaning and plotting the data. The data is in a comma separated values file type or a cvs file type.

## Data Source
Bellabeat data source : From [Kaggle.com by ](https://www.kaggle.com/datasets/arashnic/fitbit)

### Tools
 - Excel for cleaning and understading data
 - Rstudio for Data Analysis

## Data Cleaning
- Data was cleaned and origized using Excel.
- Untis of measurement found while cleaning the data in Excel

### Data Analysis

Here is an example of some code used for analysis in Rstudio

```
 Daily2 <- Daily2 %>% 
  mutate(Mean_activityLevel = case_when(
    avgTotalsteps < 5000 ~ "Sedentary lifestlye",
    avgTotalsteps >= 5000 & avgTotalsteps < 7500 ~ "Low active",
    avgTotalsteps >= 7500 & avgTotalsteps < 9999 ~ "Somewhat active",
    avgTotalsteps >= 10000 & avgTotalsteps < 12500 ~ "Active",
    avgTotalsteps >= 12500 ~ "Highly active"
  ))

colnames(Daily2)
```

### Results and Findings
The results are as follows:
1.	Users tend to be very active throughout their daily lives despite how many overall steps taken in a day.
2.	Consistent users achieved weight and calorie loss while improving in step count each week.
3.	Users who had higher steps and decent sleep took breaks throughout the week.

### Recommedations

1.	Goal hitting and high performing users could share their processes weekly to encourage and help other users stay focused and hit their own goals.
2.	Customers who have trouble sleeping or falling asleep could be offered a trial period with health professionals to help sleep regulation.
3.	Send a notification around 3pm informing users of their progress and congratulating them on their hard work Allowing them to acknowledge how far they have come in a day to encourage and strong finish and sense of accomplishment.


-	Team up with sleep experts to help users get more sleep and higher sleep quality. Using our data, we can market our devices to help users get sleep regulation and better quality.
-	Allowing users to share their accomplishments with other users gives a sense of community and Camaraderie. This should also be noted as a goal among users since they are competing each week to reach their own individual goals, rather it be sleeping goals, stress, weight, steps, time spent active or even time spent resting.
Actions to be taking based off data.

Encouraging Physical Activity
-	Sedentary Activity Alerts: By sending notifications during extended periods of sedentary activity, we can encourage users to get up and walk more, promoting regular movement and reducing inactivity.
Enhancing Sleep Patterns
-	Sleep Data Utilization: Using our sleep data, we can help users set up healthy sleep patterns. For those who have trouble falling asleep, we could offer meditation music or short videos to help them relax and de-stress before bed. For users who do not have a sleep schedule we could help them adjust to the best one that follows their daily lives.
Promoting Daily Exercise
-	Workout Timing Insights: The data reveals when and on which days users are most likely to work out. Depending on their daily lives, they may already walk plenty throughout the day. I would suggest having weekly goals set by users. Users who do not meet their weekly goals can receive notifications encouraging more daily steps through their everyday actions.
-	Daily Goals Achievement: Sending notifications when users meet their daily goals can motivate them to rest and feel a sense of accomplishment for their hard work.
  
Building Community and Support
-	Shared Goals and Social Interaction: If users are near each other, they could share their goals with other members or have weekly gatherings to walk together. This social aspect can boost motivation and create a supportive environment for achieving fitness goals.
Marketing
-	Adding a sleep application:  Would encourage new customers and existing customers. We could use this application to help promote and regulate sleep patterns for customers. Offering their first month for free will give us time to analyze data and for customers to get into a routine of checking the app daily. 
-	Weekly and Daily goals: High performing users who are constant in hitting their goals and expanding their goals could receive Bellabeat merch or discounts on other Bellabeat products.
-	Reliable Health Professionals:  By teaming up with insurance services and medical professionals, we could provide subscription-based articles and workouts for users. Having workout videos based on after surgery or post-surgery, could bring in all types of users who are solely focused on improving their health. 

