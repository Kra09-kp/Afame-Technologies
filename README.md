# Sales Price Prediction Project

## Table of Contents

- [Project Description](#project-description)
- [Technologies](#technologies)
- [Data Exploration](#data-exploration)
- [Visualizations](#visualizations)
- [Data Preprocessing](#data-preprocessing)
- [Model Building](#model-building)
- [Model Evaluation](#model-evaluation)
- [Cross-Validation](#cross-validation)
- [Conclusion](#conclusion)


## Project Description

This project aims to predict sales prices based on a small dataset containing only 200 rows and 4 columns. The dataset includes the following columns:

1. `TV`: advertising budget spent on TV
2. `Radio`: advertising budget spent on radio
3. `Newspaper`: advertising budget spent on newspaper
4. `Sales`: total sales generated

The goal is to build machine learning models to predict sales prices based on the advertising budgets spent on TV, radio, and newspaper. The models will be evaluated using cross-validation to ensure their generalization to unseen data.

## Technologies

This project is created using Python in Collab Notebook. The following libraries are used:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn


## Data Exploration

The dataset contains 200 rows and 4 columns, with no missing values.Due to the limited size of the dataset, extensive exploratory data analysis (EDA) was not required. Instead, the focus was on visualizing the data, building predictive models, and performing cross-validation. Visualizations such as correlation matrices, pair plots, and total budget versus sales were created to understand the relationships between variables.

## Visualizations

1. **Correlation Matrix**: A correlation matrix was generated to identify relationships between variables, helping in feature selection for modeling.

2. **Pair Plot**: A pair plot was created to visualize the relationships between pairs of variables in the dataset, providing insights into potential patterns and trends.

3. **Total Budget versus Sales**: A visualization was created to explore the relationship between the total budget (sum of three columns) and sales, helping to understand the impact of budget on sales.

## Data Preprocessing

The dataset was split into features (X) and target (y) variables for model training. The features were scaled using StandardScaler to ensure that all variables were on the same scale.


## Model Building

Several machine learning models were trained and evaluated for sales price prediction:

- Linear Regression (LR) 
- Random Forest (RF)
- k-Nearest Neighbors (KNN)
- Decision Tree (DT)
- Gradient Boosting (GB)
- Extreme Gradient Boosting (XGBoost)

These models were chosen based on their suitability for regression tasks and their ability to handle small datasets. As the dataset is small, I did not use deep learning models, as they typically require larger datasets to perform well.

## Model Evaluation

The models were evaluated based on the following metrics:

1. **Mean Squared Error (MSE)**: The mean squared error was used to measure the average squared difference between the predicted and actual sales prices.

2. **R2 Score**: The R2 score was used to evaluate the proportion of variance in the target variable that was captured by the model.

The models were compared based on these metrics to identify the best performer for sales price prediction.


## Cross-Validation

Cross-validation was performed to evaluate the models' performance and ensure their generalization to unseen data. This technique helps to validate the robustness of the models and identify any potential overfitting issues.

## Conclusion

After thorough evaluation, it was found that Gradient Boosting and Random Forest were the top performers for sales price prediction. Despite the small dataset size, these models demonstrated robust performance and were chosen for deployment in production. Further experimentation with larger datasets and additional features could lead to improved model performance.
