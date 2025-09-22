# Project 3: SVM for Airbnb Listing Classification and Price Prediction

This project applies **Support Vector Machines (SVM)** to perform both classification and regression tasks on an Airbnb dataset for Madrid. The study is structured into a series of experiments to build, evaluate, and optimize SVM models for two distinct goals: classifying the type of room and predicting its price.

### Key Experiments and Findings:

1.  **Room Type Classification (`LinearSVC` vs. `SVC`):**
    * Initial models were trained to classify listings into `Entire home/apt`, `Private room`, or `Shared room`.
    * Both `LinearSVC` and `SVC` performed well on the majority classes but failed to correctly classify the minority `Shared room` class due to significant class imbalance.
    * Hyperparameter tuning with `GridSearchCV` for the `SVC` model (adjusting `C` and `gamma`) improved overall accuracy but did not resolve the core issue of predicting the minority class.

2.  **Price Prediction (`LinearSVR` vs. `SVR`):**
    * Initial regression models were built to predict the `price` of listings. These models performed poorly, yielding very low R² scores, indicating they could not explain the variance in price.
    * A **modified experiment** was conducted after removing price outliers (listings > €2000). This single change led to a significant improvement in all regression metrics (MSE, MAE, and R²), demonstrating the strong negative impact of outliers.
    * Subsequent hyperparameter tuning on the cleaned data, particularly for the `SVR` model, further improved performance. The final tuned `SVR` model achieved the best results, though the overall predictive power remained modest, highlighting the complexity of price prediction with this feature set.

In summary, this project demonstrates the application of different SVM models and underscores the critical importance of data preprocessing—specifically addressing class imbalance for classification and removing outliers for regression—to build effective machine learning models.