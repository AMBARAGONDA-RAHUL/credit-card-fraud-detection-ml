## 🧹 Step 6: Preparing the Data

Before building our machine learning model, we need to **separate features and labels**, and then **split the dataset** into training and testing sets.

---

### 🎯 Purpose of This Step

- Organize data for supervised learning
- Ensure fair evaluation using **training vs. test data**
- Convert data into the format required by ML models (NumPy arrays)

---

### 🧪 Code to Prepare the Data

```python
# Separate features and target
X = data.drop(['Class'], axis=1)   # Input features
Y = data["Class"]                  # Target label

# Check shapes
print(X.shape)   # (284807, 30)
print(Y.shape)   # (284807,)

# Convert to NumPy arrays for faster computation
xData = X.values
yData = Y.values

# Train-test split: 80% train, 20% test
from sklearn.model_selection import train_test_split

xTrain, xTest, yTrain, yTest = train_test_split(
    xData, yData, test_size=0.2, random_state=42
)
````

---

### 🧾 Output Snapshot

```
(284807, 30)
(284807,)
```

This tells us:

* We have **284,807 rows** and **30 input features**
* The target array (`Class`) has the same number of rows

---

### 📌 Why `train_test_split` is Important

* Ensures that the model **does not memorize** the data
* Helps us **evaluate generalization** to new, unseen transactions
* `random_state=42` ensures **reproducibility** — consistent results every run

---

### 🧠 Key Takeaways

* Always split your dataset before training to prevent **data leakage**
* Converting to NumPy arrays (`.values`) is often more efficient for ML libraries
* You can apply **scaling** or **SMOTE oversampling** on `xTrain` later before modeling

```
