📊 Housing Price Prediction Project
🏠 Overview

This project focuses on predicting housing prices using machine learning techniques. It leverages a housing dataset to perform data preprocessing, exploratory data analysis (EDA), feature engineering, and model building.

The goal is to build accurate regression models that can estimate house prices based on various features such as location, population, number of rooms, and more.

📁 Dataset

The dataset used in this project contains housing-related features including:

Median income
Total rooms
Total bedrooms
Population
Households
Latitude & Longitude
Ocean proximity
Median house value (target variable)

📌 Dataset file: Housing.csv

⚙️ Technologies Used
Python 🐍
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn

🔍 Project Workflow
1. Data Loading & Cleaning
Loaded dataset using Pandas
Checked dataset structure (info())
Removed missing values using dropna()
2. Exploratory Data Analysis (EDA)
Histograms to understand feature distributions
Correlation heatmaps to identify relationships
Scatter plots for geographic visualization
3. Feature Engineering
Log transformation applied to skewed features:
total_rooms
total_bedrooms
population
households
Created new features:
bedroom_ratio
household_rooms
One-hot encoding for categorical feature:
ocean_proximity
4. Model Building
📈 Linear Regression
Trained a baseline model using LinearRegression
Evaluated using test data score
🌲 Random Forest Regressor
Built a more powerful ensemble model
Improved performance compared to linear regression
5. Hyperparameter Tuning

Used GridSearchCV to optimize Random Forest parameters:

param_grid = {
    "n_estimators": [3, 10, 30],
    "max_features": [2, 4, 6, 8]
}
Selected best model using cross-validation
Final model: best_forest

📊 Results
Model	Performance
Linear Regression	Moderate
Random Forest	Better
Tuned Random Forest	Best

📌 Key Insights
Feature engineering significantly improves model performance
Random Forest outperforms Linear Regression for this dataset
Hyperparameter tuning further boosts accuracy

🧠 Future Improvements
Try advanced models (XGBoost, Gradient Boosting)
Perform feature selection
Handle outliers more effectively
Deploy model using Flask or Streamlit

👨‍💻 Author
Tushar Pareek
