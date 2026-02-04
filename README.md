# 🛡️ Guardio — Credit Card Fraud Detection System

> Machine Learning system that detects fraudulent credit card transactions using advanced imbalanced data handling techniques such as SMOTE.


## 🚀 Project Overview

Credit card fraud is a major challenge in the fintech industry due to:

Extremely imbalanced datasets

Rapidly evolving fraud techniques

Need for real-time detection

High cost of false negatives

This project applies data analysis, feature engineering, and machine learning techniques to build a reliable fraud detection model.

## 📊 Dataset

Due to GitHub file size restrictions, the dataset is not included in this repository.

👉 Download it from Kaggle:
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

Dataset Highlights:

Transactions made by European cardholders

Highly imbalanced data (fraud cases are very rare)

Features are anonymized using PCA for confidentiality

Includes:

Time

Amount

PCA-transformed features (V1–V28)

Class → Fraud (1) / Not Fraud (0)

## ⚙️ Tech Stack

Python

NumPy & Pandas → Data manipulation

Matplotlib & Seaborn → Visualization

Scikit-learn → Model building & evaluation

Jupyter Notebook

🔍 Project Workflow
✅ Data Preprocessing

Checked for missing values and duplicates

Handled extreme class imbalance

Scaled transaction features for better model performance

✅ Exploratory Data Analysis

- Fraud vs Non-fraud distribution
- Transaction amount patterns
- Correlation analysis
- Outlier detection

✅ Model Building

### ✅ Handling Class Imbalance

The dataset is highly imbalanced, with fraudulent transactions representing a very small percentage of the total data.

To address this issue, **SMOTE (Synthetic Minority Oversampling Technique)** was implemented to generate synthetic samples of the minority class, resulting in a more balanced training dataset and improved model performance.


✅ Model Evaluation

### ✅ Model Evaluation

Since accuracy is not a reliable metric for imbalanced datasets, the model was evaluated using:

- Precision → Measures correctness of fraud predictions  
- Recall → Critical for fraud detection to minimize false negatives  
- F1 Score → Balances precision and recall  
- ROC-AUC Score → Evaluates overall classification performance  

**Focus:** Maximizing recall while maintaining acceptable precision to ensure fraudulent transactions are not missed.

Primary Goal:
👉 Maximize fraud detection while minimizing false alarms.

## 🧠 Key Machine Learning Concepts Applied

- Imbalanced Data Handling using SMOTE  
- Feature Scaling  
- Supervised Classification  
- Bias-Variance Consideration  
- Model Performance Optimization  

📈 Key Challenges Addressed

✔  Handling severe class imbalance using SMOTE 
✔ Avoiding overfitting
✔ Selecting the right evaluation metrics
✔ Detecting rare events effectively

🧠 Future Improvements

Try XGBoost / LightGBM
Deploy as a real-time fraud detection API
Build an interactive dashboard
Integrate streaming data detection

## ▶️ How to Run the Project

```bash
git clone https://github.com/MridulGarg08/Guardio.git
cd Guardio
pip install -r requirements.txt
jupyter notebook
```
## 📊 Results

- Achieved **94% recall** in detecting fraudulent transactions  
- Reduced false negatives significantly using SMOTE  
- Improved classification performance compared to baseline models 
💡 Why This Project Matters

Fraud detection systems are widely used in:

Banking
Payment gateways
E-commerce
Insurance

This project demonstrates practical machine learning skills applied to a real-world financial problem.

👨‍💻 Author
Mridul Garg
Aspiring Data Scientist | Machine Learning Enthusiast
