# Google Play Store App Sales Analysis

This project focuses on analyzing and predicting the number of downloads for apps on the Google Play Store using machine learning. The dataset includes information about the apps such as ratings, reviews, price, size, category, and the last updated date.

## Analysis Steps

1. **Data Loading**:
   - The data is loaded from a CSV file `googleplaystore.csv` containing information about Google Play Store apps.

2. **Data Cleaning**:
   - Dates in the `Last Updated` column are converted to datetime format.
   - A new column `Days Since Last Updated` is added, representing the number of days since the last update.

3. **Feature Selection**:
   - Selected columns are `Rating`, `Reviews`, `Price`, `Size`, `Category`, and `Days Since Last Updated` as features for the model.
   - The target column is `Installs`, representing the number of downloads.

4. **Converting Categorical Variables**:
   - The `Category` column is converted to numerical values using one-hot encoding.

5. **Data Splitting**:
   - The data is split into training and testing sets with an 80/20 ratio.

6. **Model Training**:
   - A Random Forest Regressor is used to train the model on the training set.

7. **Model Evaluation**:
   - The model is evaluated using Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²) metrics on the test set.

8. **Future Sales Prediction**:
   - An example prediction for a future app is made using the trained model.

## Results

- The model evaluation shows MAE, MSE, and R² results which help in assessing the model's performance.

## Tools and Libraries Used

- Python
- Pandas
- Scikit-learn

## Running the Project

1. Run google_store.ipynb in jupyter notebook or visual studio code.
