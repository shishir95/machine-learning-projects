# Develop Machine Learning Model to Predict Annual Return of Stock Profile Based on Historical Data

## Overview

This repository contains resources for analyzing historical stock data to predict annual returns using machine learning techniques. The project examines key financial metrics—including Relative Win Rate (%), Large S/P, Access Return, Systematic Risk, Total Risk, and Excess Return—to determine their relationship with the target variable, Annual Return.

## Table of Contents

- [Project Description](#project-description)
- [Dataset Description](#dataset-description)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis)
- [Modeling and Results](#modeling-and-results)
- [Key Findings](#key-findings)
- [Future Implications](#future-implications)
- [References](#references)

## Project Description

This project focuses on predicting the Annual Return of a stock portfolio by leveraging historical stock market data and machine learning techniques. The analysis explores key financial metrics to uncover patterns and improve prediction accuracy.

- Analyze historical stock performance and market trends.
- Identify the relationship between Relative Win Rate (%), Large S/P, Access Return, Systematic Risk, Total Risk, and Excess Return with Annual Return.
- Build and evaluate predictive models using machine learning techniques using Linear Regression.

## Dataset Description

- **Source:** [Kaggle - Video Game Sales Dataset](https://archive.ics.uci.edu/dataset/390/stock+portfolio+performance)
- **Features:** 10 attributes, including:
  - `Period`, `ID`, `Large B/P`, `Large ROE`, `Large S/P`, `Large Return Rate in the last quarter`, `Large Market Value`, `Small systematic Risk`, `Excess Return`
  - Target variable: `Annual Return`
- **Size:** 63 entries.

## Data Preprocessing

1. **Handling Missing Data:**
   - Imputation for numerical and categorical columns.
   - Dropped columns with excessive missing values.
2. **Outlier Detection:** Applied Interquartile Range (IQR) method to reduce the influence of extreme values.

## Exploratory Data Analysis (EDA)

- **Excess Return Analysis:** There is a strong positive correlation between Excess Return (%) and Annual Return.
- **Systematic Risk:** There is a positive correlation between Systematic Risk and Annual Return, but it is less structured compared to the Excess Return vs. Annual Return plot.
- **Visualizations:** Box plots, scatter plots, and heatmaps reveal patterns and relationships.

## Modeling and Results

Linear Regression model was implemented:

### Linear Regression

- **R²:** 1.0
- **MAE:** 1.67
- **MSE:** 3.801

## Key Findings

1. **Regional Variations:**
   - North America prefers Action/Shooter genres.
   - Japan favors RPGs.
2. **Platform Trends:**
   - PlayStation and Xbox lead global sales.
3. **Genre Influence:**
   - Sports and Shooter genres contribute significantly to global sales.

## Future Implications

- **Game Development:** Focus on region-specific preferences and popular genres.
- **Marketing Strategies:** Leverage insights for targeted advertising and optimized release timings.
- **Distribution:** Emphasize platforms with higher sales potential.

## References

1. [Machine Learning Repository - Stock Portfolio Performance](https://www.kaggle.com/datasets/sidtwr/videogames-sales-dataset/data)

## Repository Structure

- **`dataset/`**: Raw dataset from Machine Learning Repository.
- **`notebooks/`**: Jupyter notebooks for analysis and modeling.
- **`README.md`**: This file.
