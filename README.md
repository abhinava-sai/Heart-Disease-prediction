# Heart Disease Classification: An End-to-End Machine Learning Project

[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg?style=flat-square&logo=python&logoColor=white)](https://www.python.org/downloads/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=flat-square&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=flat-square&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Numpy](https://img.shields.io/badge/numpy-%23013243.svg?style=flat-square&logo=numpy&logoColor=white)](https://numpy.org/)

This repository contains an end-to-end data science framework for predicting the presence of heart disease in patients based on clinical parameters. It covers the full lifecycle of a machine learning project: data exploration, feature engineering, model training, hyperparameter tuning, and evaluation.

---

## 🔍 Problem Statement
Given a set of clinical parameters about a patient, can we predict whether or not they have heart disease? This is a **binary classification** problem where:
* `1` = Heart Disease present
* `0` = No Heart Disease

## 📊 Data Overview
The project utilizes the **UCI Heart Disease Dataset**, which includes 14 key clinical attributes, such as:
* **Age, Sex**
* **cp:** Chest pain type
* **trestbps:** Resting blood pressure
* **chol:** Serum cholestoral in mg/dl
* **fbs:** Fasting blood sugar > 120 mg/dl
* **restecg:** Resting electrocardiographic results
* **thalach:** Maximum heart rate achieved
* **exang:** Exercise induced angina
* **target:** The predicted attribute (1 or 0)

---

## 🏗 Project Workflow

The implementation follows a structured "Data Science Blueprint":

1.  **Exploratory Data Analysis (EDA):** Visualizing distributions, correlations, and target imbalances using `Matplotlib` and `Seaborn`.
2.  **Data Preprocessing:** Handling missing values (if any), feature scaling, and train-test splitting.
3.  **Model Selection:** Training and comparing three fundamental classifiers:
    * **Logistic Regression**
    * **K-Nearest Neighbors (KNN)**
    * **Random Forest Classifier**
4.  **Hyperparameter Tuning:** Optimizing model performance using `RandomizedSearchCV` and `GridSearchCV`.
5.  **Evaluation:** Assessing models beyond simple accuracy using:
    * Confusion Matrix
    * Precision, Recall, and F1-score
    * ROC Curve and AUC (Area Under Curve)
6.  **Feature Importance:** Identifying which clinical factors (e.g., chest pain type, max heart rate) are the strongest predictors of heart disease.

---

## 🛠 Tech Stack

| Category | Technology |
| :--- | :--- |
| **Language** | Python 3.9+ |
| **Data Manipulation** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Machine Learning** | Scikit-Learn |
| **Environment** | Jupyter Notebook |

---

## 🚀 Key Features

* **Visual Correlation Matrix:** Insightful heatmaps showing how clinical features relate to one another.
* **Model Comparison:** A side-by-side performance analysis of different algorithms to select the most robust predictor.
* **Automated Evaluation:** Customized functions to plot ROC curves and generate detailed classification reports.
* **Interpretability:** Feature importance analysis to explain *why* a model made a specific prediction, enhancing clinical trust.

---

## 📁 Project Structure

```text
Heart-Disease-Classification/
├── heart.csv                            # Raw dataset
├── HeartDiseaseTrain-Test.csv           # Train/test split data
├── end-to-end-heart-disease-classification.ipynb  # Main project notebook
├── README.md                            # Project documentation
└── .gitignore
