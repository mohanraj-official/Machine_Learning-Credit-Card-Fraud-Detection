# Credit Card Fraud Detection

## Dataset Overview

- **Rows:** 5000  
- **Columns:** 13  
  - **Numerical Columns:** 5  
  - **Categorical Columns:** 7  

---

| info |
|--|
|![info](https://github.com/user-attachments/assets/df94555d-7b49-4e17-bd58-dddc0637b4cc)|

## Key Insights

| describe |
|---|
|![describe](https://github.com/user-attachments/assets/d496a448-735e-4775-84c1-afadc0d4714a)|

### 1. Most Used Card Types:
- **MasterCard** and **Visa** are the most commonly used card types.

### 2. Most Common Merchant Categories:
- **Online Shopping** and **Retail** are the most frequently used merchant categories.

### 3. Fraudulent Transactions Insights:
- **Transaction Amount:** Fraud is most common for transaction amounts between **25,000 to 50,000**.
- **Cardholder Monthly Income:** Fraud is very rare for monthly incomes between **2,50,000 to 3,00,000**.
- **Cardholder Average Spend:** Fraud is very rare when the **Cardholder's Average Spend** is greater than **1,00,000**.
- **Regions:** Fraud is observed across all regions, but the **West** and **South** regions have significantly more fraudulent cases than the **East** and **North** regions.

---

| Eda - 1 |
|--|
|![Eda - 1](https://github.com/user-attachments/assets/542b315b-3dd4-498a-9353-d3f5519c6c46)|

| Eda - 2 |
|--|
|![Eda - 2](https://github.com/user-attachments/assets/179f88d5-b6ad-45d0-8e48-c689456c59b6)|

| Eda - 3 |
|---|
|![Eda - 3](https://github.com/user-attachments/assets/455064dc-7bfc-467a-866f-3bcb9542a571)|

| Eda - 4 |
|--|
|![Eda - 4](https://github.com/user-attachments/assets/7a405aa8-27a1-4d07-9c6b-487e2ea5ffda)|

| Eda - 5 |
|--|
|![Eda - 5](https://github.com/user-attachments/assets/7967a0bb-adc9-4d99-8f3c-d3c0bed3490b)|

| Eda - 6|
|---|
|![Eda - 6](https://github.com/user-attachments/assets/b304c84b-2767-43ce-b336-d45831a9c62e)|

| Eda - 7 |
|---|
|![Eda - 7](https://github.com/user-attachments/assets/57bb541b-fbc2-4465-94ff-515d78110098)|

| Eda - 8 |
|----|
|![Eda - 8](https://github.com/user-attachments/assets/5c4620e4-9ba4-4290-b166-c726b0bb0890)|

| Example code |
|---|
|![Example code](https://github.com/user-attachments/assets/d7babcd4-464e-4df4-b4bd-308a77e7b0ac)|

## Exploratory Data Analysis (EDA)

### a. Distribution of Categorical Features
- **Card Type**
- **Merchant Category**
- **Location**

### b. Distribution of Numerical Features
- Box plots and KDE plots were used to analyze:
  - **Transaction Amount**
  - **Cardholder Average Spend**
  - **Cardholder Monthly Income**
  - **Credit Limit**
  - **Cardholder Age**

### c. Bivariate and Multivariate Analysis
- Analyzed relationships between:
  - **Transaction Amount** and **Fraudulent Transactions**
  - **Card Type** and **Fraudulent Transactions**
  - **Merchant Category** and **Fraudulent Transactions**
  - **Region** and **Fraudulent Transactions**

---

## Data Preprocessing

### a. Imputation for Missing Values
- Categorical Features:
  - Missing values were filled with the **mode**.
- Numerical Features:
  - Missing values were filled with the **mean**.

### b. Handling Outliers
- Used the **IQR method** to identify and remove outliers in numerical features.

### c. Skewness Adjustment
- Applied transformations to reduce skewness in features.

---

## Feature Engineering

### a. Identifying Categorical Features
- Identified the following columns:
  - **Card Type**
  - **Merchant Category**
  - **Region**

### b. Encoding Categorical Features
- Used **LabelEncoder** to encode the categorical columns.

---

## Feature Selection

### a. Relevant Features
- Based on correlation analysis, the following features were selected:
  - **Transaction Amount**
  - **Cardholder Average Spend**
  - **Cardholder Monthly Income**
  - **Credit Limit**

### b. Irrelevant Features Removed
- Dropped features such as **Transaction ID**.

---

## Train-Test Split

### a. Splitting the Data
- Split the dataset into training and testing sets using an **80:20 ratio**.

### b. Feature Scaling
- Applied **StandardScaler** for scaling numerical features.

---

## Machine Learning Models

### a. Models Evaluated
- **Logistic Regression**
- **Gaussian Naive Bayes**
- **Decision Tree Classifier**
- **Random Forest Classifier**
- **K-Nearest Neighbors (KNN)**
- **Support Vector Classifier (SVC)**

### b. Performance Metrics
- Evaluated using:
  - **Accuracy Score**
  - **F1 Score**
  - **Precision Score**
  - **Recall Score**
  - **Confusion Matrix**

### c. Best Performing Models
- The following models achieved the highest accuracy:
  - **Logistic Regression**
  - **Gaussian Naive Bayes**
  - **Decision Tree Classifier**
  - **Random Forest Classifier**

---


## Summary

- Fraud detection is critical in ensuring financial security.
- Analyzed patterns and trends in credit card transactions to identify fraudulent activities.
- Implemented machine learning models to predict fraud with **73% accuracy** using top-performing algorithms.

