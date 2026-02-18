# Diabetes-Prediction
# Diabetes Prediction 🩺

## Project Overview
This project is part of the **Machine Learning Foundations Capstone** for the *AI Programmer / ML Foundations* course.  
The goal of this project is to build a **Logistic Regression classification model** that predicts whether a patient has diabetes based on diagnostic medical measurements.

---

## Objective
To develop a machine learning model that can:
- Analyze patient health data
- Predict diabetes outcome (0 = No Diabetes, 1 = Diabetes)
- Evaluate performance using standard classification metrics

---

## Dataset
The dataset used is:

**Indian Diabetes Dataset (50K records with missing values)**  
File: `Indian_Diabetes_Dataset_50K_MissingValues.csv`

### Features
| Feature | Description |
|--------|-------------|
| Pregnancies | Number of times pregnant |
| Glucose | Plasma glucose concentration |
| BloodPressure | Diastolic blood pressure (mm Hg) |
| SkinThickness | Triceps skin fold thickness (mm) |
| Insulin | 2-Hour serum insulin (mu U/ml) |
| BMI | Body Mass Index |
| DiabetesPedigreeFunction | Diabetes family history |
| Age | Age of the patient |
| Outcome | Target variable (0 or 1) |

---

## Tools & Libraries
The following Python libraries were used:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

---

## Project Workflow

### 1. Data Loading
The dataset is loaded using pandas and basic inspection is performed using:
- `.head()`
- `.info()`
- `.describe()`

### 2. Exploratory Data Analysis (EDA)
- Distribution plots for **Glucose** and **BMI**
- Count plot for **Outcome**
- Class balance analysis

### 3. Missing Data Handling
Missing values in the following columns were handled using **median imputation**:
- Glucose  
- BloodPressure  
- SkinThickness  
- Insulin  
- BMI  

This approach is robust and suitable for medical datasets.

### 4. Feature Scaling
All features were standardized using **StandardScaler** to improve model performance.

### 5. Model Training
A **Logistic Regression** model was trained using:
- 70% training data
- 30% testing data

### 6. Model Evaluation
The model was evaluated using:
- Confusion Matrix
- Accuracy
- Precision
- Recall
- F1 Score
- ROC Curve
- AUC Score

---

## Results
The model achieved strong predictive performance with a good balance between precision and recall.  
The ROC curve and AUC score indicate that the model can effectively distinguish between diabetic and non-diabetic patients.

---

## Key Insights
- **Glucose and BMI** are the most influential features.
- Logistic Regression performs well for binary medical classification problems.
- Feature scaling significantly improves model stability.
- ROC-AUC confirms good generalization.
