# AQI-Simple-Reflex-Agent
AQI classification using a Simple Reflex Agent

## 1. Introduction

Air Quality Index (AQI) is used to denote the air quality depending on the level of pollutants. For this project, Simple Reflex Agent is used to classify air quality according to the value of AQI.

This agent uses pre-defined condition action rules. The current AQI is taken as the input for the agent while the output corresponds to the category of air quality.

## 2. Objective

Some of the major objectives of this project include:

- Understanding the working of the Simple Reflex Agent.
- Using the AQI dataset of Indian cities.
- Classifying AQI according to predefined rules.
- Evaluating the classification of the agent.
- Visualizing the distribution of AQI categories.

## 3. Dataset

For this project, the 'city_day.csv' dataset is being used which consists of daily AQI of cities in India.

Important attributes include: 

- City
- Date
- AQI
- AQI_Bucket
- PM2.5
- PM10
- NO
- NO2
- NOx
- NH3
- CO
- SO2
- O3

Records with null AQI values were dropped prior to the implementation of the agent.

## 4. Simple Reflex Agent

The agent categorizes AQI according to the following condition-action pairs:

| AQI Range | Category |
|---|---|
| 0-50 | Good |
| 51-100 | Satisfactory |
| 101-200 | Moderate |
| 201-300 | Poor |
| 301-400 | Very Poor |
| Above 400 | Severe |

The agent bases its action on the current AQI value. No learning takes place.

## 5. Methodology

The project will be done in the following sequence:

1. Loading of the AQI dataset;
2. Data Exploration and investigation of columns;
3. Checking of AQI values for nulls;
4. Dropping the records with null AQI;
5. Definition of AQI condition-action rules;
6. Implementing the Simple Reflex Agent on the dataset;
7. Comparing the result with AQI category in the dataset;
8. Testing of the agent using various AQI values and different cities;
9. Visualization of AQI category distribution.

## 6. Results

The clean data contains 24,850 observations without null AQI.

The Simple Reflex Agent made the following result:

- Total observations: 24,850
- Correct classifications: 24,850
- Incorrect classifications: 0
- Accuracy: 100%

The classification of the agent was in accordance with the AQI categories available in the data set.

## 7. Visualizations 

This project contains visualization of: - AQI categories distribution. - AQI categories distribution in different cities. - Trend of AQI for the selected city. 

## 8. Conclusion 

Simple Reflex Agent was successfully implemented for AQI classification. The agent makes use of rule-based approach and classifies the AQI by mapping the AQI value to a corresponding air quality category. The results indicate that the rule-based approach is capable of classifying the AQI values in the data set if the rules are in line with the data set categories. 

## 9. Files 

- AQI_Simple_Reflex_Agent.ipynb – Google Colab notebook with code, analysis, and visualizations.
- city_day.csv – AQI data set used in the project.
