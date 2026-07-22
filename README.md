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

Multiple supervised machine learning classification algorithms were trained and evaluated using the preprocessed dataset.

**Completed Models**

- ✅ Logistic Regression
- ✅ Decision Tree
- ✅ Random Forest
- ✅ Support Vector Machine (SVM)
- ✅ K-Nearest Neighbors (KNN)

**Planned**

- Hyperparameter Tuning
- Model Optimization
- Final Model Selection
- XGBoost *(optional)*

Status: 🚧 In Progress
---

### 6️⃣ Model Evaluation

Each machine learning model was evaluated using multiple classification metrics.

**Evaluation Metrics**

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

Since the dataset is imbalanced, model performance was evaluated using Recall and F1-score in addition to Accuracy.

Status: ✅ Completed

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
│   ├── 04_model_training_lr.ipynb
|   ├── 05_decision_tree.ipynb
|   ├── 06_random_forest.ipynb
|   ├── 07_support_vector_machine.ipynb
|   ├── 08_knn.ipynb
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
- ✅ Data Cleaning
- ✅ Exploratory Data Analysis (EDA)
- ✅ Data Preprocessing
- ✅ Logistic Regression
- ✅ Decision Tree
- ✅ Random Forest
- ✅ Support Vector Machine (SVM)
- ✅ K-Nearest Neighbors (KNN)

The next phase of the project is to compare the trained models, perform hyperparameter tuning, improve model performance, and select the best model for employee attrition prediction.



---

## 📈 Results

Five supervised machine learning classification models have been trained and evaluated.

| Model | Accuracy |
|--------|---------:|
| Logistic Regression | **86.05%** |
| Decision Tree | 75.85% |
| Random Forest | 83.33% |
| Support Vector Machine (SVM) | **86.73%** |
| K-Nearest Neighbors (KNN) | 84.69% |

Although Support Vector Machine achieved the highest overall accuracy, Logistic Regression provided the best balance between Accuracy, Precision, Recall, and F1-score for predicting employee attrition.

Since the dataset is imbalanced, Recall and F1-score were considered alongside Accuracy when evaluating model performance.

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

## 📚 Learning Outcomes

This project demonstrates practical experience with:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Visualization
- Data Preprocessing
- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Classification Model Evaluation
- Handling Imbalanced Datasets
- End-to-End Machine Learning Workflow

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
