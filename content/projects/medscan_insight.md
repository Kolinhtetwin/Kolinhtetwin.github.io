---
title: "MedScan Insight"
date: 2023-11-20
draft: false
links:
  - icon: fab fa-github
    url: https://github.com/Kolinhtetwin/MedScan-Insight
author: "Lin Htet Win"
tags:
  - Python
  - Pandas
  - HTML
  - CSS
  - SQL
  - Flask
badges:
 - Python
 - Pandas
 - HTML
 - CSS
 - SQL
 - Flask
image: /projects/medscan_insight/medscan_logo.png
description: "A web application designed to predict the disease with symptoms."
toc: 
---
### About application
This project represents the culmination of my academic journey as a Bachelor's degree student, serving as the final year project that synthesizes and applies the knowledge and skills acquired throughout my undergraduate studies.

MedScan Insight is a web application designed to predict the diseases with the user's symptoms. It utilized machine learning to predict the diseases and build upon the Flask framework. The dataset to train and test was obtained from the Kaggle dataset [Predict Disease Symptom](https://www.kaggle.com/datasets/karthikudyawar/disease-symptom-prediction). It was trained and predicted using decision tree algorithm and also utilized the decision tree to ask the question of the symptoms based on the user's first input symptom.

The project aims to allow users to diagnose illnesses from home, which is particularly beneficial during times such as the COVID-19 pandemic when visiting clinics may not be feasible. Users can input their symptoms and receive potential diagnoses, empowering them to take charge of their health. Users can know about what kind of diseases may have, the condition and how to take care before making the decision to go to clinic.

The application is a web-based platform built using the Flask framework. The required libraries for the project can be found in the [requirements.txt]. You can test MedScan Insight at https://medscan-insight.onrender.com/. Below screenshots are the sample image of MedScan Insight web application. 

<hr>

### Home page
This is the home page of MedScan Insight application. It includes the button of symptom checker that will take your symptoms to predict the disease and how its works.

![home page](/projects/medscan_insight/home_page.png)
<hr>

### About page
This is the about page of MedScan Insight application. It serves as the introduction of MedScan Insight application and it includes all the diseases that can be predicted with symptom checker.

![about page](/projects/medscan_insight/about_page.png)
<hr>

### Explore page
This is the explore page of MedScan Insight application. It will show the healthcare article that you can read and prevent the upcoming diseases. The articles will be updated by the author (healthcare-profession). In the [demo](https://medscan-insight.onrender.com/), there is no articles in the explore page as there is no healthcare professional to upload the articles.

![explore page](/projects/medscan_insight/Explore.png)

This is how the explore page looks like for author-type user (healthcare-professional).

![explore admin page](/projects/medscan_insight/Explore_author.png)
<hr>

### Symptom checker page
This is the symptom checker page of MedScan Insigth where the user has to input their initial symptom and day-suffering. With the first symptom choose, the system will give the corresponding symptoms that is related to your symptom.

![symptom page](/projects/medscan_insight/Symptom_asking.png)

This is the second symptom checker page where the user has to press "Yes" for the symptom they are suffering and "No" for the symptoms they are not suffering.

![symptom_yes_no page](/projects/medscan_insight/Symptom_yes_no.png)

After finish asking all the symptoms, the system will predict the disease name, and it will also include disease description, condition of the patient and the precaution which you can do to take care.

![result page](/projects/medscan_insight/disease_result.png)

