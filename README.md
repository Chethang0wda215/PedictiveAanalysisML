# PedictiveAanalysisML
California Housing Price Prediction

# Predictive Analysis Using Machine Learning

## California Housing Price Prediction

---

##  Project Overview

This project focuses on building a **machine learning regression model** to predict housing prices using the California Housing dataset. The workflow includes data preprocessing, feature engineering, model training, hyperparameter tuning, and evaluation.

---

##  Objective

To develop a predictive model that estimates **median house values** based on various socio-economic and geographical features.

---

##  Dataset Description

The dataset contains information such as:

* Longitude & Latitude
* Housing Median Age
* Total Rooms & Bedrooms
* Population & Households
* Median Income
* Ocean Proximity (categorical)
* Median House Value (target variable)

---

##  Steps Performed

### 1. Data Loading

* Imported dataset from local storage
* Inspected structure using `.info()`, `.describe()`

### 2. Data Preprocessing

* Handled missing values (`total_bedrooms`)
* Converted categorical feature (`ocean_proximity`) using one-hot encoding
* Feature scaling using `StandardScaler`

### 3. Feature Engineering

Created new features:

* Rooms per household
* Bedrooms per room
* Population per household

---

### 4. Feature Selection

* Correlation analysis performed
* Identified important predictors such as:

  * Median income
  * Location features

---

### 5. Model Building

Models used:

* Linear Regression
* Random Forest Regressor

---

### 6. Hyperparameter Tuning

Used `GridSearchCV` to find optimal parameters:

Best parameters:

* `n_estimators = 100`
* `max_depth = 20`

---

### 7. Model Evaluation

Evaluation metrics used:

* Root Mean Squared Error (RMSE)
* R² Score

Findings:

* Random Forest outperformed Linear Regression
* Tuned model showed improved performance

---

### 8. Visualization

* Scatter plot of Actual vs Predicted values
* Observed strong correlation with some dispersion

---

### 9. Key Insights

* Median income is the most influential feature
* Model performs well overall but struggles with extreme values
* Dataset has a price cap (~500,000), affecting predictions

---

##  Results Summary

* Tuned Random Forest achieved the best performance
* Good predictive capability with room for improvement

---

##  Future Improvements

* Use advanced models (e.g., Gradient Boosting, XGBoost)
* Perform cross-validation
* Handle capped values more effectively
* Add more relevant features

---

##  Technologies Used

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn

---

##  Project Structure

* `notebook.ipynb` → Complete workflow
* `housing.csv` → Dataset
* `README.txt` → Project documentation

---

##  Conclusion

This project successfully demonstrates a complete machine learning pipeline for regression analysis. The tuned Random Forest model provides reliable predictions and highlights the importance of feature engineering and hyperparameter optimization.

---

##  Author

Chethan Gowda

---

