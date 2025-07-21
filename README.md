PREDICTING HEART FAILURE OUTCOMES USING MACHINE LEARNING

📊 Project Overview

This project aims to develop and evaluate machine learning models to predict patient survival from heart failure using clinical data. Leveraging techniques from data preprocessing, exploratory data analysis (EDA), and various classification algorithms, we identify key risk factors and present a robust predictive model to support early intervention and personalized healthcare.

🎯 Objective

To build and compare supervised machine learning models for predicting DEATH_EVENT in heart failure patients.

To identify the most effective model and its performance metrics (Accuracy, F1-Score, ROC-AUC).

To extract insights into the most influential clinical features contributing to heart failure outcomes.

💾 Dataset

The project utilizes the Heart Failure Clinical Records Dataset, obtained from the UCI Machine Learning Repository.
This dataset contains 299 patient records with 13 clinical features and a binary target variable (DEATH_EVENT).

Key Features:

age: Patient's age (years)

ejection_fraction: Percentage of blood leaving the heart at each contraction (%)

serum_creatinine: Level of serum creatinine in the blood (mg/dL)

time: Follow-up period (days)

other clinical indicators (anaemia, creatinine_phosphokinase, diabetes, high_blood_pressure, platelets, serum_sodium, sex, smoking).

DEATH_EVENT: (Target) Binary outcome (0 = No Death Event, 1 = Death Event)

🛠️ Methodology

The project workflow encompassed the following stages:

Data Loading & Initial Inspection: Loaded heart_failure_clinical_records_dataset.csv and performed initial data quality checks.

Exploratory Data Analysis (EDA): Visualized feature distributions, correlations, and relationships with the target variable to gain insights.

Data Preprocessing: Handled scaling of numerical features and split data into training and testing sets.

Model Development: Implemented and trained various classification models, including:

Logistic Regression

K-Nearest Neighbors (KNN)

Decision Tree

Random Forest (Best Performer)

Support Vector Machine (SVM)

Gaussian Naive Bayes

Linear Discriminant Analysis (LDA)

Model Evaluation: Assessed model performance using accuracy, precision, recall, F1-score, and ROC-AUC metrics, reinforced by Stratified K-Fold Cross-Validation.

Feature Importance Analysis: Determined the most impactful features for prediction using the best-performing model.

✨ Results & Findings

Top Model: The Random Forest Classifier demonstrated superior performance compared to other models.

Overall Accuracy: Approximately 84%

ROC-AUC Score: 89.15% (indicating strong discriminative power)

Key Predictors: ejection_fraction, serum_creatinine, and age were identified as the most significant features influencing heart failure outcomes.

Performance Note: While overall accuracy was high, the model's recall for DEATH_EVENT (positive class) was lower (~63%), suggesting a need for further optimization on imbalanced data.

A detailed analysis, including model performance comparisons and visualizations, can be found in classification.ipynb and summarized in final.pptx.

🚀 How to Run Locally

To replicate and explore this project:

Clone the Repository:

Bash

git clone https://github.com/shyam16843/predicting-heart-failure-outcomes.git

cd predicting-heart-failure-outcomes


Install Dependencies:
It's highly recommended to use a virtual environment.

Bash

pip install pandas numpy matplotlib seaborn scikit-learn jupyter

Launch Jupyter Notebook:

Bash

jupyter notebook classification.ipynb
This will open the Jupyter interface in your browser, where you can run the analysis.

💻 Technologies Used

Python 3.x

Jupyter Notebook

Key Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

👥 Contributors

Akshay J P

Fahad Muhammed M

Ghanashyam T V

Jibin K

Mohammed Fahim P
