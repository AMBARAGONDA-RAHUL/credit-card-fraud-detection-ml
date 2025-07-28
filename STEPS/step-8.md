
## 🧪 Step 8: Evaluating the Model

After training our Random Forest model, it's important to evaluate how well it performs—especially since fraud detection datasets are usually **imbalanced** (fraud cases are rare).

We use several metrics to get a full picture of the model’s effectiveness:

* **Accuracy**: Overall correctness of predictions.
* **Precision**: How many predicted frauds were actually fraud.
* **Recall**: How many real frauds did the model detect.
* **F1-Score**: Balance between precision and recall.
* **Matthews Correlation Coefficient (MCC)**: Balanced metric that works well with imbalanced datasets.

---

### Model Evaluation Code

```python
from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score, matthews_corrcoef, confusion_matrix
import matplotlib.pyplot as plt
import seaborn as sns

# Calculate metrics
accuracy = accuracy_score(yTest, yPred)
precision = precision_score(yTest, yPred)
recall = recall_score(yTest, yPred)
f1 = f1_score(yTest, yPred)
mcc = matthews_corrcoef(yTest, yPred)

# Print metrics
print("Model Evaluation Metrics:")
print(f"Accuracy: {accuracy:.4f}")
print(f"Precision: {precision:.4f}")
print(f"Recall: {recall:.4f}")
print(f"F1-Score: {f1:.4f}")
print(f"Matthews Correlation Coefficient: {mcc:.4f}")

# Plot confusion matrix heatmap
conf_matrix = confusion_matrix(yTest, yPred)
plt.figure(figsize=(8, 6))
sns.heatmap(conf_matrix, annot=True, fmt="d", cmap="Blues",
            xticklabels=['Normal', 'Fraud'], yticklabels=['Normal', 'Fraud'])
plt.title("Confusion Matrix")
plt.xlabel("Predicted Class")
plt.ylabel("True Class")
plt.show()
```

---

### What the Metrics Mean

| Metric                                       | Interpretation                                                                                                       |
| -------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| **Accuracy: 0.9996**                         | 99.96% of all predictions were correct. However, due to class imbalance, this metric alone can be misleading.        |
| **Precision: 0.9873**                        | When the model predicted fraud, it was correct 98.73% of the time — meaning very few false alarms (false positives). |
| **Recall: 0.7959**                           | The model detected 79.59% of all actual fraud cases — indicating some frauds were missed (false negatives).          |
| **F1-Score: 0.8814**                         | A balanced score combining precision and recall — shows the model performs well overall.                             |
| **Matthews Correlation Coefficient: 0.8863** | A balanced metric for imbalanced data. Near 1 means very strong, reliable predictions.                               |

