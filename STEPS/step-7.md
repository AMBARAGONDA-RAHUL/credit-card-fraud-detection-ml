
## 🧠 Step 7: Building and Training the Model

In this step, we teach the computer to recognize fraud by using a machine learning algorithm called **Random Forest**.

---

### What is Random Forest?

- It’s like asking many decision trees to vote on whether a transaction is fraud or not.
- This method is good because it reduces mistakes that a single tree might make.
- It works well even when the data has many features and is complicated.
- It helps us catch tricky fraud patterns.

---

### How We Train the Model

1. **Create the model:** We make a new Random Forest classifier.
2. **Train the model:** We give the model our training data (features and labels) so it can learn patterns.
3. **Make predictions:** We ask the model to predict fraud for new, unseen data (test data).

---

### Code to Build and Train the Model

```python
from sklearn.ensemble import RandomForestClassifier

# Step 1: Create the model
rfc = RandomForestClassifier()

# Step 2: Train the model using training data
rfc.fit(xTrain, yTrain)

# Step 3: Predict fraud on test data
yPred = rfc.predict(xTest)
````

---

### What Does This Code Do?

* `RandomForestClassifier()` — sets up the random forest model.
* `fit(xTrain, yTrain)` — the model learns from the training data.
* `predict(xTest)` — the model guesses if each test transaction is fraud or not.

---
