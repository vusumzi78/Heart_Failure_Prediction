# Heart Failure Prediction

## Overview

The Heart Failure Prediction project aims to develop a machine learning model to predict the likelihood of heart failure events based on patient data. The goal is to assist healthcare professionals in identifying high-risk patients for timely intervention and improved outcomes.

## Dataset

The dataset used in this project includes the following columns:
- **age**: Age of the patient
- **anaemia**: Whether the patient has anemia
- **creatinine_phosphokinase**: Level of the CPK enzyme in the blood
- **diabetes**: Whether the patient has diabetes
- **ejection_fraction**: Percentage of blood leaving the heart at each contraction
- **high_blood_pressure**: Whether the patient has high blood pressure
- **platelets**: Platelet count in the blood
- **serum_creatinine**: Level of serum creatinine in the blood
- **serum_sodium**: Level of serum sodium in the blood
- **sex**: Gender of the patient
- **smoking**: Whether the patient is a smoker
- **time**: Follow-up period in days
- **DEATH_EVENT**: Whether the patient experienced a heart failure event

## Project Objective

The project involves:
1. Exploring and preprocessing the dataset.
2. Building and evaluating various machine learning models to predict heart failure events.
3. Identifying the most important features influencing the prediction.
4. Providing recommendations for improving model performance.

## Model Performance

- The Logistic Regression model initially performed better than the Random Forest and SVM models.
- After hyperparameter tuning, the Random Forest model achieved a cross-validated score of approximately 90%, but the test accuracy was around 73%. This indicates potential overfitting or variance in the test set.

## Feature Importance

- Random Forest models can provide insights into feature importance, helping to understand which features are most influential in predicting the target variable.

## Recommendations

- Consider further feature engineering, such as creating interaction terms or using domain knowledge to create new features.
- Explore additional models or ensemble methods to improve performance.
- Investigate the data distribution and potential class imbalance, as the recall for the positive class (`DEATH_EVENT = 1`) is lower, indicating that the model may not be capturing this class as effectively.
