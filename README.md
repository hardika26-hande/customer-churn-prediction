
# Customer Churn Prediction

## Project Overview
This project uses Machine Learning to predict whether a telecom customer is likely to leave the service (churn).

It includes data exploration, preprocessing, model training, evaluation, and an interactive Streamlit application.

## Dataset
The project uses the Telco Customer Churn dataset, containing customer demographics, services, account information, and churn status.

## Technologies Used
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Streamlit
- Joblib
- Jupyter Notebook

## Machine Learning Models
Three models were evaluated:
- Logistic Regression
- Random Forest
- Decision Tree

A balanced Logistic Regression model was selected for the Streamlit app because it detects more customers likely to churn.

## Model Performance

| Model | Accuracy | Churn Recall |
|---|---:|---:|
| Logistic Regression | 80.55% | 55.88% |
| Balanced Logistic Regression | 73.81% | 78.34% |

The balanced model improves churn detection, although it may produce more false alarms.

## Project Structure

```text
customer-churn-prediction/
├── data/
│   └── raw/
├── models/
│   ├── customer_churn_model.pkl
│   ├── feature_importance.csv
│   └── model_comparison.csv
├── 01_data_exploration.ipynb
├── app.py
├── requirements.txt
├── .gitignore
└── README.md
