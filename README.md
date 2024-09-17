# Chicago Traffic Crash Analysis

This project focuses on analyzing traffic crash data from the City of Chicago to identify patterns, trends, and insights related to traffic safety and congestion. The analysis involves integrating multiple datasets, processing large data volumes in Databricks, and visualizing the findings in an interactive dashboard.

## Table of Contents
- [Introduction](#introduction)
- [Dataset Description](#dataset-description)
- [Objectives](#objectives)
- [Process Overview](#process-overview)
- [Analysis and Insights](#analysis-and-insights)
- [Dashboard](#dashboard)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction

The project aims to analyze traffic safety and congestion on Chicago streets by combining multiple datasets, including crash data and people involved in traffic crashes. By using Databricks, Delta Lake, and Azure Blob Storage, the data was processed efficiently to generate actionable insights, ultimately displayed in an interactive dashboard.

## Dataset Description

1. **Traffic Crash Data**:
   - Source: City of Chicago Open Data Portal
   - Records: Over 837K crash records starting from September 2017.
   
2. **People Involved in Crashes Data**:
   - Source: City of Chicago Open Data Portal
   - Records: Over 1 million records detailing the people involved in traffic crashes, including demographics and injury severity.

### Combined Dataset:
- After merging the two datasets on the `CRASH_ID` key, the combined dataset contains 1.85 million rows and 48 columns.

## Objectives

The primary goals of this project are to:
1. Analyze traffic crash patterns and trends.
2. Examine demographic and injury data of people involved in crashes.
3. Generate insights to improve traffic safety measures.
4. Provide an interactive dashboard for visualization and analysis.

## Process Overview

1. **Data Ingestion**:
   - Data was uploaded to Azure Blob Storage and ingested into Databricks for analysis.

2. **Data Processing**:
   - Cleaned, transformed, and merged traffic crash data with people-involved data.
   - Converted the cleaned data into Delta format for efficient querying.

3. **Analysis**:
   - SQL queries were used to extract insights from the merged dataset, including crash counts by various factors such as weather, lighting, and time.

4. **Dashboard Creation**:
   - An interactive dashboard was built to visualize key findings, making insights accessible to policymakers and the public.

## Analysis and Insights

1. **Crashes by Traffic Control Device**:
   - Most crashes occurred in areas with no traffic controls, followed by traffic signal-controlled areas.

2. **Crashes by Weather Conditions**:
   - Clear weather had the highest crash rate, while rain and snow also contributed significantly.

3. **Crashes by Lighting Conditions**:
   - Most crashes occurred in daylight, though nighttime crashes on lighted roads also posed a risk.

4. **Average Crashes per Month**:
   - April and October showed peaks in crash occurrences, while February and June had the lowest crash rates.

5. **Contributory Causes of Crashes**:
   - Failing to yield the right of way and following too closely were common causes.

6. **Crash Locations**:
   - A map visualization of crash hotspots in Chicago was created using latitude and longitude data.

## Dashboard

An interactive dashboard was created to visualize the key findings. You can explore the data through various charts, graphs, and maps.

**Public Dashboard Link**:
[Interactive Dashboard](https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/3190617666491842/2373282331786799/6555990026723924/latest.html)

### Dashboard Features:
- View crash distributions by day of the week, time of day, and weather conditions.
- Explore geographical distribution of crashes across Chicago.
- Analyze injury severity and crash causes.

## Conclusion

This project successfully analyzed traffic crash data to uncover patterns and trends that can inform traffic safety measures in Chicago. The interactive dashboard provides an accessible platform for decision-makers and the public to explore the data and gain insights into road safety.

## References

1. [Big Data Streets - GitHub](https://github.com/ymericson/big-data-streets?tab=readme-ov-file)
2. [Traffic Crashes - City of Chicago Data Portal](https://data.cityofchicago.org/Transportation/Traffic-Crashes-Crashes/85ca-t3if/about_data)
3. [Data Science Basics - YouTube](https://www.youtube.com/watch?v=uZtzARQ2bw8)
