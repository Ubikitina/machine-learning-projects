# Project 1: Airbnb Room Type Classification in Madrid

This project explores the use of machine learning to classify Airbnb listings in Madrid based on their room type (`Entire home/apt`, `Private room`, or `Shared room`). The analysis is conducted on a dataset from **InsideAirbnb**, containing listing data from April 2017.

The primary objective is to implement, compare, and optimize three classification algorithms: **Naive Bayes**, **K-Nearest Neighbors (K-NN)**, and **Decision Trees**.

The notebook follows a structured approach:
1.  **Exploratory Data Analysis (EDA):** Initial investigation of the data reveals no missing values, identifies potential outliers, and highlights an imbalanced class distribution in the target variable (`room_type`).
2.  **Data Preprocessing:** A pipeline is established to handle categorical features using `OneHotEncoder` and to scale numerical features, testing both `MinMaxScaler` and `StandardScaler`.
3.  **Model Experimentation:** Multiple experiments are run to evaluate the models. Initial results show that **Decision Trees** achieve the highest accuracy (~85%), while **Naive Bayes** models perform poorly. K-NN shows moderate performance, which improves significantly with `StandardScaler`.
4.  **Hyperparameter Tuning:** `GridSearchCV` is used to find optimal parameters for K-NN and Decision Trees. The optimized Decision Tree becomes simpler and more interpretable, highlighting **price** as the most influential feature for classification.
5.  **Feature Reduction:** An exploratory step confirms that reducing correlated or redundant features can slightly improve K-NN performance without affecting the simplified Decision Tree's outcome.

Ultimately, the optimized Decision Tree is identified as the most suitable model due to its high accuracy, efficiency, and interpretability.