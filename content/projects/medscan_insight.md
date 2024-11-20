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

**MedScan Insight** is a web application designed to predict diseases based on the user's symptoms. It utilizes machine learning to make predictions and is built on the Flask framework. The dataset used for training and testing was obtained from the Kaggle dataset [Predict Disease Symptom](https://www.kaggle.com/datasets/karthikudyawar/disease-symptom-prediction). It was trained and tested using a decision tree algorithm, which is also employed to ask symptom-related questions based on the user's initial input.

The project aims to allow users to diagnose illnesses from home, which is particularly beneficial during times such as the COVID-19 pandemic when visiting clinics may not be feasible. Users can input their symptoms and receive potential diagnoses, empowering them to take charge of their health. They can learn about possible diseases, understand the condition, and know how to care for themselves before making the decision to visit a clinic.

The application is a web-based platform built using the Flask framework. The required libraries for the project can be found in the [requirements.txt]. You can test MedScan Insight at https://medscan-insight.onrender.com/. Below are screenshots of the MedScan Insight web application. Please note that the website is hosted on a free platform, so the performance may be slower than expected. I apologize for any inconvenience.

<hr>

### Home page
This is the home page of the MedScan Insight application. It includes the Symptom Checker button, which will allow users to input their symptoms and predict the disease, as well as information on how the system works.

![home page](/projects/medscan_insight/home_page.png)
<hr>

### About page
This is the About page of the MedScan Insight application. It serves as an introduction to the application and lists all the diseases that can be predicted using the Symptom Checker.

![about page](/projects/medscan_insight/about_page.png)
<hr>

### Explore page

This is the Explore page of the MedScan Insight application. It displays healthcare articles that users can read to help prevent upcoming diseases. The articles are updated by the author (healthcare professional). In the [demo](https://medscan-insight.onrender.com/), there are no articles on the Explore page, as there is no healthcare professional to upload them.
![explore page](/projects/medscan_insight/Explore.png)

This is how the Explore page looks for an author-type user (healthcare professional).

![explore admin page](/projects/medscan_insight/Explore_author.png)
<hr>

### Symptom checker page
This is the Symptom Checker page of MedScan Insight, where the user inputs their initial symptom and the duration of their suffering. Based on the first symptom selected, the system will display corresponding symptoms related to the user's condition.

![symptom page](/projects/medscan_insight/Symptom_asking.png)

This is the second Symptom Checker page, where the user selects "Yes" for symptoms they are experiencing and "No" for those they are not.

![symptom_yes_no page](/projects/medscan_insight/Symptom_yes_no.png)

After all symptoms have been entered, the system will predict the disease, providing the disease name, description, patient condition, and precautions that can be taken for self-care before deciding to visit a clinic.

![result page](/projects/medscan_insight/disease_result.png)

