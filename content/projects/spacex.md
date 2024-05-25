---
title: "SpaceX Rocket Analysis"
date: 2023-11-20
draft: false
links:
  - icon: fab fa-github
    url: https://github.com/Kolinhtetwin/SpaceX_Rocket_Analysis
author: "Lin Htet Win"
tags:
  - Python
  - Pandas
  - Numpy
  - SQL
  - Matplotlib
badges:
 - Python
 - Pandas
 - Numpy
 - SQL
 - Matplotlib
image: /projects/spacex/Space_X_falcon_9_landing.jpeg
description: ""
toc: 
---

This is the final capstone project where I have to utilize the data analysis tools that i learned from IBM data science. The things I have to do in this project are
- Data collection with api and webscraping
- Data Wrangling
- Exploratory Data Analysis using SQL
- EDA Data Visualization Using Python Pandas and Matplotlib
- Launch Sites Analysis with Folium-Interactive Visual Analytics and PlotyDash
- Machine Learning Landing Prediction

## Data collection with api 
First, I request the necessary data from the SpaceX REST API.

![Request Data from SpaceX Rest API](/projects/spacex/request_api.png)

Then, I use json_normalize meethod to convert the json result into a panda dataframe. 

![Normalize Data into Dataframe](/projects/spacex/normalize_json.png)

Then, I analyze the features and labels of the dataset. Finally, I filter the dataset to include only Falcon 9 launches.

![Filter Data](/projects/spacex/Filter_data.png)
<hr>

## Exploratory Data Analysis using Pandas
In this part, I perform exploratory data analysis using Pandas library. First, I try to see how FlightNumber (indicating the continuous launch attempts.) and Payload variables would affect the launch outcome. For payload mass exceeding 10,000 kg, the launch attempts are more successful compared to those with lower payload masses. Starting from the 79th attempt, all launches have been successful regardless of the payload mass.

![Payload x FlightNumber](/projects/spacex/payload_flightnumber.png)

After that, I try to find the patterns between the FlightNumber and Launchsite based on the success rate for landing. Based on the scatterplot, CCAFS SLC 40 and KSC LC 39A has the 100 percentage success rate for above 80 Flight Number. Although KSC LC 39A has no data below 20 FlightNumber, its success rate for between 40 and 65 Flight Number is also 100 percentage. CCAFS SLC 40 has launched more flight than other two launch sites.

![FlightNumber x LaunchSite](/projects/spacex/flightnumber_site.png)

Based on the relationship between payload and launch site, CCAFS launch site has the most flight than other site. VAFB SLC 4E site doesn't launch the flight that weighted more than 10,000 payload mass. KSC LC 39A site has 100% success in launching the flight that weighted between 2000 and 5000 payload mass.

![Payload x LaunchSite](/projects/spacex/payload_launchsite.png)

Additionally, I analyze the average success rate over the year. From 2013 to 2020, the success rate exhibited a consistent upward trend. Notably, the year 2019 recorded the highest success rate within this period, reaching an impressive 90%.

![Average Success Rate](/projects/spacex/average_success_rate.png)

**Based on the exploratory data analysis, the key insights are**
- For payload mass exceeding 10,000 kg, the launch attempts are more successful compared to those with lower payload masses.
- If you want to try launching the payload mass between 2000 and 5000, KSC LC 39A site has been the best launch site.
- CCAFS SLC 40 has succeed every launch attempt for payload mass greater than 10,000 kg.
- According to the analysis of the average success rate over the years, the success rate has increased dramatically from 2015 to 2019, reaching an impressive 90%.

<hr>

## Machine Learning 
With exploratory data analysis, I split the data into training and testing data. I use GridSearch Cv to find the best parameters from the parameters I provided and use four different machine learning to find which machine learning is the best to predict the successful landing.

According to the graph, Decision Tree performs well on train accuracy but the test accuracy is pretty low compared to other machine learning models. Logistic Regression, Support Vector Machine and K Neares Neighbors performs nearly the same on the validation accuracy but test accuarcy is the same for these three models.

![Four Machine Learning](/projects/spacex/machine_learning.png)
<hr>

## Dashboard for launch record
In this part, I build the interactive dashboard for my team to see which sites and payload mass has affected the success rate. In the dashboard, you can see the success rate of the site and the correlation between the site and payload mass to see the success or fail.

![Dashboard for launch record](/projects/spacex/launch_records_dashboard.jpg)

<hr>
