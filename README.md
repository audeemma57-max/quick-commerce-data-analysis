 #Quick Commerce Data Analysis & Delivery Time Prediction

 #Project Overview

This project analyses quick-commerce order data across major Indian cities
and delivery platforms.

The objective is to identify business and operational patterns and generate
data-driven insights related to revenue, customer satisfaction, order value,
discounts, delivery performance, and delivery time prediction.

The project is structured into three main parts:

1. Exploratory Data Analysis (EDA)
2. Business Analysis & KPIs
3. Predictive Modelling

---

# Objectives

The analysis aims to:

- Compare revenue performance across platforms
- Analyse Average Order Value (AOV)
- Compare customer satisfaction
- Study delivery performance
- Analyse the impact of discounts on order value
- Identify promising cities for expansion
- Evaluate operational efficiency
- Predict delivery time using machine learning

---

# Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Exploratory Data Analysis (EDA)
- Data Visualization
- Statistical Analysis
- Machine Learning

---

# Part 1: Exploratory Data Analysis

The first part explores the main characteristics of the dataset.

# Revenue Performance

Swiggy Instamart generated the highest total revenue,
followed by Blinkit and Zepto.

# Average Order Value

Swiggy Instamart also recorded the highest Average Order Value (AOV),
indicating higher spending per transaction.

# Customer Satisfaction

Customer satisfaction varies across platforms.

Blinkit recorded the highest average customer rating,
while Dunzo showed lower satisfaction levels.

# Delivery Time & Partner Ratings

The Pearson correlation between delivery time and delivery partner
ratings was approximately -0.003, indicating an almost negligible
linear relationship between the two variables.

# Customer Segment Analysis

For Swiggy Instamart customers aged 30–40 in Mumbai,
dairy products were the most popular category, followed by groceries
and fresh produce.

---

# Part 2: Business Analysis & KPIs

# Impact of Discounts

Orders with discounts had a higher median order value:

- Without discount: approximately ₹450
- With discount: approximately ₹670

This suggests an association between discounts and larger basket sizes.

# City Expansion Analysis

Bengaluru recorded a customer satisfaction score of 3.47,
approximately 79K orders, and ₹46M in total revenue.

Delhi recorded an average delivery time of approximately 7.14 minutes.

These metrics were used to identify cities with different combinations
of customer satisfaction, order volume, revenue and delivery efficiency.

# Operational Efficiency

Zepto recorded the fastest average delivery time at approximately
9.64 minutes and the highest orders-per-minute ratio in the analysis.

Blinkit combined an average delivery time of approximately 15.12 minutes
with total revenue of approximately ₹72.5M.

Swiggy Instamart generated the highest total revenue despite a slower
average delivery time.

---

# Part 3: Predictive Modeling

# Objective

The objective of the machine learning model was to predict delivery time
based on order characteristics.

# Model

A Random Forest Regressor with 100 estimators was trained.

The dataset was divided into:

- 80% training data
- 20% test data
- random state = 42

# Features

The model used:

- Distance (km)
- Items count
- Order value
- City
- Company
- Product category
- Discount applied
- Payment method

Categorical variables were encoded using LabelEncoder.

---

# Model Performance

The model achieved the following results:

| Metric | Result |
|---|---:|
| MSE | 1.32 |
| RMSE | 1.15 min |
| MAE | 0.97 min |
| R² | 0.967 |

The feature importance analysis identified City, Company and Distance
as the main predictors of delivery time.

---

# Key Findings

The analysis identified several important patterns:

- Swiggy Instamart generated the highest total revenue
- Zepto recorded the fastest average delivery time
- Bengaluru had the highest customer satisfaction score
- Delhi showed particularly fast delivery performance
- Discounted orders had a higher median order value
- City, Company and Distance were the main model features associated
  with delivery time

---

# Limitations

The dataset appears to be synthetically generated, which limits the
real-world interpretation of the model performance.

Important operational variables such as:

- Weather
- Traffic
- Time of day
- Rider availability

were not included in the dataset.

The use of LabelEncoder for categorical variables such as City and
Company may also introduce artificial ordinal relationships.

Therefore, the high R² score should not be interpreted as representative
of real-world predictive performance.

---

# Project Files

- Projet python kanga blengbi.ipynb — Complete Python analysis,
  visualizations and predictive modeling.

---

## Authors

*Blengbi Kanga*  
*Sophia Troquereau*

SKEMA Business School
