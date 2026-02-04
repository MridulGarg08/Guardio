# 🛡️ Guardio — Credit Card Fraud Detection System

> Machine Learning system that detects fraudulent credit card transactions using advanced imbalanced data handling techniques such as **SMOTE**, improving the model’s ability to identify high-risk transactions.

---

## 🚀 Project Overview

Credit card fraud is a major challenge in the fintech industry due to:

- Extremely imbalanced datasets  
- Rapidly evolving fraud techniques  
- Need for real-time detection  
- High cost of false negatives  

This project applies data analysis, feature engineering, and machine learning techniques to build a reliable fraud detection model capable of identifying anomalous transaction patterns.

---

## 📊 Dataset

Due to GitHub file size restrictions, the dataset is not included in this repository.

👉 **Download it from Kaggle:**  
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

### Dataset Highlights:
- Transactions made by European cardholders  
- Highly imbalanced data (fraud cases are very rare)  
- Features anonymized using PCA for confidentiality  
- Key columns include:
  - `Time`
  - `Amount`
  - PCA-transformed features (`V1–V28`)
  - `Class` → Fraud (1) / Not Fraud (0)

---

## ⚙️ Tech Stack

- **Python**
- **NumPy & Pandas** → Data manipulation  
- **Matplotlib & Seaborn** → Data visualization  
- **Scikit-learn** → Model building and evaluation  
- **Imbalanced-learn** → SMOTE implementation  
- **Jupyter Notebook**

---

## 🔍 Project Workflow

### ✅ Data Preprocessing
- Checked for missing values and duplicates  
- Scaled transaction features for improved model performance  
- Prepared data for handling severe class imbalance  

### ✅ Exploratory Data Analysis
- Fraud vs Non-fraud distribution  
- Transaction amount behavior  
- Correlation analysis  
- Outlier detection  

### ✅ Handling Class Imbalance
The dataset contains a very small percentage of fraudulent transactions, which can bias models toward predicting non-fraud cases.

To address this, **SMOTE (Synthetic Minority Oversampling Technique)** was implemented to generate synthetic samples of the minority class, resulting in a more balanced training dataset and improved fraud detection capability.

### ✅ Model Building
Multiple classification algorithms were evaluated to identify the best-performing model:

- Logistic Regression  
- Decision Tree  
- Random Forest  

### ✅ Model Evaluation
Since accuracy is misleading for imbalanced datasets, the model was evaluated using:

- **Precision** → Measures correctness of fraud predictions  
- **Recall** → Critical for minimizing false negatives  
- **F1 Score** → Balances precision and recall  
- **ROC-AUC Score** → Evaluates overall classification performance  

**Primary Objective:**  
Maximize fraud detection while maintaining acceptable precision to reduce false alerts.

---

## 📊 Results

- Achieved **~92% recall** in detecting fraudulent transactions  
- Significantly reduced false negatives using SMOTE  
- Improved classification performance compared to baseline models  
- Built a robust pipeline for rare-event detection  

---

## 🧠 Key Machine Learning Concepts Applied

- Imbalanced Data Handling using SMOTE  
- Feature Scaling  
- Supervised Classification  
- Bias-Variance Tradeoff  
- Model Performance Optimization  

---

## 📈 Key Challenges Addressed

✔ Handling severe class imbalance  
✔ Avoiding model overfitting  
✔ Selecting appropriate evaluation metrics  
✔ Detecting rare events effectively  

---

## 🧠 Future Improvements

- Implement advanced boosting algorithms such as **XGBoost** and **LightGBM**  
- Deploy the model as a **real-time fraud detection API**  
- Build an interactive visualization dashboard  
- Integrate streaming transaction data for live detection  

---

## ▶️ How to Run the Project

```bash
# Clone the repository
git clone https://github.com/MridulGarg08/Guardio.git

# Navigate into the folder
cd Guardio

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook

👨‍💻 Author

Mridul Garg
Aspiring Data Scientist | Machine Learning Enthusiast
