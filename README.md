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
## Dataset: ●Used Car Listings (Dallas)

- `location`
- `condition`
- `listed_date`
- `listed_time`
- `drive`
- `fuel`
- `odometer`
- `paint color`
- `size`
- `title status`
- `transmission`
- `year`
- `models`
- `cylinders`
- `brand`
- `price` (target variable)

---

## Project Workflow

### 1. Data Preprocessing
- Dropped rows with missing values in core columns required for modeling, including:
'price', 'odometer', 'year', 'condition', 'drive', 'fuel', 'transmission', 'paint color'
- Removed unhelpful or sparse columns like 'size', 'cylinders', and 'type'
- Excluded rows missing geographic coordinates (lat and long) to ensure completeness
- Filtered out outliers:
  1. Kept only cars with odometer < 1,000,000 miles
  2. Kept only cars newer than year 1990
  3. Removed the top 1% most expensive listings to reduce the effect of price outliers on prediction accuracy
- Checked for remaining missing values and printed the final dataset shape

### 2. Exploratory Data Analysis (EDA)

### 1. Price Distribution
To understand the overall pricing landscape of the Dallas used car market, I plotted the distribution of vehicle prices using a histogram (`seaborn.histplot`).

**Key observations:**
- Most vehicles are priced between **$5,000 and $20,000**, indicating a concentration of lower- to mid-priced listings.
- The distribution is **right-skewed**, with a long tail extending up to ~$75,000.
- The long tail suggests the presence of a small number of **high-end or luxury vehicles**, which may require transformation or outlier handling during modeling.

*Plot:*  
![Used Car Price Distribution](https://github.com/user-attachments/assets/de70bd1a-5b0e-4b4b-ae76-42c13cdfa05f)


---

### 2. Price Distribution by Major Brand
To analyze how prices vary by manufacturer, I extracted brand information from the `year_make_model` column and focused on the 10 most common brands (e.g., Toyota, Honda, Ford, BMW, Mercedes).

A boxplot was used to compare the price distributions across brands.

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
