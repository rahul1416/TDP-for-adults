Overleaf link: https://www.overleaf.com/project/638b720d14e025765b4c8fab/invite/token/5ad638327d65ff00cd1122953c370ec0323c8a4efd4b6f87?project_name=T2_Project_Report_DS201&user_first_name=dr.nitin.khanna
# Temporal Dietary Patterns and Diet Quality Analysis

This repository contains code and documentation for a research project on the relation between Temporal Dietary Patterns (TDP) and Diet Quality among clusters of US adults with similar eating habits. The project utilizes data from the National Health and Nutrition Examination Survey (NHANES) datasets spanning from 2007 to 2018.

## Introduction

The project investigates the relationship between temporal dietary patterns and diet quality among US non-pregnant adults aged 20-65 years. Temporal dietary patterns consider the timing of food consumption in addition to other dietary characteristics. Clusters were derived from cleaned NHANES data using various clustering algorithms, and diet quality was assessed using the Healthy Eating Index (HEI) - 2015.

## Materials & Methods

The NHANES dataset, sourced from the US government, was cleaned by removing null values, dropping unnecessary columns, and combining datasets. Clustering was performed using K-means with Euclidean distance as the initial metric, resulting in the identification of 3 clusters. Diet quality analysis was based on the HEI-2015 index, calculated using multiple linear regression.

## Results

Initial attempts using K-means clustering with Euclidean distance revealed limitations, particularly in comparing dietary patterns associated with time stamps. Kernel K-means clustering with Dynamic Time Warping (DTW) was proposed as an alternative but proved computationally intensive, exceeding local resources. K-means clustering was retained, but clusters were formed based on energy consumption rather than eating time, hindering the intended analysis.

![Results](/figures/energy_intake_vs_time.jpeg)
*Figure 1: Clusters formed by KMeans Clustering*

## Discussion

Clusters derived using K-means clustering did not effectively capture temporal dietary patterns, complicating the intended analysis of their relation to diet quality. The discrepancy between actual dietary patterns and those inferred from energy consumption underscores the need for alternative clustering methods sensitive to time-series data.

## Conclusions

Despite limitations encountered, the project highlights the importance of appropriate clustering techniques in analyzing temporal dietary patterns. Future work could explore more computationally intensive methods such as Kernel K-means with DTW to better capture the nuances of dietary behavior.

## Acknowledgements

We would like to express our gratitude to Dr. Nitin Khanna for initiating this project and providing guidance throughout its execution.

For any inquiries, please contact [Project Lead](mailto:projectlead@example.com).
