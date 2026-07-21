# 🏢 Employee Attrition Prediction using Machine Learning

## 📌 Project Overview

Employee attrition is one of the biggest challenges organizations face because replacing experienced employees is costly and time-consuming. This project applies supervised machine learning techniques to predict whether an employee is likely to leave the company based on demographic, job-related, and workplace factors.

The project demonstrates an end-to-end machine learning workflow, including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and performance comparison.

---

## 🎯 Business Problem

High employee turnover affects productivity, recruitment costs, and organizational performance.

The objective of this project is to build a predictive model that helps Human Resources (HR) identify employees at risk of leaving so that proactive retention strategies can be implemented.

---

## 📊 Dataset Information

The dataset contains employee demographic, professional, and workplace-related information.

### Target Variable

| Column        | Description                                       |
| ------------- | ------------------------------------------------- |
| **Attrition** | Whether an employee left the company (**Yes/No**) |

### Features

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

## 📂 Project Workflow

### 1️⃣ Data Understanding

* Loaded the dataset using Pandas
* Explored dataset dimensions
* Inspected data types
* Reviewed feature descriptions

---

### 2️⃣ Data Cleaning

Performed data quality checks including:

* Missing value detection
* Duplicate record detection
* Data consistency verification

**Results**

* ✅ No missing values
* ✅ No duplicate records

---

### 3️⃣ Exploratory Data Analysis (EDA)

Exploratory analysis was performed to understand employee behavior and identify factors associated with attrition.

The analyses include:

* Employee Attrition Distribution
* Department vs Attrition
* Overtime vs Attrition
* Monthly Income vs Attrition
* Age vs Attrition
* Work-Life Balance vs Attrition

**Key Observations**

* Employees working overtime showed higher attrition.
* Research & Development contained the largest workforce and the highest number of employees leaving.
* The dataset is imbalanced, with significantly more employees staying than leaving.

---

### 4️⃣ Data Preprocessing

### 4️⃣ Data Preprocessing

The dataset was prepared for machine learning by performing the following preprocessing steps:

- Removed non-informative features (`EmployeeCount`, `EmployeeNumber`, and `StandardHours`)
- Separated features (`X`) and target variable (`y`)
- Encoded the target variable using `LabelEncoder`
- Applied One-Hot Encoding to categorical features
- Split the dataset into training and testing sets using a stratified split (80/20)
- Standardized the feature values using `StandardScaler`

Status: ✅ Complete

---

### 5️⃣ Machine Learning Models

Multiple classification algorithms are trained and compared.


The first machine learning classification model has been implemented and evaluated.

**Completed**

- ✅ Logistic Regression

**Planned**

- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- XGBoost *(optional)*

Status: 🚧 In Progress
---

### 6️⃣ Model Evaluation

The Logistic Regression model was evaluated using multiple classification metrics.

**Evaluation Metrics**

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

**Initial Results**

- Accuracy: **86.05%**
- The model performs well in predicting employees who stay.
- The model achieves low recall for employees who leave, indicating that many attrition cases are missed.
- These results establish a baseline for comparing more advanced machine learning models.

Status: 🚧 In Progress

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

## 📁 Project Structure

```text
IBM-HR-Employee-Attrition/
│
├── data/
│   └── raw/
│       └── WA_Fn-UseC_-HR-Employee-Attrition.csv
│
├── notebooks/
│   ├── 01_data_understanding.ipynb
│   ├── 02_exploratory_data_analysis.ipynb
│   ├── 03_data_preprocessing.ipynb
│   └── 04_model_training_lr.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
│
└── LICENSE


```

## 📌 Current Progress

The following project stages have been completed:

- ✅ Data Understanding
- ✅ Exploratory Data Analysis (EDA)
- ✅ Data Preprocessing
- ✅ Logistic Regression Model Training
- ✅ Logistic Regression Model Evaluation

The next phase is to train and compare additional machine learning models to 



---

## 📈 Results

The first machine learning model, **Logistic Regression**, achieved an overall accuracy of **86.05%** on the test dataset.

Although the model performed well at predicting employees who remained with the company, it struggled to identify employees who were likely to leave because of the class imbalance in the dataset. The evaluation highlighted the importance of using metrics such as **Recall** and **F1-score**, rather than relying solely on accuracy.

The Logistic Regression model serves as the baseline for evaluating and comparing additional machine learning models in the next phase of the project.

---

## 🚀 Future Improvements

* Hyperparameter tuning using GridSearchCV
* Feature selection
* Cross-validation
* SMOTE for class balancing
* Model deployment with Flask or FastAPI
* Docker containerization
* CI/CD pipeline
* Cloud deployment (AWS, Azure, or GCP)

---

## 📚 Learning Outcomes

This project demonstrates practical experience with:

* Data Cleaning
* Exploratory Data Analysis
* Feature Engineering
* Data Visualization
* Classification Algorithms
* Model Evaluation
* Handling Imbalanced Datasets
* End-to-End Machine Learning Workflow
* Logistic Regression
* Classification Model Evaluation

---

## ⚙️ Installation

```bash
git clone https://github.com/yourusername/Employee-Attrition-Prediction.git

cd Employee-Attrition-Prediction

pip install -r requirements.txt
```

---

## ▶️ Run the Project

```bash
jupyter notebook
```

Open the notebook and run all cells sequentially.

---

## 📄 License

This project is intended for educational and portfolio purposes.
