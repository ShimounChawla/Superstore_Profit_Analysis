# 🛍️ Superstore Sales & Profit Analysis | Machine Learning Dashboard

This project explores a retail superstore dataset with the goal of uncovering actionable business insights and building predictive models to estimate profit from structured sales data. The analysis covers everything from exploratory data analysis (EDA) to feature engineering, model building, and evaluation using multiple regression techniques.

---

## 📊 Project Objectives

- Analyze sales, profit, discount, and shipping trends
- Identify underperforming product categories and sub-categories
- Uncover regional differences in profitability and shipping modes
- Build and evaluate regression models to predict profit
- Recommend business decisions based on data insights

---

## 📁 Dataset

- **Source**: [Sample - Superstore Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
- **Size**: ~10,000 records
- **Features**:
  - `Order Date`, `Ship Date`, `Category`, `Sub-Category`, `Region`, `Segment`
  - `Sales`, `Profit`, `Discount`, `Shipping Mode`, `Customer ID`, etc.

---

## 🔧 Technologies Used

- **Python**
- **Pandas, NumPy** for data manipulation
- **Matplotlib, Seaborn** for visualization
- **Scikit-learn, LightGBM, XGBoost** for model building
- **Jupyter Notebook** for interactive development

---

## 📚 Workflow Summary

### 1. Data Preprocessing
- Date parsing, feature extraction (`Month`, `Quarter`, `Weekday`)
- Null and duplicate handling
- Whitespace normalization in column names
- One-hot encoding of categorical variables

### 2. Exploratory Data Analysis (EDA)
- Monthly shipment trends
- Profit by region, category, and segment
- Discount vs Profit correlation
- Shipping mode inefficiencies

### 3. Feature Engineering
- Created lag features, binary flags for high discount
- Cleaned column names for model compatibility

### 4. Model Building
- **Random Forest Regressor**
- **XGBoost Regressor**
- **LightGBM Regressor**
- **Gradient Boosting Regressor**
- **Support Vector Regressor (SVR)**

### 5. Model Evaluation
- Cross-validation using `GridSearchCV`
- Metrics: **R² Score**, **RMSE**, **MAE**
- Comparison of model performances on test set

---

## 📈 Results

- Achieved R² > 0.84 on best models
- Identified major profit leaks in high-discount, low-margin categories
- Suggested actions:
  - Cap discounts based on category
  - Optimize shipping cost per region
  - Focus on profitable customer segments

---

## 🚀 How to Run This Notebook

### ✅ Prerequisites:
Make sure you have the following Python libraries installed:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost lightgbm
