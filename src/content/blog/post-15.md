---
title: Bike Availability Prediction for Bicing Barcelona
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

In this project we aim to predict the percentage of free docks given the historical data of each
station of Bicing Barcelona.

# What is Bicing Barcelona?

Bicing Barcelona is a bicycle rental service introduced in 2007 in the city of Barcelona, designed to provide residents and visitors with a sustainable and practical way to get around the city. The system allows users to rent bicycles from various strategic points across Barcelona, making this eco-friendly mode of transportation more accessible.

To use Bicing Barcelona, users must register on the platform and select the type of bicycle they wish to rent. The service offers different rental options tailored to each user's needs, whether for short trips or extended use. Bicing Barcelona contributes to sustainable mobility in the city by reducing traffic congestion and promoting a healthy lifestyle among its users.


# The Challenge
Although Bicing offers many benefits, its effectiveness depends on the number of bikes and docking spaces available at each station. Users may face difficulties if, upon arrival, they find no bikes to use or spaces to return them. This issue is more noticeable during peak hours and in areas with high demand. To ensure a better experience and more efficient service operation, it is essential to accurately predict the availability of bikes and docking spaces.

# The project

In this project, we aim to develop a predictive model to Predict the percentage of free docks at Bicing stations in Barcelona given the historical data of each station, furthermore we leveraged other geographical and temporal data. To achieve this goal we followed the next steps:

Data collection and cleaning

Development of machine learning models

Create a Streamlit app to visualize the predictions

# Data collection and cleaning
We began downloading the datasets from the "Open Data BCN" website:

https://opendata-ajuntament.barcelona.cat/data/ca/dataset/estat-estacions-bicing

The datasets contained data about bike availability from the years 2020, 2021, 2022, 2023 (January-December) and 2024(January- May).

![A person standing at the window](/Dataset1.png)
![A person standing at the window](/Dataset2.png)

Some columns and rows were droped from the datasets, either because they were empty, they had NAN values, or they didn't provide relevant information for the purpose of this project. Since weather conditions can influence whether a person chooses to use a bicycle as a means of transportation, we added weather information to the datasets.

![A person standing at the window](/Dataset3.png)

# Development of machine learning models
To predict the percentage of free docks we used two machine learning models: Light Gradient-Boosting Machine (LGBM) and Long short-term memory (LSTM).

## Light Gradient-Boosting Machine (LightGBM)
LightGBM is an open-source gradient boosting framework developed by Microsoft that is designed for speed and efficiency. It is particularly optimized for large datasets and high-performance machine learning tasks. One of the main characteristics of LGBM is that unlike traditional boosting methods, LightGBM selects the most informative samples for training, which reduces computational cost without sacrificing accuracy.


## Long short-term memory (LSTM)
LSTM is a type of recurrent neural network (RNN) architecture designed to handle sequential data while mitigating the vanishing gradient problem. It is widely used in applications requiring the modeling of long-term dependencies, such as time series forecasting, natural language processing (NLP) and speech recognition.

## Create a Streamlit app to visualize the predictions