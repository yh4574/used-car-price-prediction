# Used Car Price Prediction

Introduction

The used car market plays a significant role in the automotive industry and is influenced by factors, including brand, mileage, year, fuel type, etc. With the increasing availability of used car listings online, this project aims to apply data science techniques to predict the price of a used car based on their features, enabling better decision-making for buyers, sellers, and platforms.This project focuses specifically on the Dallas market, leveraging a dataset of used car listings from the region. 

---
Objectives
- Explore the factors that most significantly impact used car pricing in the Dallas region
- Build regression models to predict car prices
- Evaluate the model's performance and interpret key drivers of price variation
- Provide insights that can guide pricing strategies for sellers or filtering options for buyers

---
## Dataset
The dataset consists of used car listings collected from a public source.  
It includes key variables such as:

- `year`
- `mileage`
- `condition`
- `fuel`
- `manufacturer`
- `model`
- `odometer`
- `price` (target variable)

No personal or sensitive information is included.

---

## 🔍 Project Workflow

### 1. Data Cleaning
- Handle missing values  
- Remove unrealistic values (e.g., negative mileage or extreme outliers)  
- Convert categorical variables into usable formats  

### 2. Exploratory Data Analysis (EDA)
- Distribution of car prices  
- Correlation between year/mileage and price  
- Price differences across brands and fuel types  

### 3. Feature Engineering
- Age of the car  
- Condition level encoding  
- One-hot encoding for categorical features  

### 4. Model Building
Models tested include:

- Linear Regression  
- Decision Tree  
- Random Forest  

The goal is to compare model performance and choose the best-performing one.

---

## Model Performance
Key evaluation metrics:

- **R² Score**
- **RMSE (Root Mean Squared Error)**

*(Add your model results here after reviewing the notebook)*

---

## Key Insights
- Newer cars with lower mileage predictably have higher prices  
- Condition and brand significantly influence price  
- Ensemble tree models (e.g., Random Forest) tend to outperform linear models for this dataset  

---

## What I Learned
- How to clean and preprocess real-world datasets  
- The full machine learning workflow from EDA to modeling  
- How to evaluate models using appropriate metrics  
- How to interpret machine learning outputs and extract business insights  
