# Vehicle-Inventory-Prediction
# Datathon Results

This document summarizes the results of the datathon, including the models used, their performance, and the corresponding submission files. Each Jupyter Notebook (.ipynb) contains implementations of both Decision Tree and Random Forest models.

## 1. Random Forest (Baseline)

**Data Used:** Raw data (no preprocessing).

- **Decision Tree RMSE:** 8001.78(discared)
- **R^2 on test set:** 0.89
- **Random Forest RMSE:** 7573.58
- **R^2 on test set:** 0.90
- **Submission File:** submission_file_updated.xlsx
- **Notebook:** random_forest.ipynb

## 2. Random Forest with NA Filled

**Data Used:**

- Filled missing values in `['model_year']` using the median value and converted to integer.
- Added an age variable (numerical).

- **Decision Tree RMSE:** 5213.35(discared)
- **R^2 on test set:** 0.96
- **Random Forest RMSE:** 4773.67
- **R^2 on test set:** 0.97
- **Submission File:** submission_file_updated_fill_na.xlsx
- **Notebook:** random_forest_fill_na.ipynb

## 3. Random Forest with Fuel Type Classification

**Data Used:**

- Same as 2, with an additional binary classification feature for fuel type.

- **Decision Tree RMSE:** 5381.77(discared)
- **R^2 on test set:** 0.94
- **Random Forest RMSE:** 4738.51
- **R^2 on test set:** 0.97
- **Submission File:** submission_file_updated_class.xlsx
- **Notebook:** random_forest_2class.ipynb

## 4. XGBoost

**Data Used:** Same as 2 (filled NA and added age variable).

- **RMSE:** 3895.53
- **R^2 on test set:** 0.96
- **Submission File:** submission_file_xgboost.xlsx
- **Notebook:** Cheveron_xgb.ipynb
- 

## 5. Summary

- **Best Model:** XGBoost
- **Best RMSE:** 3895.53
- **Best Submission File:** submission_file_xgboost.xlsx

**Notes:**

- The XGBoost model achieved the best performance with the lowest RMSE.
- Further improvements could be explored by:
    - Tuning hyperparameters.
    - Incorporating additional features or advanced feature engineering techniques.

## Notebook Structure

Each Jupyter Notebook (.ipynb) contains the following:

1. **Data Preprocessing:** Steps to clean and prepare the data.
2. **Decision Tree Model:** Implementation and evaluation of the Decision Tree model.
3. **Random Forest Model:** Implementation and evaluation of the Random Forest model.
4. **Submission File Generation:** Code to generate the submission file for each model.

This concludes the summary of the datathon results. For further details, refer to the respective Jupyter Notebooks and submission files.
