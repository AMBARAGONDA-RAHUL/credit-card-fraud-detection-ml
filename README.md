
# 💳 Credit Card Fraud Detection — Machine Learning Project

![Python](https://img.shields.io/badge/Python-ML-yellow?style=for-the-badge&logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Modeling-orange?style=for-the-badge&logo=scikitlearn)
![Pandas](https://img.shields.io/badge/Pandas-EDA-blue?style=for-the-badge&logo=pandas)
![Project Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

---

## 📌 Introduction

This end-to-end machine learning project detects fraudulent credit card transactions using advanced analytics and classification algorithms. The focus is on solving a real-world, high-impact problem with class imbalance using Python, Scikit-learn, and domain-aware metrics like precision and recall.

### 🎯 **What You’ll Learn:**

✔ Protect users from financial loss  
✔ Prevent misuse of banking systems  
✔ Improve transaction trustworthiness in digital platforms  
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
````

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
[Open Step 1](credit-card-fraud-detection-ml/STEPS/step-1.md)

### ✅ Step 2: Load Dataset

Loads `creditcard.csv` and displays initial insights.
[Open Step 2](credit-card-fraud-detection-ml/STEPS/step-2.md)

### ✅ Step 3: Data Exploration

* Class distribution (fraud vs. valid)
* Amount analysis by class
* Correlation matrix heatmap
  [Open Step 3](credit-card-fraud-detection-ml/STEPS/step-3.md)

### ✅ Step 4: Data Preparation

* Separate features and target
* Train/test split (80/20)
  [Open Step 4](credit-card-fraud-detection-ml/STEPS/step-4.md)

### ✅ Step 5: Model Training

* **Random Forest Classifier**
* Fit on training set
* Predict on test set
  [Open Step 5](credit-card-fraud-detection-ml/STEPS/STEP-5.md)

### ✅ Step 6: Model Evaluation

* Accuracy
* Precision
* Recall
* F1-Score
* Matthews Correlation Coefficient (MCC)
* Confusion Matrix (Heatmap)
  [Open Step 6](credit-card-fraud-detection-ml/STEPS/step-6.md)

### ✅ Step 7: Building and Training the Model

* Train a Random Forest classifier on the training data to predict fraudulent transactions.
  [Open Step 7](credit-card-fraud-detection-ml/STEPS/step-7.md)

### ✅ Step 8: Evaluating the Model

* Evaluate the trained model using metrics like accuracy, precision, recall, F1-score, Matthews correlation coefficient, and confusion matrix.
  [Open Step 8](credit-card-fraud-detection-ml/STEPS/step-8.md)

### ✅ Step 9: Future Improvements

* Ideas for oversampling, advanced models, API deployment, and CI/CD automation.
  [Open Step 9](credit-card-fraud-detection-ml/STEPS/step-9.md)

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

