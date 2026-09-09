# Students Pass Prediction ML

A machine learning project that predicts whether a student is likely to pass or fail an exam based on different academic, personal, and environmental factors.

## 📌 Project Overview

The goal of this project is to understand how machine learning can be used for a binary classification problem.

Instead of predicting a continuous exam score, the project transforms the exam score into a binary outcome:

- **1 → Pass**
- **0 → Fail**

The project uses Logistic Regression to learn patterns from student-related features and predict the final class.

## 📊 Dataset

The dataset contains information about students, including factors such as:

- Hours Studied
- Attendance
- Previous Scores
- Sleep Hours
- Tutoring Sessions
- Physical Activity
- Parental Involvement
- Access to Resources
- Motivation Level
- Family Income
- Teacher Quality
- School Type
- Peer Influence
- Learning Disabilities
- Parental Education Level
- Distance from Home
- Gender
- And other student-related attributes

The `Exam_Score` column is used to create the target variable for the classification task.

## 🔍 Exploratory Data Analysis

The project begins with Exploratory Data Analysis (EDA) to understand the dataset before training the model.

This includes examining:

- Dataset structure and data types
- Missing values
- Basic statistics
- Feature distributions
- Relationships between numerical features
- Correlations with exam performance
- Visual patterns in the data

Graphs and visualizations are used to better understand how different factors relate to student performance.

## ⚙️ Feature Engineering

A new binary target variable called `Pass` is created from `Exam_Score`.

Students scoring **70 or above** are classified as Pass, while students scoring below 70 are classified as Fail.

The original `Exam_Score` is then excluded from the model features to prevent data leakage, since it was directly used to create the target.

## 🤖 Machine Learning

The first model is a Logistic Regression classifier.

A baseline model is trained using selected numerical features such as:

- Hours Studied
- Attendance
- Previous Scores
- Sleep Hours

The baseline model achieved an accuracy of **88.65%** on the test set.

## 📈 Model Evaluation

The model is evaluated using more than just accuracy.

The project examines:

- Confusion Matrix
- Precision
- Recall
- F1-score
- Predicted probabilities

This helps determine not only how accurate the model is, but also what types of mistakes it makes.

The baseline model achieved:

- **Accuracy:** 88.65%
- **Pass Precision:** 0.83
- **Pass Recall:** 0.70
- **Pass F1-score:** 0.76

The confusion matrix showed that the model was better at identifying students who fail than students who pass.

## 🚀 Further Improvements

The next stage of the project focuses on improving the baseline model by using more information from the dataset.

This includes:

- Handling missing values
- Encoding categorical features
- Scaling numerical features
- Using preprocessing pipelines
- Training an improved Logistic Regression model
- Comparing the improved model with the baseline

The purpose is to understand how proper preprocessing and feature selection can affect model performance.

## 🧠 What I Learned

Through this project, I practiced the complete basic machine learning workflow:

**Data → EDA → Feature Engineering → Preprocessing → Model Training → Prediction → Evaluation → Model Comparison**

The project also helped me understand how Logistic Regression works internally, including probabilities, the sigmoid function, decision thresholds, loss, and gradient descent.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## 📁 Project Structure

The repository contains the Jupyter Notebook with the complete analysis and machine learning workflow, along with the supporting project files.

## 🎯 Project Goal

This project is part of my journey toward building a stronger foundation in Machine Learning and Data Science by learning concepts through practical, project-based implementation.
