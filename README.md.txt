# Diabetes Risk Stratification & Predictive Modeling

## 📌 Project Overview
This project analyzes patient health metrics to:
- Identify natural risk segments using K-Means clustering
- Predict diabetes using Logistic Regression
- Interpret key metabolic risk drivers
- Validate clinical alignment between unsupervised and supervised models

The objective is to demonstrate end-to-end healthcare analytics workflow including EDA, feature scaling, clustering, predictive modeling, and interpretation.

---

## 📊 Dataset
- Source: PIMA Indians Diabetes Dataset
- Observations: 768 patients
- Features:
  - Pregnancies
  - Glucose
  - BloodPressure
  - SkinThickness
  - Insulin
  - BMI
  - DiabetesPedigreeFunction
  - Age
- Target:
  - Outcome (0 = No Diabetes, 1 = Diabetes)

---

## 🔎 Exploratory Data Analysis
- Checked missing values and distributions
- Identified glucose and BMI as dominant risk factors
- Applied feature scaling using StandardScaler

---

## 🔬 Unsupervised Learning – K-Means Clustering
- Applied K-Means with 3 clusters
- PCA used for 2D visualization

### Cluster Insights:
| Cluster | Avg Glucose | Diabetes Rate |
|----------|------------|---------------|
| 0 | 141 mg/dL | 55% |
| 1 | 130 mg/dL | 51% |
| 2 | 106 mg/dL | 13% |

Cluster 0 identified as High Risk metabolic segment.

---

## 🤖 Supervised Learning – Logistic Regression
- Train/Test Split (80/20)
- Evaluated using Precision, Recall, F1-score

Key Focus:
- High recall for diabetic patients (healthcare critical metric)

---

## 📈 Model Performance
- Accuracy: ~74%
- Strong recall for diabetes class
- Glucose identified as strongest predictor

---

## 🧠 Key Insights
- Glucose is the most influential feature in diabetes prediction
- Clustering revealed clinically meaningful risk segments
- Unsupervised clusters aligned with actual diagnosis rates
- Demonstrates real-world healthcare risk stratification logic

---

## 🚀 Tools & Technologies
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

---

## 📌 Business Applications
- Preventive healthcare targeting
- Insurance risk scoring
- Public health intervention planning
- Early diabetes detection systems

---

## 📎 Future Improvements
- Hyperparameter tuning
- Cross-validation
- ROC-AUC optimization
- Deployment as a Streamlit web app
