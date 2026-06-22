# 🏢 Employee Attrition Prediction using Machine Learning

## 📌 Project Overview

Employee attrition is one of the biggest challenges organizations face because replacing experienced employees is costly and time-consuming. This project applies supervised machine learning techniques to predict whether an employee is likely to leave the company based on demographic, job-related, and workplace factors.

The project demonstrates an end-to-end machine learning workflow, including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and performance comparison.

---

## 🎯 Business Problem

High employee turnover affects productivity, recruitment costs, and organizational performance.

The objective of this project is to build a predictive model that helps Human Resources (HR) identify employees at risk of leaving so that proactive retention strategies can be implemented.

---

# Dataset Information

The dataset contains employee demographic, professional, and workplace-related information.

### Target Variable

| Column    | Description                                   |
| --------- | --------------------------------------------- |
| Attrition | Whether an employee left the company (Yes/No) |

### Example Features

* Age
* BusinessTravel
* Department
* DailyRate
* DistanceFromHome
* Education
* EducationField
* EnvironmentSatisfaction
* JobLevel
* JobRole
* JobSatisfaction
* MaritalStatus
* MonthlyIncome
* MonthlyRate
* NumCompaniesWorked
* OverTime
* PercentSalaryHike
* PerformanceRating
* RelationshipSatisfaction
* StockOptionLevel
* TotalWorkingYears
* TrainingTimesLastYear
* WorkLifeBalance
* YearsAtCompany
* YearsInCurrentRole
* YearsSinceLastPromotion
* YearsWithCurrManager

---

# Project Workflow

## 1. Data Understanding

* Loaded the dataset using Pandas
* Explored dataset dimensions
* Inspected data types
* Reviewed feature descriptions

---

## 2. Data Cleaning

Performed data quality checks including:

* Missing value detection
* Duplicate record detection
* Data consistency verification

Results:

* ✅ No missing values
* ✅ No duplicate records

---

## 3. Exploratory Data Analysis (EDA)

Exploratory analysis was performed to understand employee behavior and identify factors associated with attrition.

Examples include:

* Employee Attrition Distribution
* Department vs Attrition
* Overtime vs Attrition
* Monthly Income vs Attrition
* Age vs Attrition
* Business Travel vs Attrition
* Work-Life Balance vs Attrition

Key observations:

* Employees working overtime showed higher attrition.
* Research & Development contained the largest workforce and the highest number of employees leaving.
* The dataset is imbalanced, with significantly more employees staying than leaving.

---

## 4. Data Preprocessing

Preprocessing steps include:

* Label Encoding
* One-Hot Encoding (where appropriate)
* Feature Scaling
* Train/Test Split

---

## 5. Machine Learning Models

Multiple classification algorithms are trained and compared.

Examples:

* Logistic Regression
* Decision Tree
* Random Forest
* Support Vector Machine (SVM)
* K-Nearest Neighbors (KNN)
* XGBoost *(optional)*

---

## 6. Model Evaluation

Evaluation metrics include:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC Score
* Confusion Matrix
* Classification Report

Because the dataset is imbalanced, model performance is evaluated using metrics beyond accuracy.

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

# Project Structure

```
Employee-Attrition-Prediction/
│
├── data/
│   └── employee_attrition.csv
│
├── notebooks/
│   └── Employee_Attrition_EDA.ipynb
│
├── models/
│
├── images/
│
├── requirements.txt
│
├── README.md
│
└── LICENSE
```

---

# Results

After comparing multiple machine learning models, the best-performing model was selected based on overall predictive performance rather than accuracy alone.

Special attention was given to Recall and F1-Score due to the class imbalance, ensuring that employees at risk of leaving are identified more effectively.

---

# Future Improvements

* Hyperparameter tuning using GridSearchCV
* Feature selection
* Cross-validation
* SMOTE for class balancing
* Model deployment with Flask or FastAPI
* Docker containerization
* CI/CD pipeline
* Cloud deployment (AWS, Azure, or GCP)

---

# Learning Outcomes

This project demonstrates practical experience with:

* Data Cleaning
* Exploratory Data Analysis
* Feature Engineering
* Data Visualization
* Classification Algorithms
* Model Evaluation
* Handling Imbalanced Datasets
* End-to-End Machine Learning Workflow

---

# Installation

```bash
git clone https://github.com/yourusername/Employee-Attrition-Prediction.git

cd Employee-Attrition-Prediction

pip install -r requirements.txt
```

---

# Run the Project

```bash
jupyter notebook
```

Open the notebook and run all cells sequentially.

---

# License

This project is intended for educational and portfolio purposes.
