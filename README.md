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

| **Metric**        | **Log_R** | **DT**  | **RF**  | **KNN** | **NB**  | **GB**  | **AB**  |
|--------------------|-----------|---------|---------|---------|---------|---------|---------|
| **Accuracy**       | 0.7468    | 0.7273  | 0.7662  | 0.6623  | 0.7662  | 0.7403  | 0.7338  |
| **Precision**      | 0.6379    | 0.6032  | 0.6727  | 0.5246  | 0.6610  | 0.6271  | 0.6250  |
| **F1 Score**       | 0.6549    | 0.6441  | 0.6727  | 0.5517  | 0.6842  | 0.6491  | 0.6306  |
| **Recall**         | 0.6727    | 0.6909  | 0.6727  | 0.5818  | 0.7091  | 0.6727  | 0.6364  |
| **ROC AUC**        | 0.7303    | 0.7192  | 0.7455  | 0.6444  | 0.7535  | 0.7253  | 0.7121  |


These results have been saved in the file `pima_diabetes.csv`.

---

### **Modified Dataset (Balanced and Scaled)**
To address the **class imbalance** in the Outcome variable, the following preprocessing techniques were applied:
1. **Random Over-Sampling:** To balance the classes.
2. **Standard Scaling:** To scale the data for consistent feature ranges.

| **Metric**        | **Log_R** | **DT**  | **RF**  | **KNN** | **NB**  | **GB**  | **AB**  |
|--------------------|-----------|---------|---------|---------|---------|---------|---------|
| **Accuracy**       | 0.7468    | 0.7468  | 0.7468  | 0.6623  | 0.7662  | 0.7468  | 0.7338  |
| **Precision**      | 0.6379    | 0.6212  | 0.6429  | 0.5246  | 0.6610  | 0.6379  | 0.6250  |
| **F1 Score**       | 0.6549    | 0.6777  | 0.6486  | 0.5517  | 0.6842  | 0.6549  | 0.6306  |
| **Recall**         | 0.6727    | 0.7455  | 0.6545  | 0.5818  | 0.7091  | 0.6727  | 0.6364  |
| **ROC AUC**        | 0.7303    | 0.7465  | 0.7263  | 0.6444  | 0.7535  | 0.7303  | 0.7121  |


The results for this analysis are saved in `pima_diabetes_scaled.csv`.



### Observations and Insights

1. **Logistic Regression (Log_R)**:  
   - Performance metrics such as accuracy and F1 score remained consistent before and after scaling, showing minimal sensitivity to feature scaling.

2. **Decision Tree (DT)**:  
   - Scaling led to improvements across most metrics, particularly in recall (0.6909 → 0.7455) and F1 score (0.6441 → 0.6777).

3. **Random Forest (RF)**:  
   - RF showed consistent accuracy before and after scaling but saw slight variations in metrics like recall and ROC AUC.

4. **K-Nearest Neighbors (KNN)**:  
   - No noticeable performance gain was observed, with accuracy and F1 score remaining nearly identical.

5. **Naive Bayes (NB)**:  
   - Naive Bayes performed robustly both before and after scaling, with high recall and F1 scores.

6. **Gradient Boosting (GB)**:  
   - Performance improved in recall and F1 score after scaling, indicating better handling of imbalanced data.

7. **AdaBoost (AB)**:  
   - Scaling had minimal impact, with most metrics staying consistent, showcasing its robustness.


---

## Acknowledgments
The dataset was provided by the National Institute of Diabetes and Digestive and Kidney Diseases (NIDDK).
Special thanks to the Pima Indian community for participating in this study.





















##
