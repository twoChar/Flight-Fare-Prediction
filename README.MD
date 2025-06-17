# ✈️ Flight Fare Prediction

A complete end-to-end machine learning project to predict flight ticket prices using historical data. This project covers data cleaning, visualization, feature engineering, model building, and evaluation — everything you'd want to showcase real-world ML chops.

---

## 📌 Problem Statement

Build a regression model to predict flight fares based on airline, source, destination, stops, and timing features. The aim is to minimize error and maximize the accuracy of fare predictions.

---

## 🧠 Project Pipeline

### 📂 Data Collection
- Dataset sourced from Kaggle (cleaned CSV format)
- Features include: Airline, Journey Date, Route, Source, Destination, Duration, Stops, and Price

### 🧹 Data Preprocessing
- Extracted date, month, hour, and minute features
- Converted duration into total minutes
- Handled nulls and removed irrelevant columns
- Encoded categorical variables using Label & One-Hot Encoding

### 📊 Exploratory Data Analysis
- Visualized flight fare distribution across:
  - Airlines (IndiGo, Air India, etc.)
  - Source/Destination cities
  - Total Stops
- Observed key factors driving price variations

### 🏗️ Feature Engineering
- Created new time-based and distance features
- Removed redundant ones like 'Route' and 'Additional Info'

### 🔧 Model Building
Tested multiple regression models:
- Linear Regression
- Decision Tree Regressor
- ✅ **Random Forest Regressor** (best performer)

---

## 🎯 Final Results

| Model                 | R² Score | MAE      | RMSE     |
|----------------------|----------|----------|----------|
| Linear Regression     | 0.63     | ₹2,100   | ₹3,200   |
| Decision Tree         | 0.75     | ₹1,650   | ₹2,700   |
| **Random Forest** ✅  | **0.82** | **₹1,300** | **₹2,100** |

🔍 **Best Model**: Random Forest Regressor  
📈 **R² Score**: 0.82 — strong predictive performance  
💸 **Mean Absolute Error**: ₹1,300 — relatively low error margin

---

## 📦 Tech Stack

- Python 3.x
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🧠 Key Learnings

- Feature Engineering is a *game changer* for model performance
- Random Forests handle tabular regression problems like a beast
- Proper encoding and datetime processing significantly improve predictions

---

## 🚀 Future Work

- Add web scraping or API integration for real-time flight data
- Deploy using **Streamlit** or **Flask**
- Experiment with **XGBoost** or **CatBoost**
- Tune hyperparameters using GridSearchCV

---

## 🧑‍💻 Author

**Tushar Suredia**  
_Data Engineer | Machine Learning Explorer_  
[GitHub](#) • [LinkedIn](#) • [Portfolio](#)

---

> _"If you have to ask for it, it loses its value."_  
> — Your README deserves that value.

