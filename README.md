# 📊 Customer Churn Prediction – Telco Dataset

## Project Overview
Customer churn is a major problem for telecom companies. Losing customers directly impacts revenue and growth.

This project builds a **machine learning model to predict which customers are likely to churn**, enabling businesses to take proactive retention actions.

The complete workflow includes:
- Data cleaning
- Exploratory Data Analysis (EDA)
- Feature engineering
- Handling class imbalance (SMOTE)
- Model training
- Evaluation
- Model saving

---

## Objective
Predict whether a customer will **Churn (Yes/No)** based on:
- Demographics
- Account details
- Service usage
- Billing information

---

##  Dataset
**Telco Customer Churn Dataset**

Contains:
- 7000+ customers
- 21 features
- Target: `Churn`

Key features:
- tenure
- MonthlyCharges
- TotalCharges
- Contract type
- Payment method
- Internet services

---

##  Tech Stack

### Languages & Tools
- Python
- Google Colab
- GitHub

### Libraries
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- imbalanced-learn (SMOTE)
- Pickle

---

## Exploratory Data Analysis (EDA)

Performed:
✔ Histograms for numerical features  
✔ Boxplots for outlier detection  
✔ Correlation heatmap  
✔ Class distribution check  

Insights:
- Higher churn in month-to-month contracts
- High monthly charges increase churn risk
- Dataset is imbalanced

---

## Data Preprocessing

Steps:
- Handling missing values
- Label Encoding categorical variables
- Feature scaling (if applicable)
- Train-test split
- SMOTE for class imbalance

---

## Models Implemented
 Decision Tree : Baseline 
 Random Forest : Ensemble improvement 
 XGBoost : Boosting for higher accuracy 

---

##  Model Evaluation

Metrics used:
- Accuracy
- Confusion Matrix
- Classification Report (Precision, Recall, F1)
- Cross-validation

XGBoost provided the best performance.



##Model Saving
Trained model saved using:

```python
pickle.dump(model, open('model.pkl', 'wb'))
