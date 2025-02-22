# ML-assignment-2
Housing prices 
# Housing Price Prediction using Regression Models

## Overview
This project aims to predict **housing prices** based on various features using multiple **regression models**. The dataset includes information such as **median income, total rooms, ocean proximity, and house age**, which are used as input features for the predictive models.

## Dataset Description
- **File Name:** `1553768847-housing.csv`
- **Number of Rows:** 20,640
- **Number of Features:** 10
- **Target Variable:** `median_house_value`
- **Key Features:**
  - `longitude` and `latitude` - Geographical location of the house.
  - `housing_median_age` - Age of the house.
  - `total_rooms`, `total_bedrooms` - Total number of rooms and bedrooms.
  - `population`, `households` - Population and number of households in the area.
  - `median_income` - Median income of residents.
  - `ocean_proximity` - Categorical feature representing house location relative to the ocean.

## Data Preprocessing
- **Handling Missing Values:** `total_bedrooms` column had missing values, which were filled using the **median**.
- **Encoding Categorical Features:** One-Hot Encoding was applied to the `ocean_proximity` column.
- **Feature Scaling:** Standardization (z-score normalization) was applied to numerical features to improve model performance.

## Exploratory Data Analysis (EDA)
- **Correlation Heatmap:** Analyzed relationships between numerical features.
- **Histograms:** Visualized the distribution of numerical variables.
- **Scatter Plot (Median Income vs. House Value):** Examined key trends.
- **Box Plots:** Identified outliers in numeric features.

## Regression Models Used
We trained and evaluated multiple regression models to predict housing prices:

### 1️⃣ **Linear Regression**
- A simple baseline model.
- Performance:
  - RMSE: ~X
  - R² Score: ~X

### 2️⃣ **Ridge Regression**
- Regularized version of Linear Regression to handle multicollinearity.
- Performance:
  - RMSE: ~X
  - R² Score: ~X

### 3️⃣ **Random Forest Regressor**
- An ensemble learning method using multiple decision trees.
- Performance:
  - RMSE: **50,330**
  - R² Score: **0.807**

## Model Evaluation
We used **cross-validation** to validate our models and prevent overfitting. The models were compared based on **Root Mean Square Error (RMSE)** and **R² Score**.

## Installation & Requirements
To run this project, install the following dependencies:
```sh
pip install numpy pandas scikit-learn  matplotlib seaborn
```

## Running the Project
1. Load the dataset in Python using pandas.
2. Perform data preprocessing (handling missing values, encoding, feature scaling).
3. Conduct EDA (visualizations, statistical analysis).
4. Train and evaluate multiple regression models.
5. Compare performance metrics to select the best model.

## Conclusion
- **Random Forest Regression** provided the best balance of accuracy and performance.
- **Linear Regression and Ridge Regression** served as simple benchmarks but had lower accuracy.

This project demonstrates how **multiple regression techniques** can be applied to **predict housing prices** accurately. Future work could include **hyperparameter tuning, feature selection, and deploying the model as an API**.


