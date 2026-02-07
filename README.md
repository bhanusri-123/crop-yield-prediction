## Crop Yield Prediction using Machine Learning

## Problem Understanding
The project looks for developing a machine-learning model that should predict the yields depending on actual data with respect to agriculture. Crop yield prediction serves as a critical agricultural challenge which helps farmers decide when to grow crops and how to distribute their resources while safeguarding food supplies.

The dataset used includes historical crop data from various states which spans different seasons and years and incorporates environmental data and agricultural input data like rainfall and fertilizer and pesticide usage and cultivated area. Effective preprocessing and proper model selection become necessary because real-world agricultural data contains multiple interacting elements which exhibit natural variations.

The project aims to predict crop yield through regression-based machine learning methods which analyze multiple factors. The project develops a dependable model which enables users to understand its predictions through a complete machine learning process that includes data preparation and model development and validation and result assessment. The project main objective lies in establishing model reasoning abilities which enable practical use cases instead of achieving accuracy results.

## Dataset
- **Type:** Public agricultural dataset
- **Domain:** Crop Yield Prediction
- **Target Variable:** Yield

## Features Used
- Crop
- Crop_Year
- Season
- State
- Area
- Annual_Rainfall
- Fertilizer
- Pesticide

## Model Pipeline Description
1. Data Preprocessing
   The dataset needed cleaning because it contained both missing data and duplicated records. The Production column was dropped to avoid data leakage because yield depends on production and area. One-Hot Encoding was used to encode categorical features Crop Season and State while StandardScaler was applied to scale the numerical features. The data was divided into training and testing sets using an 80/20 ratio.
2. Model Selection & Training
   A Random Forest Regressor was selected for use in processing and analyzing real-world agriculture data, as well as modeling possible non-linear relationships within the data. The team ensured that all preprocessing of the data would be done prior to running the model by using a scikit-learn pipeline. The data used to train the model was contained in the training dataset; this is where the model learns.
3. Evaluation
   Regression metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R2 score were used to assess the model on test data that had not yet been seen. Strong predictive performance and good generalization are indicated by the low error values and high R2 score.
   
# Results & Metrics
Since the target variable is a continuous value, the regression metrics for evaluating the model were utilized.

## Metrics to Evaluate Regression
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- R² Score

## Results
- MAE: 9.65
- MSE: 15,954.62
- R² Score: 0.98
The low MAE means the average absolute difference between the predicted and actual values was minimal; the MSE shows large differences between the predictions and actual values are limited; the high R² score demonstrates that the model accounts for most of the variation in the crop yield and indicates that the model has strong predictive capabilities as well as good ability to generalize.
