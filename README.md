# PREDICTING HEART FAILURE OUTCOMES USING MACHINE LEARNING

## 📊 Project Overview
Machine learning system predicting heart failure survival with **84% accuracy** using clinical data. Identifies key risk factors through comprehensive analysis.

## 🎯 Objective
- Predict `DEATH_EVENT` occurrence
- Compare multiple classification models
- Identify top clinical risk factors

## 💾 Dataset
📂 [UCI Heart Failure Clinical Records](https://archive.ics.uci.edu/ml/datasets/Heart+failure+clinical+records)  
**Records:** 299 patients | **Features:** 13 clinical indicators  

**Key Features:**  
`age` • `ejection_fraction` • `serum_creatinine` • `time` • `anaemia`

## 🛠️ Methodology
```mermaid
graph TD
    A[Data Cleaning] --> B[EDA]
    B --> C[Feature Engineering]
    C --> D[Model Training]
    D --> E[Performance Evaluation]
🤖 Models Implemented
Traditional ML:
Random Forest (Best: 84% Accuracy)

Logistic Regression

SVM

K-Nearest Neighbors

Decision Trees

Gaussian Naive Bayes

LDA

Deep Learning:
Neural Network (3-layer MLP)

RNN (Experimental)

CNN (Future Work)

✨ Results
Performance Comparison
Model	Accuracy	ROC-AUC	Recall
Random Forest	84%	0.891	63%
Logistic Regression	82%	0.865	61%
SVM	81%	0.852	59%
Neural Network	79%	0.831	57%
Top 3 Predictors:

Ejection Fraction (27%)

Serum Creatinine (22%)

Age (19%)

🚀 Installation
bash
git clone https://github.com/shyam16843/predicting-heart-failure-outcomes.git
cd predicting-heart-failure-outcomes
python -m venv venv
source venv/bin/activate  # Linux/Mac
pip install -r requirements.txt
jupyter notebook classification.ipynb
💻 Technologies
🖥️ Python 3.8+ | 📦 Pandas | 🧮 NumPy | 📊 Matplotlib | 🎨 Seaborn | 🔬 Scikit-learn | 📓 Jupyter

🔮 Future Work
Class Imbalance - SMOTE/ADASYN

Model Tuning - Bayesian Optimization

Deployment - Flask API

Advanced Models - Transformers