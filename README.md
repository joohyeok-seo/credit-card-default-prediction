# Credit Card Default Prediction

This repository contains a comprehensive machine learning project focused on predicting whether a credit card customer will default on their payment for the next month. The project demonstrates end-to-end data analysis, preprocessing, model development, and evaluation using Python and Scikit-learn.

---

## **Overview**

In the financial industry, understanding customer behavior is critical to managing risks. This project utilizes a publicly available credit card dataset to predict default probabilities. It includes data exploration, cleaning, feature engineering, and classification modeling to build an accurate and interpretable model.

---

## **Project Goals**
- Analyze the relationship between customer demographics and default probabilities.
- Build a classification model to predict customer defaults with high precision and recall.
- Optimize model performance through hyperparameter tuning and evaluation.
- Automate the data preprocessing and modeling process using Scikit-learn pipelines.

---

## **Dataset**

The dataset contains information about credit card customers, including:
- **Demographics**: Age, education level, marital status, and gender.
- **Financial Information**: Limit balance, payment history, and bill amounts.
- **Target Variable**: `default_payment_next_month` (1 if the customer defaulted, 0 otherwise).

---

## **Key Features**

### **1. Exploratory Data Analysis (EDA)**
- Visualized trends between default rates and features such as education level, age, and payment history.
- Identified feature distributions and handled outliers effectively.

### **2. Data Preprocessing**
- **Missing Value Imputation**:
  - Numerical features: Replaced missing values with the median.
  - Categorical features: Replaced missing values with the mode.
- **Feature Encoding**:
  - One-hot encoding for categorical variables.
  - Target encoding to improve performance for imbalanced data.
- **Data Splitting**:
  - Stratified train-test split to ensure proportional representation of the target variable.

### **3. Machine Learning Modeling**
- Built a Decision Tree model using Scikit-learn.
- Evaluated model performance using confusion matrix, precision-recall curves, and ROC-AUC.

### **4. Hyperparameter Tuning**
- **GridSearchCV**:
  - Explored all combinations of hyperparameters such as max depth, criterion, and min samples per leaf.
- **RandomizedSearchCV**:
  - Selected hyperparameters randomly to reduce computation time for large search spaces.

### **5. Pipeline Integration**
- Integrated data preprocessing and modeling into a single Scikit-learn pipeline for reproducibility.

---

## **Results**

- **Key Metrics**:
  - **Accuracy**: 85%
  - **Precision**: 0.78
  - **Recall**: 0.80
  - **ROC-AUC**: 0.85
- Successfully optimized the Decision Tree model for better recall, ensuring effective prediction of defaulting customers.

---
