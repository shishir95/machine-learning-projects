# Global Video Game Sales Prediction

## Overview

This repository contains the final report and associated resources for the **Global Video Game Sales Prediction** project. This project analyzes historical video game sales data to uncover market trends and build predictive models using machine learning techniques. The analysis highlights regional preferences, platform popularity, and genre trends, offering actionable insights for stakeholders in the gaming industry.

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

The video game industry generates billions of dollars annually, making it a cornerstone of the global entertainment sector. This project aims to:

- Predict global video game sales based on historical data.
- Identify trends in genres, platforms, and regional preferences.
- Use machine learning models to optimize sales predictions.

## Dataset Description

- **Source:** [Kaggle - Video Game Sales Dataset](https://www.kaggle.com/)
- **Features:** 16 attributes, including:
  - `Platform`, `Genre`, `Year_of_Release`, `Publisher`
  - Regional sales data (`NA_Sales`, `EU_Sales`, `JP_Sales`, `Other_Sales`)
  - Target variable: `Global_Sales`
- **Size:** 16,719 entries.
- **Challenges:** Missing values in `Critic_Score`, `User_Score`, and `Developer` columns.

## Data Preprocessing

1. **Handling Missing Data:**
   - Imputation for numerical and categorical columns.
   - Dropped columns with excessive missing values.
2. **Outlier Detection:** Applied Interquartile Range (IQR) method to reduce the influence of extreme values.
3. **Standardization:** Scaled sales data for consistent comparison.

## Exploratory Data Analysis (EDA)

- **Platform Analysis:** PlayStation and Xbox dominate global sales.
- **Genre Trends:** Sports and Shooter genres outperform others; Strategy has the lowest sales.
- **Regional Preferences:**
  - North America favors Action and Shooter games.
  - Japan prefers Role-Playing Games (RPGs).
- **Visualizations:** Box plots, scatter plots, and heatmaps reveal patterns and relationships.

## Modeling and Results

Two machine learning models were implemented:

### Random Forest Regressor

- **R²:** 0.875
- **MAE:** 0.0223
- **MSE:** 0.0013

### XGBoost Regressor

- **R²:** 0.8848
- **MAE:** 0.0216
- **MSE:** 0.0012

**Comparison:** XGBoost slightly outperformed Random Forest, demonstrating superior predictive accuracy and generalization.

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

1. [Kaggle - Video Game Sales Dataset](https://www.kaggle.com/datasets/sidtwr/videogames-sales-dataset/data)
2. VanderPlas, J. (2016). _Python Data Science Handbook._
3. Hyndman, R. J., & Athanasopoulos, G. (2018). _Forecasting: Principles and Practice._
4. Breiman, L. (2001). _Random Forests._
5. Chen, T., & Guestrin, C. (2016). _XGBoost: A Scalable Tree Boosting System._

## Repository Structure

- **`dataset/`**: Raw dataset from kaggle.
- **`notebooks/`**: Jupyter notebooks for analysis and modeling.
- **`report/`**: Contains the final report document.
- **`README.md`**: This file.
