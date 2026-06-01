# house-price-prediction
A machine learning project to predict house prices using regression techniques.
# House Price Prediction

## Overview
This repository contains a machine learning project aimed at predicting house prices based on various structural and locational features[cite: 1]. The project walks through data preprocessing, handling missing values, encoding categorical variables, and evaluating multiple regression models[cite: 1]. 

## Project Structure
* `House_data_project.ipynb`: The main Jupyter Notebook containing the Python code for data processing and model training[cite: 1].
* `HousePricePrediction.csv`: The dataset used to train and test the models[cite: 1].

## Tools and Libraries Used
* **Pandas & NumPy:** For data manipulation and mathematical operations[cite: 1].
* **Seaborn:** For potential data visualization[cite: 1].
* **Scikit-Learn:** For machine learning model building, splitting the dataset, and evaluation[cite: 1].

## Data Preprocessing Steps
The data pipeline includes several essential steps to prepare the dataset for modeling:
* **Handling Missing Values:** Missing numerical values in the features (X) and the target variable (SalePrice) were imputed using their respective statistical means[cite: 1].
* **Feature Selection:** The `Id` and `SalePrice` columns were dropped from the independent variables (X)[cite: 1].
* **Categorical Encoding:** One-hot encoding (`pd.get_dummies`) was applied to convert categorical features into a machine-readable format, specifically targeting the `MSZoning`, `LotConfig`, `BldgType`, and `Exterior1st` columns while dropping the first category to avoid dummy variable trap[cite: 1].
* **Data Splitting:** The dataset was split into an 80% training set and a 20% testing set to properly evaluate model performance[cite: 1].

## Models and Performance
Two different machine learning models were trained and evaluated using the **R-squared (R²)** metric:
1. **Linear Regression:** Achieved an R² Score of **0.355**[cite: 1].
2. **Random Forest Regressor:** Achieved an R² Score of **0.191**[cite: 1].

## How to Run the Project
1. Clone this repository to your local machine.
2. Ensure you have Python installed along with the required libraries (`pandas`, `numpy`, `seaborn`, `scikit-learn`).
3. Open `House_data_project.ipynb` in Jupyter Notebook, Jupyter Lab, or Google Colab.
4. Run the cells sequentially to observe the data processing steps and model outputs.
