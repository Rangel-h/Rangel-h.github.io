---
title: Bike Availability Prediction
excerpt: Intoduccion
publishDate: 'Apr 01 2025'
tags:
  - Predicition
  - Machine learning
  - Regression
seo:
  image:
    src: '/post-1.jpg'
    alt: A person standing at the window
---



## What is Bicing Barcelona?

Bicing Barcelona is a bicycle rental service introduced in 2007 in the city of Barcelona, designed to provide residents and visitors with a sustainable and practical way to get around the city. The system allows users to rent bicycles from various strategic points across Barcelona, making this eco-friendly mode of transportation more accessible.

To use Bicing Barcelona, users must register on the platform and select the type of bicycle they wish to rent. The service offers different rental options tailored to each user's needs, whether for short trips or extended use. Bicing Barcelona contributes to sustainable mobility in the city by reducing traffic congestion and promoting a healthy lifestyle among its users.


## The Challenge
Although Bicing offers many benefits, its effectiveness depends on the number of bikes and docking spaces available at each station. Users may face difficulties if, upon arrival, they find no bikes to use or spaces to return them. This issue is more noticeable during peak hours and in areas with high demand. To ensure a better experience and more efficient service operation, it is essential to accurately predict the availability of bikes and docking spaces.

## The project

In this project, we aim to develop a predictive model to Predict the percentage of free docks at Bicing stations in Barcelona given the historical data of each station, furthermore we leveraged other geographical and temporal data. To achieve this goal we followed the next steps:

Data collection and cleaning

Data analysis

Predicts the availability of free docks

Create a Streamlit app to visualize the predictions

## Data collection and cleaning
We began downloading the datasets from the "Open Data BCN" website:

https://opendata-ajuntament.barcelona.cat/data/ca/dataset/estat-estacions-bicing

The datasets contained data about bike availability from the years 2020, 2021, 2022, 2023 (January-December) and 2024(January- May).

![A person standing at the window](/Dataset1.png)
![A person standing at the window](/Dataset2.png)

Some colummns and rows were droped from the datasets, either because they were empty, they had NAN values, or they didn't provide relevant information for the purpose of this project. Since weather conditions can influence whether a person chooses to use a bicycle as a means of transportation, we added weather information to the datasets.

![A person standing at the window](/Dataset3.png)

## Development of machine learning models

## Predict the availability of free docks

## Create a Streamlit app to visualize the predictions