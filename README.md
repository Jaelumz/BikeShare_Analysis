# Bike Sharing Analysis & Trend Prediction Project

## Project Description
Traditionally, bike sharing operations relied heavily on the widespread availability of bicycles at designated station hubs. However, the detrimental effects of seasonal variations and weather conditions on bike-share rentals have become more evident. As a result, service operators encounter difficulties in making informed decisions regarding the sustainable enhancement of first and last-mile connectivity to cater to demand, considering weather and seasonal influences. Simply purchasing bicycles en masse for year-round availability has proven ineffective.

This project aims to provide insights into the intelligent management of a bike-sharing service using data components such as timestamp, number of bike rides, weather conditions (temperature, humidity, wind speed, weather code), and period identifiers (weekend, season, holiday). By analyzing this dataset, stakeholders can make informed decisions to optimize bike availability, improve customer experience, and enhance operational efficiency.

## Introduction
In the context of optimizing operational efficiency for "BikesR'Us" to meet demand, a critical determinant is its sustainable enhancement of first and last-mile service connectivity. However, a contemporary concern of paramount significan is the unprecendented changes in weather conditions and seasonal variations as well as other events. This has exerted a notable impact on the bike sharing industry, particularly in terms of growing demand for ridership subscription during off-peak periods. Given the constraints posed by huge influx of market competition, the feasibility of service expansion is constrained. Accordingly, there exists a compelling need for implementation of intelligent management strategy to optimize extant resources.

Analyzing ride patterns and weather conditions to determine peak demand periods and locations is essential to ensure optimal bike availability; utilizing insights from data analysis to streamline operations, minimize downtime, and optimize resource allocation. Implementing predictive techniques to proactively address potential issues and enhance system reliability will be beneficial to the expansion plans of "BikesR'Us".

## Dataset

This project utilized an agricultural dataset that is open to the public and collected from Kaggle's website. The dataset contains 8 attributes or columns : 4 of which are related to the soil composition, 3 columns are related to climatic conditions and 1 columns for the label or target variable. The dataset also contains 2200 instances or rows. The label or target variable contains 22 distinct classes.

Libraries used for analysis
Python is primarily used for the project and the following variables were used in importing, exploring, visualizing and analysing the dataset.
-NumPy
-Pandas
-Seaborn
-Matplotlib
-Sklearn
-Ipywidgets
-Tableau

## Exploratory Data Analysis

    -As earlier highlighted, this dataset contains 17414 rows and 10 columns. The column names in this dataset is as follows: Nitrogen (N), Phosphorus (P), Potassium (K), Ph, Temperature, Humidity and Rainfall.
-7 of the 8 columns are numerical columns except for the target or label column.
    -The data set does not contain any missing values.
    -Using box plots to visualize the dataset, it can be observed that there seems to be lots of data points that at first glance, looks like "outliers" for all of the factors except nitrogen. However, upon further examination, this is due to the different optimal soil conditions for the different plants.
    -Each unique crop or distinct class of the target variable has 100 rows of data, representing 4.5% of the entire data set.
    -The summary statistics for the dataset:
        --Average Ratio of Nitrogen in the Soil: 50.55
        --Average Ratio of Phosphorus in the Soil: 53.36
        --Average Ratio of Potassium in the Soil: 48.15
        --Average PH Value of the Soil: 6.47
        --Average Temperature in Celsius: 25.62
        --Average Relative Humidity in %: 71.48
        --Average Rainfall in mm: 103.46
    -We also discover the following facts:
        --Cotton requires a very high ratio of nitrogen content in the soil.
        --Grapes and Apples requires a very high ratio of phosphorus and potassium content in the soil.
        --Most crops require a ph level between 6 and 7
        --Most crops require temperatures above 20C with Papaya and Grapes needing the highest temperatures at above 30C.
        --Chickpea and Kidneabeans require the least humidity, around 20
        --Muskmelon requires the lowest rainfall at 25mm while rice has the highest at almost 250mm.

-Below visualizations were created to provide insights to report consumers:
    -- Total Number of Bike Rides
    -- Moving Average Chart (main visual) with additional visuals in tooltip
    -- Temperature vs Wind Speed Heat Map
    -- Total bike rides split by weather and hour

User-defined parameters are applied to Moving Average Chart to get insights on historical trends over time

## Findings

    -Using KMeans and the Elbow method, I found the optimal number of clusters in the dataset to be 4.
    -Therefore, this is the classification of the crops based on each cluster
        --Cluster 1
            ---Grapes
            ---Apple
        --Cluster 2
            ---Maize
            ---Chickpea
            ---Kidneybeans
            ---Pigeonpeas
            ---Mothbeans
            ---Mungbean
            ---Blackgram
            ---Lentil
            ---Pomegranate
            ---Mango
            ---Orange
            ---Papaya
            ---Coconut
        --Cluster 3
            ---Maize
            ---Banana
            ---Watermelon
            ---Muskmelon
            ---Papaya
            ---Cotton
            ---Coffee
        --Cluster 4
            ---Rice
            ---Pigeonpeas
            ---Papaya
            ---Coconut
            ---Jute
            ---Coffee
    -Logistic regression was used in the building of the model because it works better in the case of likelihood and multiple labels.

## Model Accuracy and Results


## Conclusion
