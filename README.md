
# 💳 Credit Card Fraud Detection — Machine Learning Project

![Python](https://img.shields.io/badge/Python-ML-yellow?style=for-the-badge\&logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Modeling-orange?style=for-the-badge\&logo=scikitlearn)
![Pandas](https://img.shields.io/badge/Pandas-EDA-blue?style=for-the-badge\&logo=pandas)
![Project Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

---

## 📌 Introduction

This project uses **Machine Learning** to detect fraudulent credit card transactions from anonymized data. The dataset is heavily imbalanced (very few fraud cases), so special attention is given to **precision, recall, and F1-score** rather than just accuracy.

### 🎯 **What You’ll Learn:**

✔ Perform Exploratory Data Analysis (EDA) with Python

✔ Handle imbalanced datasets for classification tasks

✔ Train and evaluate a Random Forest model

✔ Understand performance metrics like precision, recall, F1, MCC

✔ Visualize fraud detection results with heatmaps and statistics

---

## 🛠️ Tech Stack

* **Python** (Pandas, NumPy, Matplotlib, Seaborn)
* **Scikit-learn** (Random Forest, Model Evaluation)
* **Jupyter Notebook** for experimentation
* **Git** & **GitHub** for version control and sharing

---

## 📁 Project Structure

```bash
📦 credit-card-fraud-detection-ml
├── creditcard.csv
├── fraud_detection.ipynb
├── README.md
├── requirements.txt
└── screenshots/
    ├── data_head.png
    ├── heatmap.png
    ├── confusion_matrix.png
```

---

## 🚀 Steps to Run the Project

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/RAHUL-AMBARAGONDA/credit-card-fraud-detection-ml.git
cd credit-card-fraud-detection-ml
```

### 2️⃣ Install Requirements

```bash
pip install -r requirements.txt
```

### 3️⃣ Open the Notebook

```bash
jupyter notebook fraud_detection.ipynb
```

---

## 📊 Project Workflow

### ✅ Step 1: Import Libraries

Includes `pandas`, `matplotlib`, `seaborn`, `sklearn`, and `numpy`.

### ✅ Step 2: Load Dataset

Loads `creditcard.csv` and displays initial insights.

### ✅ Step 3: Data Exploration

* Class distribution (fraud vs. valid)
* Amount analysis by class
* Correlation matrix heatmap

### ✅ Step 4: Data Preparation

* Separate features and target
* Train/test split (80/20)

### ✅ Step 5: Model Training

* **Random Forest Classifier**
* Fit on training set
* Predict on test set

### ✅ Step 6: Model Evaluation

* Accuracy
* Precision
* Recall
* F1-Score
* Matthews Correlation Coefficient (MCC)
* Confusion Matrix (Heatmap)

---

## 📈 Sample Output

| Metric    | Value  |
| --------- | ------ |
| Accuracy  | 99.96% |
| Precision | 98.73% |
| Recall    | 79.59% |
| F1-Score  | 88.14% |
| MCC       | 0.88   |

Confusion Matrix:

![Confusion Matrix](screenshots/confusion_matrix.png)

---

## ⚡ Future Improvements

* Use **SMOTE / Oversampling** for class imbalance
* Try **XGBoost** or **LightGBM**
* Deploy as an API using **Flask** or **FastAPI**
* Automate pipeline with **MLflow** and **CI/CD**

---

## 📌 Dataset Source

[Credit Card Fraud Detection Dataset – Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud)

---

## 🧠 Author

Made with ❤️ by **Rahul Ambaragonda**
🔗 [LinkedIn](https://linkedin.com/in/rahulambaragonda) • [GitHub](https://github.com/RAHUL-AMBARAGONDA) • [Blog](https://hashnode.com/@rahulambaragonda)

---

Let me know if you'd like a matching `requirements.txt` or help converting this into a `.py` script for production deployment.

---

## 👨‍💻 Author  
📌 Rahul – | Azure & DevOps Engineer 
🔗 [LinkedIn](https://www.linkedin.com/in/Rahul-Ambaragonda) | 

🚀 **Happy Terraforming!** 🏗️🔥
