# Health & Walkability Analysis

A data analytics and machine learning project exploring how public health patterns relate to walkability across U.S. counties.

## Overview

This project combines public health data from the CDC with the EPA National Walkability Index to investigate whether community health indicators can help explain and predict differences in walkability.

The analysis examines 29+ health measures, including obesity, diabetes, asthma, smoking, and depression, alongside walkability data aggregated across 3,066 U.S. counties.

## Data

- **CDC Local Data for Better Health: ~240,000 county-measure observations covering 29+ health indicators
- **EPA National Walkability Index: ~220,000 Census block groups with walkability scores and built-environment data

Because the two datasets use different geographic units, EPA block-group data was aggregated to the county level before being combined with the CDC health data.

## Methods

- Cleaned, reshaped, and merged CDC and EPA datasets
- Conducted exploratory and correlation analyses of health and walkability patterns
- Used K-means clustering to group counties based on health profiles
 -Trained and compared Ridge Regression, Random Forest, and XGBoost models
- Used cross-validation and hyperparameter tuning to evaluate model performance
- Compared feature importance across modeling approaches
- Used grouped train/test splitting to prevent county-level data leakage

## Results

Healthier county clusters generally had higher average walkability scores than less healthy clusters.

Coronary heart disease, obesity, cigarette smoking, and arthritis showed some of the strongest negative correlations with walkability.

Ridge Regression, Random Forest, and XGBoost produced similar results, with R² values around 0.42, suggesting that increasing model complexity provided limited improvement in predicting walkability from the available health data.

## Technologies

Python · Pandas · NumPy · scikit-learn · XGBoost · Matplotlib

## Contributors

Emma Luque · Anjana Begur · Kelli Eng