# Phishing Website Detection

This project aims to build a machine learning model to detect phishing websites based on various URL and website features. The dataset used in this project is obtained from the UCI Machine Learning Repository.

## Data

The dataset used is the "Phishing Websites Dataset" from the UCI Machine Learning Repository. It contains 11055 instances and 31 features, including the target variable "Result".

## Exploratory Data Analysis

Initial exploratory data analysis revealed:

- No missing values in the dataset.
- The dataset is relatively balanced, with a slightly higher number of instances for the positive class (1) compared to the negative class (-1).
- Most features exhibit weak to moderate correlations with each other and the target variable.

## Model Selection and Evaluation

Two classification models were explored:

1.  **Logistic Regression:**

    - Achieved a mean accuracy of 93% with a standard deviation of 0.01 across 10-fold cross-validation.
    - The classification report showed consistent precision, recall, and F1-scores around 0.93 for both classes.

2.  **Random Forest:**
    - Achieved a mean accuracy of 95% with a standard deviation of 0.00 across 10-fold cross-validation.
    - The classification report indicated excellent performance, with precision, recall, and F1-scores around 0.95-0.96 for both classes.

Based on the evaluation metrics, the Random Forest model demonstrated slightly better performance and consistency compared to Logistic Regression for this dataset.

## Conclusion

The Random Forest model shows promising results for detecting phishing websites based on the provided features. Further improvements could be explored by trying other models, feature engineering, or hyperparameter tuning.

## How to Run the Notebook

1. Clone the repository (if applicable).
2. Open the notebook in Google Colab.
3. Run the cells sequentially.

## Dependencies

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- liac-arff
- requests
- io
