## 🧮 Step 3: Analyzing Class Distribution

The next step is to **understand the distribution of classes** in the dataset — specifically, how many transactions are fraudulent compared to valid ones.

### 🎯 Why It Matters

Fraud detection is a **highly imbalanced classification problem**. Out of 284,807 transactions:
- Only a tiny fraction are fraudulent (`Class = 1`)
- The vast majority are valid (`Class = 0`)

If we don’t address this imbalance, a model could predict all transactions as valid and still get >99% accuracy — but completely fail at catching fraud.

### 🧪 Code to Analyze Class Distribution

```python
# Count the number of valid and fraud transactions
fraud = data[data['Class'] == 1]
valid = data[data['Class'] == 0]

# Calculate outlier fraction
outlier_fraction = len(fraud) / float(len(valid))

print(f"Fraudulent Transactions: {len(fraud)}")
print(f"Valid Transactions     : {len(valid)}")
print(f"Outlier Fraction       : {outlier_fraction:.6f}")

📊 Output Example
Fraudulent Transactions: 492  
Valid Transactions     : 284315  
Outlier Fraction       : 0.001732
