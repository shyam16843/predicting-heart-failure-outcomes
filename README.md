\# PREDICTING HEART FAILURE OUTCOMES USING MACHINE LEARNING



\## 📊 Project Overview

Machine learning system that predicts patient survival from heart failure with \*\*84% accuracy\*\* using clinical data. Identifies key risk factors through comprehensive EDA and model interpretation.



\## 🎯 Objective

\- Predict `DEATH\_EVENT` occurrence

\- Compare 7 classification models

\- Identify top clinical risk factors



\## 💾 Dataset

\*\*Source:\*\* 📂 \[UCI Heart Failure Clinical Records](https://archive.ics.uci.edu/ml/datasets/Heart+failure+clinical+records) 

\*\*Records:\*\* 299 patients | \*\*Features:\*\* 13 clinical indicators  



\*\*Key Features:\*\*  

`age` • `ejection\_fraction` • `serum\_creatinine` • `time` • `anaemia`



\## 🛠️ Methodology

```mermaid

graph TD

&nbsp;   A\[Data Cleaning] --> B\[EDA]

&nbsp;   B --> C\[Feature Engineering]

&nbsp;   C --> D\[Model Training]

&nbsp;   D --> E\[Performance Evaluation]

✨ Results

Model Performance (Random Forest)

Metric	Score

Accuracy	84%

ROC-AUC	0.891

Recall	63%

Top 3 Predictors:



Ejection Fraction (27% importance)



Serum Creatinine (22% importance)



Age (19% importance)



🚀 Installation

Clone repository:



bash

git clone https://github.com/shyam16843/predicting-heart-failure-outcomes.git

cd predicting-heart-failure-outcomes

Create virtual environment:



bash

python -m venv venv

source venv/bin/activate  # Linux/Mac

\# OR

venv\\Scripts\\activate  # Windows

Install dependencies:



bash

pip install -r requirements.txt

Run Jupyter Notebook:



bash

jupyter notebook classification.ipynb

💻 Technologies

🖥️ Python 3.8+ |

📦 Pandas |

🧮 NumPy |

📊 Matplotlib |

🎨 Seaborn |

🔬 Scikit-learn |

📓 Jupyter



🔮 Future Work

Class Imbalance Solutions



Implement SMOTE/ADASYN techniques



Model Optimization



Bayesian hyperparameter tuning



Clinical Integration



Develop Flask API endpoint

