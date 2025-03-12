# Car Price Prediction using Machine Learning

This project aims to predict the price of Mercedes-Benz GLE cars based on various attributes. The goal is to create an accurate regression model for price estimation.

## ⚙️ Technologies & Libraries Used

Python  <br />
Pandas for data manipulation  <br />
NumPy for numerical operations  <br />
BeautifulSoup for data scraping  <br />
Matplotlib, Seaborn for data visualization  <br />
Scikit-learn for Machine Learning models and preprocessing  <br />
Optuna for hyperparameter tuning  <br />


## 📊 Dataset Description & Preprocessing

1️⃣ Handling Missing Data: remove or filled missing values.  <br />
2️⃣ Feature Engineering: created age feature: age = current year - manufacturing_year  <br />
3️⃣ Create 2 preprocessors One-Hot Encoding and Label Encoding for categorical features. Standardization for numerical features.  <br />

The cleaned dataset contains 760 car records with the following features:  <br />
- price	in Bulgarian Lev - target variable (numerical)
- age of the car (numerical)
- mileage	- km driven (numerical)
- color	of the car (many categories)
- fuel type: gasoline, diesel, etc (many categories)
- hp - horsepower (numerical)
- type - body type: coupe, jeep (binary)
- region where the car is sold (many categories)
- is_amg - whether the car is an AMG model (binary: 0 or 1)


## ML models
Regression models: I try 4 regression models - LinearRegression, DecisionTree, RandomForest, XGBoost  <br />

## 🎯 Hyperparameter Optimization
Optuna was used to tune hyperparameters for each model. Test each model and each preprocessor.

## 📈 Model Evaluation & Visualizations
1️⃣ Mean squared error  <br />
2️⃣ Mean Absolute error  <br />
3️⃣ R-squared  <br />
4️⃣ Residual plots analysis  <br />
5️⃣ Feature Importance analysis: Top 3 most important features are Age, Mileage and HP.  <br />

## 🏆 Results
Here is the results [here](data/test_results12-03-2025.csv).

XGBoost performed the best, achieving the lowest errors (MAE, MSE) and highest R² score.  <br />
Decision Tree and Random Forest also performed well, but XGBoost had better generalization.  <br />
Linear Regression struggled due to non-linearity in data.  <br />





