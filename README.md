# Car Price Prediction

This project predicts the selling price of a used car based on its features, using Linear Regression. I built this as a college project to practice the full machine learning workflow — from raw, messy data to a working model.

# What it does

Given details about a used car (brand, year, mileage, engine size, fuel type, transmission, number of previous owners, etc.), the model predicts what its selling price should be.

# How it works

1. Loaded the car dataset using Pandas
2. Dropped the `torque` column since it wasn't useful for this model
3. Removed missing values and duplicate rows
4. Extracted the brand name from the full car name (e.g. "Maruti Swift Dzire VDI" → "Maruti")
5. Cleaned numeric columns like mileage, max_power, and engine which had units attached as text
6. Encoded categorical columns (brand, fuel type, seller type, transmission, owner type) into numbers
7. Split the data into training and test sets
8. Trained a Linear Regression model to predict `selling_price`
9. Tested the model on sample car details and saved the trained model using Pickle

# Tech used

- Python
- Pandas, NumPy
- Scikit-learn (Linear Regression, train_test_split)
- Pickle (for saving the model)

# Files

- `Car_Price_Model.ipynb` — the main notebook with all the data cleaning, feature engineering, and model training code
- `Cardetails.csv` — the dataset
