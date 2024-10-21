# Diabetes-Machine-Learning-Project
Project for the exam "Machine Learning"

This project focuses on building and evaluating machine learning models to classify individuals as diabetic (1) or non-diabetic (0) based on clinical data. The dataset includes key medical variables, and several machine learning techniques are applied, including Decision Trees, Neural Networks, and Support Vector Machines (SVMs).

Table of Contents:

Overview

Dataset

Models

Decision Tree

Neural Network

Support Vector Machine (SVM)

Results

# Overview

The goal of this project is to create a robust classifier that accurately distinguishes diabetic patients from non-diabetic individuals using clinical data. Several models are developed and evaluated, including decision trees, neural networks, and SVMs. The dataset is balanced through oversampling and undersampling techniques to ensure improved model performance.

Dataset:
The dataset focuses on key clinical variables for diabetes classification, including:

Gender: The biological sex of the individual.

Age: Age of the individual, ranging from 0 to 80 years.

Hypertension: Presence or absence of hypertension (0 or 1).

Heart Disease: Presence or absence of heart disease (0 or 1).

Smoking History: Smoking habits with five categories.

BMI: Body Mass Index, ranging from 10.16 to 71.55.

HbA1c Level: Average blood sugar levels over the past 2-3 months.

Blood Glucose Level: Blood glucose concentration at a specific point in time.

Diabetes: Target variable, with 1 indicating diabetes and 0 indicating non-diabetes.

# Models

Decision Tree:

The Decision Tree classifier was used as the first model. After initial fitting, hyperparameter tuning was performed using Cross-Validated Cost-Complexity Pruning (CCP Alpha) and Grid Search to find the optimal configuration.

Neural Network:

The Neural Network was designed with multiple layers. The architecture includes 7 input neurons, 5 hidden neurons, and an output layer with 2 neurons. The model was trained for 20 epochs based on the performance observed during training.

Support Vector Machine (SVM):

The SVM model was implemented with a radial basis function (RBF) kernel. Hyperparameter tuning was performed using a Grid Search, leading to the selection of an optimal Slack variable (C) and kernel.

# Results

Decision Tree: Achieved good performance after pruning and tuning, avoiding overfitting with a final accuracy of 85%.

Neural Network: Final accuracy of 85%, with a test loss of 0.222 and 91% sensitivity for detecting true positives.

SVM: The best model, achieving an AUC of 0.89 and high accuracy of 84.7% in classifying diabetic individuals.
