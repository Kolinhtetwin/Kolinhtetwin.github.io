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

This is the final capstone project where I have to utilize the data analysis tools that I learned from IBM Data Science. The things I have to do in this project are:
- Data collection with API and web scraping
- Data wrangling
- Exploratory data analysis using SQL
- EDA data visualization using Python Pandas and Matplotlib
- Launch sites analysis with Folium-Interactive Visual Analytics and Plotly Dash
- Machine learning landing prediction

## Data collection with API and web scraping 
First, I request the necessary data from the SpaceX REST API.

![Request Data from SpaceX Rest API](/projects/spacex/request_api.png)

Then, I use the `json_normalize` method to convert the JSON result into a Pandas DataFrame.

![Normalize Data into DataFrame](/projects/spacex/normalize_json.png)

Then, I analyze the features and labels of the dataset. Finally, I filter the dataset to include only Falcon 9 launches.

![Filter Data](/projects/spacex/Filter_data.png)
<hr>

## Exploratory Data Analysis using Pandas

In this part, I perform exploratory data analysis using the Pandas library. First, I try to see how Flight Number (which indicates continuous launch attempts) and Payload variables affect the launch outcome. For payload mass exceeding 10,000 kg, the launch attempts are more successful compared to those with lower payload masses. Starting from the 79th attempt, all launches have been successful regardless of the payload mass.

![Payload x FlightNumber](/projects/spacex/payload_flightnumber.png)

After that, I try to find the patterns between the Flight Number and Launch Site based on the success rate for landing. Based on the scatterplot, CCAFS SLC 40 and KSC LC 39A have a 100 percent success rate for flight numbers above 80. Although KSC LC 39A has no data below 20 Flight Numbers, its success rate for between 40 and 65 Flight Numbers is also 100 percent. CCAFS SLC 40 has launched more flights than the other two launch sites.

![FlightNumber x LaunchSite](/projects/spacex/flightnumber_site.png)

Based on the relationship between payload mass and launch site, CCAFS launch site has the most flights. VAFB SLC 4E does not launch flights that weigh more than 10,000 kg. KSC LC 39A site has a 100% success rate for launching flights that weigh between 2,000 and 5,000 kg.

![Payload x LaunchSite](/projects/spacex/payload_launchsite.png)

Additionally, I analyze the average success rate over the years. From 2013 to 2020, the success rate exhibited a consistent upward trend. Notably, the year 2019 recorded the highest success rate within this period, reaching an impressive 90%.

![Average Success Rate](/projects/spacex/average_success_rate.png)

**Based on the exploratory data analysis, the key insights are**
- For payload mass exceeding 10,000 kg, the launch attempts are more successful compared to those with lower payload masses.
- If you want to try launching payloads weighing between 2,000 and 5,000 kg, KSC LC 39A site has been the best launch site.
- CCAFS SLC 40 has succeeded in every launch attempt for payload mass greater than 10,000 kg.
- According to the analysis of the average success rate over the years, the success rate has increased dramatically from 2015, reaching an impressive 90% at 2019.

<hr>

## Machine Learning models

With exploratory data analysis, I split the data into training and testing data. I use GridSearchCV to find the best parameters from the parameters I provided and use four different machine learning models to find which one is the best at predicting successful landings.

According to the graph, the Decision Tree performs well on training accuracy, but the test accuracy is pretty low compared to other machine learning models. Logistic Regression, Support Vector Machine, and K-Nearest Neighbors perform nearly the same on validation accuracy, but test accuracy is the same for these three models.

![Four Machine Learning](/projects/spacex/machine_learning.png)
<hr>

## Dashboard for Launch Records
In this part, I build an interactive dashboard for my team to see which sites and payload masses have affected the success rate. In the dashboard, you can see the success rate of the site and the correlation between the site and payload mass to determine success or failure.

![Dashboard for launch record](/projects/spacex/launch_records_dashboard.jpg)

<hr>
