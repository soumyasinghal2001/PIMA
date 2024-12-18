# Pima Indians Diabetes Analysis
## Overview
The Pima Indians Diabetes Dataset is a widely used dataset for exploring machine learning techniques and statistical analysis related to diabetes prediction.
This project analyzes the dataset to identify patterns and factors contributing to diabetes, leveraging data science tools and techniques.

## Dataset Description
The dataset contains medical and demographic data collected from Pima Indian women aged 21 and above, living near Phoenix, Arizona. 
The primary goal is to predict whether a patient is likely to have diabetes based on diagnostic measurements.

## Features
Pregnancies: Number of times pregnant.
Glucose: Plasma glucose concentration (2 hours after a glucose tolerance test).
BloodPressure: Diastolic blood pressure (mm Hg).
SkinThickness: Triceps skinfold thickness (mm).
Insulin: 2-Hour serum insulin (mu U/ml).
BMI: Body mass index (weight in kg/(height in m)^2).
DiabetesPedigreeFunction: A function that scores the likelihood of diabetes based on family history.
Age: Age in years.
Outcome: Binary (0 or 1), indicating whether diabetes is present (1) or not (0).

## Project Objectives
### Exploratory Data Analysis (EDA):
Understand feature distributions and correlations using Histogram and Correlation Matrix.
Identify missing or inconsistent values.

### Data Preprocessing:
Handle missing data.
Normalize or standardize features for better model performance.

### Modeling:
Develop machine learning models to predict diabetes.
Compare model performance using metrics such as accuracy, precision, recall, and F1-score.

### Insights:
Identify the most important factors influencing diabetes prediction.
Provide actionable recommendations for healthcare professionals.

Here’s how we can incorporate your **Results** section into the README in a polished manner:

---

## **Results**

### **Original Dataset**
Using the original `diabetes.csv` dataset, we evaluated multiple machine learning models. The key findings are as follows:

- **Accuracy:**  
  - **Decision Tree** and **Naive Bayes** performed best, achieving an accuracy of **76.6%**.
  
- **Precision:**  
  - **Naive Bayes** performed the best with a precision score of **66.1%**.
  
- **ROC-AUC:**  
  - **Decision Tree** outperformed others with an AUC score of **76.16%**.

These results have been saved in the file `pima_diabetes.csv`.

---

### **Modified Dataset (Balanced and Scaled)**
To address the **class imbalance** in the Outcome variable, the following preprocessing techniques were applied:
1. **Random Over-Sampling:** To balance the classes.
2. **Standard Scaling:** To scale the data for consistent feature ranges.

Post preprocessing, **Naive Bayes** outperformed all other models with the following metrics:
- **Accuracy:** **76.6%**
- **Precision:** **66.1%**
- **ROC-AUC:** **75.35%**

The results for this analysis are saved in `pima_diabetes_scaled.csv`.

---

## Acknowledgments
The dataset was provided by the National Institute of Diabetes and Digestive and Kidney Diseases (NIDDK).
Special thanks to the Pima Indian community for participating in this study.





















##
