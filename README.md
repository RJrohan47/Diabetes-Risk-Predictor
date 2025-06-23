# 🩺 Diabetes Prediction System

A **machine learning-based predictive analysis tool** that helps in identifying the likelihood of diabetes in patients using clinical features from the **Pima Indian Diabetes dataset**. This project walks through the complete **ML pipeline** including data preprocessing, EDA, model training, evaluation, and deployment readiness.

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Tech Stack](#tech-stack)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Preprocessing](#data-preprocessing)
- [Model Building](#model-building)
- [Evaluation Metrics](#evaluation-metrics)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Future Work](#future-work)
- [License](#license)

---

## 📖 Project Overview

This project aims to build a **binary classification model** to predict whether a patient has diabetes based on diagnostic measurements. It applies **data science principles** such as data cleaning, EDA, statistical imputation, outlier detection, feature selection, and model evaluation.

---

## 📊 Dataset Description

The dataset contains several **medical predictors** and one **target variable**, `Outcome` (0 or 1). Key features include:

- **Pregnancies**: Number of times pregnant  
- **Glucose**: Plasma glucose concentration  
- **BloodPressure**: Diastolic blood pressure (mm Hg)  
- **SkinThickness**: Triceps skin fold thickness (mm)  
- **Insulin**: 2-Hour serum insulin (mu U/ml)  
- **BMI**: Body mass index (weight in kg/(height in m)^2)  
- **DiabetesPedigreeFunction**: Function that scores likelihood of diabetes based on family history  
- **Age**: Age in years  
- **Outcome**: Class variable (`0` = no diabetes, `1` = diabetes)

---

## 🛠️ Tech Stack

- **Language**: Python  
- **Data Analysis**: `pandas`, `numpy`  
- **Visualization**: `matplotlib`, `seaborn`  
- **Machine Learning**: `scikit-learn`  
- **Notebook Environment**: Jupyter Notebook  

---

## 📈 Exploratory Data Analysis

- **Correlation heatmap** to visualize feature relationships  
- **Distribution plots** to assess data symmetry and outlier presence  
- **Descriptive statistics** to summarize central tendency, dispersion, and shape  
- **Box plots** for visual outlier detection  

---

## 🧹 Data Preprocessing

- **Missing Value Analysis**: No null values found  
- **Outlier Detection**: Applied IQR method  
- **Data Imputation**:  
  - **Mean** for symmetric distributions  
  - **Median** for skewed distributions (robust to outliers)  
- **Feature Scaling**: Used `StandardScaler` for standardization  

---

## 🧠 Model Building

- **Model Used**: Logistic Regression  
- **Data Split**: Train-Test split (typically 80/20)  
- **Pipeline**: Preprocessing → Model Training → Prediction  

---

## 📏 Evaluation Metrics

- **Accuracy**  
- **Recall**  
- **Precision**  
- **Confusion Matrix**  
- **ROC-AUC Curve**

📌 **Model Performance**:
- **Accuracy**: ~78%  
- **Recall**: ~84%  
> _High recall indicates strong ability to detect diabetic patients, which is critical in healthcare._

---

## 📊 Results

- The model performs well with **strong recall**.
- **Top correlated features**: Glucose, BMI, Age.

---

## 🚀 Installation

```bash
git clone https://github.com/yourusername/diabetes-prediction.git
cd diabetes-prediction
pip install -r requirements.txt
