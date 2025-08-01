
# PREDICTING HEART FAILURE OUTCOMES USING MACHINE LEARNING

## 📊 Project Overview
Machine learning system predicting heart failure survival with **84% accuracy** using clinical data. Identifies key risk factors through comprehensive analysis.

## 🎯 Objective
- Predict `DEATH_EVENT` occurrence
- Compare multiple classification models
- Identify top clinical risk factors

## 💾 Dataset
**Source:** [UCI Heart Failure Clinical Records](https://archive.ics.uci.edu/ml/datasets/Heart+failure+clinical+records)  
**Records:** 299 patients | **Features:** 13 clinical indicators  

**Key Features:**  
`age` • `ejection_fraction` • `serum_creatinine` • `time` • `anaemia`

## 🛠️ Methodology
1. Data Cleaning → EDA
2. EDA → Feature Engineering
3. Feature Engineering → Model Training
4. Model Training → Performance Evaluation

## 🤖 Models Implemented
### Traditional ML:
- Random Forest (Best: 84% Accuracy)
- Logistic Regression
- SVM
- K-Nearest Neighbors
- Decision Trees
- Gaussian Naive Bayes
- LDA

### Deep Learning:
- Neural Network (3-layer MLP)
- RNN (Experimental)
- CNN (Future Work)

## ✨ Results
### Performance Comparison
| Model              | Accuracy | ROC-AUC | Recall |
|--------------------|----------|---------|--------|
| Random Forest      | 84%      | 0.891   | 63%    |
| Logistic Regression| 82%      | 0.865   | 61%    |
| SVM                | 81%      | 0.852   | 59%    |
| Neural Network     | 79%      | 0.831   | 57%    |

**Top 3 Predictors:**  
1. Ejection Fraction (27%)  
2. Serum Creatinine (22%)  
3. Age (19%)

## 🚀 Installation
```bash
git clone https://github.com/shyam16843/predicting-heart-failure-outcomes.git
cd predicting-heart-failure-outcomes
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate  
pip install -r requirements.txt
jupyter notebook classification.ipynb 
```

## 💻 Technologies  

[🖥️ Python 3.8+](https://www.python.org) | 
[📦 Pandas](https://pandas.pydata.org) | 
[🧮 NumPy](https://numpy.org) |  
[📊 Matplotlib](https://matplotlib.org) | 
[🎨 Seaborn](https://seaborn.pydata.org) |  
[🔬 Scikit-learn](https://scikit-learn.org) | 
[📓 Jupyter](https://jupyter.org)

🔮 Future Work

Class Imbalance - SMOTE/ADASYN

Model Tuning - Bayesian Optimization

Deployment - Flask API

Advanced Models - Transformers