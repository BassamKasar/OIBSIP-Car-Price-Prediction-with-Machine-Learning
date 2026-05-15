# Car Price Prediction using Machine Learning

## Project Overview
Car price prediction is a critical research area in machine learning. This project aims to estimate the resale value of a car based on various features such as its original price, mileage, fuel type, transmission, and age. This model helps both buyers and sellers determine a fair market price for used vehicles.

## Dataset Description
The model is trained using the **"car data.csv"** dataset, which includes the following features:
* **Car_Name**: Name of the car model.
* **Year**: Year of manufacture (used to calculate **Car_Age**).
* **Selling_Price**: The target variable (price at which the car is being sold).
* **Present_Price**: The current showroom price of the car.
* **Driven_kms**: Total kilometers the car has been driven.
* **Fuel_Type**: Petrol, Diesel, or CNG.
* **Selling_type**: Dealer or Individual seller.
* **Transmission**: Manual or Automatic.
* **Owner**: Number of previous owners.

## Technical Stack
* **Language:** Python
* **Libraries:** 
  * `Pandas` & `NumPy` for data manipulation.
  * `Matplotlib` & `Seaborn` for data visualization.
  * `Scikit-Learn` for model building and evaluation.

## Workflow
1. **Data Cleaning:** Checked for missing values and duplicates.
2. **Feature Engineering:** Derived `Car_Age` from the `Year` column to improve model accuracy.
3. **Exploratory Data Analysis (EDA):** 
   * Created **Scatter Plots** to visualize the relationship between Present Price and Selling Price.
   * Generated a **Correlation Heatmap** to identify key price drivers.
4. **Data Preprocessing:** Performed One-Hot Encoding on categorical variables.
5. **Model Training:** Implemented a **Random Forest Regressor** with an 80/20 train-test split.
6. **Evaluation:** Validated the model using R² Score and Mean Absolute Error (MAE).

## Results
Our model demonstrates high predictive power:
- **R² Score:** `0.96` (The model explains 96% of the price variance)
- **Mean Absolute Error:** `0.64 Lakhs`
