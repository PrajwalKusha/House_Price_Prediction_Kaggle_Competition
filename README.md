# House Price Prediction Model Card

This repository contains a machine learning pipeline for predicting house prices using scikit-learn. Features include preprocessing, feature engineering, and models like Gradient Boosting and Random Forest. Includes a .ipynb, submission file, and model card. Ideal for real estate and predictive modeling projects.

# Basic Information
* **Group Members:**
   * **Prajwal Kusha - p.kusha@gwmail.gwu.edu**
   * Manasi Jha -
   * Kumar Tare -
   * Isheneasu -
     
* **Model Date: Decemeber, 2024**
* **Model Version: 1.0**
* **License: MIT** 
* **Model Implementation Code: [Link to your notebook, if applicable]**

## Intended Use:
* **Intended Uses:** Predict house sale prices based on property features for real estate analysis and market trend predictions.
* **Intended Users:** Real estate professionals, data analysts, and researchers.
* **Out-of-Scope Uses:** This model is not suitable for applications requiring legal or financial guarantees or for use outside the distribution of the training dataset.

# Training Data: 
* **Source:** The dataset is sourced from **Kaggle's "House Prices: Advanced Regression Techniques"** competition.

* **How Data was divided:**
  * **80% training data**
  * **20% validation data**

* **Data Dictionary:**

| Name           | Modeling Role | Measurement Level | Description                             |
|----------------|---------------|-------------------|-----------------------------------------|
| MSSubClass     | Predictor     | Categorical       | Building class                          |
| LotFrontage    | Predictor     | Continuous        | Lot size in feet                        |
| PropertyAge    | Predictor     | Continuous        | Age of the property at sale             |
| OverallQual    | Predictor     | Ordinal           | Overall material and finish quality     |
| SalePrice      | Target        | Continuous        | Sale price of the house                 |

# Test Data:
* **Source:** Kaggle's **"House Prices: Advanced Regression Techniques" test dataset.**
* **Number of Rows:** 1459 rows.

* **Differences:**
  * The test dataset lacks the `SalePrice` column, which is the target variable in the training dataset.

# Quantitative Analysis
* **Metrics Used: Root Mean Squared Error (RMSE)**
* **Final Values:**

| Dataset      | RMSE       |
|--------------|------------|
| Training     | 26348.71   |
| Validation   | 27897.11   |
| Test (estimate) | TBD        |

> **Note**: The test RMSE is not included because the true labels (`SalePrice`) for the test dataset are not available in the provided data. Validation RMSE is used as an estimate of the test performance.

* **Plots:**
1. **Feature Importance Plot:**
     * **Description:** The plot ranks the features by their importance in predicting house prices. The top features contributing to the model's accuracy are shown.
     * **Top Features:** OverallQual, GrLivArea, GarageCars, TotalBsmtSF, 1stFlrSF
     * **Insights:** The model relies heavily on quality and size-related features to predict the target variable.
2. 
    
