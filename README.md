# used car price prediction
# Used Car Price Prediction

This project aims to build a machine learning model to predict the price of used cars based on publicly available listing data.  
It explores how factors such as mileage, model year, condition, fuel type, and brand influence market value.

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
