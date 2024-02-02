# Bike Sharing Analysis & Trend Prediction Project

## Project Description
Traditionally, bike sharing operations relied heavily on the widespread availability of bicycles at designated station hubs. However, the detrimental effects of seasonal variations and weather conditions on bike-share rentals have become more evident. As a result, service operators encounter difficulties in making informed decisions regarding the sustainable enhancement of first and last-mile connectivity to cater to demand, considering weather and seasonal influences. Simply purchasing bicycles en masse for year-round availability has proven ineffective.

This project aims to provide insights into the intelligent management of a bike-sharing service using data components such as timestamp, number of bike rides, weather conditions (temperature, humidity, wind speed, weather code), and period identifiers (weekend, season, holiday). By analyzing this dataset, stakeholders can make informed decisions to optimize bike availability, improve customer experience, and enhance operational efficiency.

## Introduction
Optimizing operational efficiency for "BikesR'Us" to meet demand is a crucial factor in its sustainable enhancement of first and last-mile service connectivity. However, a major concern is the unprecendented shifts in weather conditions and seasonal fluctuations and other related events. These factors have significantly impacted the bike sharing industry, particularly in terms of the need to grow demand for ridership subscription and rentals during off-peak periods. Given the constraints posed by intense market competition, the feasibility of service expansion becomes limited. Hence, there is a pressing need for the implementation of an intelligent management strategy to optimize extant resources.

An essential aspect involves analyzing ride patterns and weather conditions to identify peak demand periods and locations, ensuring optimal bike availability; leveraging insights from data analysis to streamline operations, minimize downtime, and optimize resource allocation. Implementing predictive techniques to proactively address potential issues and enhance system reliability will greatly benefit the expansion plans of "BikesR'Us".

## Dataset

This project utilized a bike sharing dataset that is open to the public and collected from Kaggle's website. The dataset contains 10 attributes or columns : 6 of which are related to the weather and seasonal conditions, 2 are related to time-event and periodic factors and 1 column for the count of rider bookings. The dataset also contains 17414 instances or rows. The label or target variable contains 11 distinct classes.

The dataset includes information such as:
Timestamp
Number of bike rides
Temperature_actual
Temperature_feels
Humidity %
Wind speed
Weather code
Period identifiers – weekend, season, holiday

Exploratory Data Analysis was done on the dataset, leveraging python with imported libraries and tableau for visualization of trends.

## Process
    Data Preparation:
        Downloaded the provided datasets.
        Imported datasets (CSV) and libraries to Python.
        Created pandas dataframe
        Exported dataframe to excel file for Tableau visualisations

    Exploratory Analysis:
        Conducted exploratory analysis on the datasets to grasp the data and its datatypes; executing hypothesis testing
        Checked for any missing values or necessary manipulations to prepare the data for visualization.

    Data Transformations:
        Executed data transformations, using data dictionaries and calculated fields to extract specific insights from the data.

    Visualization:
        Utilized optimal visualizations to provide desired insights to consumers of the report to base their decisions.

## Findings
-As earlier highlighted, 


## Results and Insights
- Months like Dec, Jan and Feb sees less amount of booking. Incentives could be offerd to attract more customers to the bike sharing service. Working days sees more booking so we can provide an offer during weekends or holidays to bring in more bookings.
- More users are booking the bike when humidity is less so we can provide offer to add a refreshment stand at the station hubs for subscribers during humid weather.


## Conclusion
The intelligent management of a bike-sharing service requires a comprehensive understanding of various factors influencing ride demand and system performance. By leveraging historical data from trends analysis, stakeholders can gain actionable insights and make informed decisions to enhance bike availability, customer experience, and operational efficiency, ultimately leading to a more sustainable and successful bike-sharing service.
