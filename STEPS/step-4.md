## 💰 Step 4: Exploring Transaction Amounts

In this step, we analyze the **transaction amount** to understand how monetary values differ between **fraudulent** and **valid** transactions.

### 🎯 Why This Matters

Understanding transaction amounts gives insight into:
- Whether fraudsters tend to target **high-value transactions**
- How different the amount distributions are between fraud and non-fraud cases
- Whether **amount** can be a useful feature for modeling or risk scoring

### 📊 Code to Explore Amount Distributions

```python
import matplotlib.pyplot as plt
import seaborn as sns

# Create separate datasets
fraud = data[data['Class'] == 1]
valid = data[data['Class'] == 0]

# Plot distribution of transaction amounts
plt.figure(figsize=(14,6))

# Valid transactions
sns.histplot(valid['Amount'], bins=100, color='green', label='Valid', kde=False, stat="density")

# Fraudulent transactions
sns.histplot(fraud['Amount'], bins=100, color='red', label='Fraudulent', kde=False, stat="density")

plt.title('Transaction Amount Distribution: Fraud vs Valid')
plt.xlabel('Transaction Amount')
plt.ylabel('Density')
plt.legend()
plt.grid(True)
plt.show()
 🔍 Summary Statistics for Fraudulent Transactions
print("Amount details of the fraudulent transaction")
fraud.Amount.describe()
````
<img width="444" height="430" alt="Image" src="https://github.com/user-attachments/assets/8f8bde77-1229-4801-9445-7e52e3a5235e" />
### OUTPUT
```python
print("details of valid transaction")
valid.Amount.describe()
````
<img width="283" height="432" alt="Image" src="https://github.com/user-attachments/assets/5c42145a-0dca-4391-b6d1-fdea7397c344" />
