# Salary Prediction of Data Professions

![Salary Prediction Model](https://repository-images.githubusercontent.com/293898841/c91e7100-5e42-11eb-9820-2f68d80ed516)

This project aims to build a machine learning model that predicts the salary of data professionals based on various features such as personal information, job details, and performance metrics. The model uses a Random Forest Regressor, and the application is deployed using Gradio for easy user interaction.

## Dataset Overview

The dataset contains the following columns:

- `FIRST NAME`: First name of the employee
- `LAST NAME`: Last name of the employee
- `SEX`: Gender of the employee
- `DOJ`: Date of joining the company
- `CURRENT DATE`: The current date of the data
- `DESIGNATION`: Job role/designation of the employee
- `AGE`: Age of the employee
- `SALARY`: Target variable, the salary of the employee
- `UNIT`: Business unit or department
- `LEAVES USED`: Number of leaves used by the employee
- `LEAVES REMAINING`: Number of leaves remaining for the employee
- `RATINGS`: Performance ratings of the employee
- `PAST EXP`: Past work experience of the employee (in years)

## Project Pipeline

1. **Exploratory Data Analysis (EDA)**: Understand the dataset through visualization and summary statistics.
2. **Feature Engineering**: Create new features or transform existing ones to improve model performance.
3. **Data Preprocessing**: Handle missing values, encode categorical variables, and scale/normalize features as needed.
4. **Model Development**: Train various regression models to predict salaries. Experiment with different algorithms such as linear regression, decision trees, random forests, and gradient boosting.
5. **Model Evaluation**: Assess model performance using metrics like Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R²) score.
6. **ML Pipelines and Model Deployment**: Create ML pipelines to streamline the process from data preprocessing to model training. Deploy the model using Gradio.
7. **Recommendations**: Provide actionable insights based on the model's predictions and findings.

## Preprocessing and Feature Engineering

1. **Date Features**: Extract month and year from the date of joining (`DOJ`).
2. **Grouping**: Group `AGE` and `PAST EXP` into categories.
3. **Leave Calculations**: Calculate the percentage of leaves used.
4. **Tenure Calculation**: Calculate the tenure of employees from the date of joining to the current date.
5. **Encoding**: Encode categorical features using one-hot encoding.

## Model Training

The project uses a Random Forest Regressor as the primary model. The trained model is saved as a pickle file (`best_rf_regressor.pkl`) for deployment.

## Deployment with Gradio

The application uses Gradio to provide a user-friendly interface for salary prediction.

## Contributors

Riyad Ahmadov

## Conclusion

This project demonstrates the end-to-end process of building a salary prediction model, from data preprocessing and feature engineering to model training and deployment using Gradio. The final application allows users to input various details and receive a predicted salary, providing valuable insights into the factors influencing salary in data professions.


