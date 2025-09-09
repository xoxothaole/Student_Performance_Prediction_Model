# Student_Performance_Prediction_Model
A machine learning project that predicts student final grades using academic and demographic features to identify students who may need additional support.
Project Overview
This project develops regression models to predict student performance (final grade G3) based on various factors including demographics, family background, and academic history. The goal is to enable early intervention by identifying at-risk students before final exams.

## Dataset

Source: Portuguese secondary school student performance data
Size: 395 students with 35 features
Target: Final grade (G3) on a 0-20 scale
Features: Demographics, family background, school-related attributes, and previous grades

## Key Features

### Two Prediction Scenarios
- With previous grades (G1, G2): Higher accuracy but requires semester data
Without previous grades: Early prediction capability for immediate intervention
###Custom Data Processing
- Custom transformer class for feature engineering
- Automated absence feature combination
- Comprehensive preprocessing pipeline with imputation and scaling

## Model Comparison

- ### Linear Regression
- ### Support Vector Machine (SVM) Regression
- ### Lasso Regression
- ### Cross-validation for robust evaluation

## Technologies Used

- ### Python: Core programming language
- ### scikit-learn: Machine learning algorithms and preprocessing
- ### pandas: Data manipulation and analysis
- ### matplotlib: Data visualization
- ### numpy: Numerical computing

## Machine Learning Pipeline

- ### Data Exploration: Correlation analysis and feature visualization
- ### Feature Engineering: Custom transformer for absence data aggregation
- ### Preprocessing: Separate pipelines for numeric, categorical, and ordinal features
- ### Model Training: Cross-validation comparison of multiple algorithms
- ### Hyperparameter Tuning: GridSearchCV optimization for best models
- ### Evaluation: RMSE and R² metrics on test set

## Results

### Model Performance (RMSE)
With Previous Grades: Linear Regression achieved ~1.86 RMSE
Without Previous Grades: SVM achieved ~4.17 RMSE after hyperparameter tuning

## Key Insights

Previous grades (G1, G2) are the strongest predictors of final performance
Parent education level and study time show moderate correlation with success
Early prediction (without previous grades) is more challenging but achievable

