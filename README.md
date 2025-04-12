
## 🧠 Project Overview

Credit card fraud is a significant problem in financial services. With highly imbalanced data (very few fraud cases), building a robust classifier is challenging. This project addresses the problem by training a machine learning model and deploying it with a simple web UI.

## 📊 Dataset

- **Source**: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Size**: 284,807 transactions
- **Fraud Cases**: 492 (~0.17%)
- **Features**:
  - `Time`, `Amount`
  - `V1` to `V28`: PCA-transformed numerical features
  - `Class`: Target variable (0 = legit, 1 = fraud)

## 🛠 Technologies Used

- Python 3
- Pandas, NumPy
- Scikit-learn
- Flask
- Matplotlib, Seaborn
- Joblib (model serialization)

## 🔍 Key Steps

### 1. Data Preprocessing
- Loaded dataset and checked class imbalance
- Scaled `Amount` and `Time` features
- Split data into training and testing sets

### 2. Model Training
- Trained Logistic Regression classifier
- Evaluated using Accuracy, Precision, Recall, and F1 Score
- Saved model and label encoders using `joblib`

### 3. Web App Deployment
- Created a simple form-based interface using Flask
- Takes user input and returns fraud prediction

## ✅ How to Run

1. Run this command in your terminal -- 
streamlit run app.py
