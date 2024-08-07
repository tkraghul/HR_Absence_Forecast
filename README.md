## HR Absenteeism Prediction Project
# Overview

This project aims to predict the number of hours an employee might be absent from work using various regression models. The dataset used contains information on 8,330 employees, including demographic details, job roles, and absenteeism records.
Objective

The primary objective of this project was to compare different machine learning models to determine the most accurate method for predicting absenteeism hours.
Dataset

    Source: [Include the source of your dataset if publicly available]
    Size: 8,330 entries
    Features: Age, Gender, Job Title, Department, Length of Service, etc.
    Target Variable: Absent Hours

Methodology

    Data Cleaning:
        Dropped irrelevant columns like Employee Number, Surname, and Given Name.
        Handled missing values and removed outliers from the numeric features.

    Feature Engineering:
        Encoded categorical variables using One-Hot Encoding.
        Applied dimensionality reduction using Principal Component Analysis (PCA).

    Modeling:
        Implemented Multiple Linear Regression (MLR) and Random Forest Regressor (RFR).
        Compared the performance of the models with and without PCA.

Results

After evaluating the models, we found that the Random Forest Regressor (RFR) performed the best, achieving an R-Squared of 0.7347 and a Root Mean Squared Error (RMSE) of 24.71. The use of PCA slightly reduced the model's performance but provided better interpretability by reducing the feature set.
Model	Mean Squared Error (MSE)	Root Mean Squared Error (RMSE)	R-Squared
MLR	3.59e+20	1.89e+10	-1.56e+17
RFR	610.57	24.71	0.7347
MLR with PCA	612.99	24.76	0.7336
RFR with PCA	622.89	24.96	0.7293
Visualizations

    Boxplots: Displayed the distribution of key numeric features to identify outliers.
    Explained Variance Plot: Demonstrated the cumulative variance explained by the PCA components.
    Feature Importance: Highlighted the top 20 most important features in the Random Forest model.


Conclusion

The Random Forest Regressor was the most effective model for predicting absenteeism in this dataset. Although PCA reduced the model's performance slightly, it allowed for a more manageable and interpretable model by reducing the dimensionality of the dataset.
Tools & Libraries

    Python
    Pandas
    Scikit-learn
    Seaborn
    Matplotlib

Future Work

    Explore additional models such as Gradient Boosting or XGBoost.
    Fine-tune hyperparameters of the Random Forest model for further improvement.
    Investigate potential external factors influencing absenteeism that are not included in this dataset.

Author

[Your Name] - Your LinkedIn Profile
