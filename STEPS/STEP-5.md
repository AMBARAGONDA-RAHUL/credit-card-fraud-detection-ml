
## 📊 Step 5: Plotting the Correlation Matrix

To better understand the relationships between variables, we compute and visualize the **correlation matrix** using a heatmap. This helps identify:

- Which features are highly correlated (positive or negative)
- Potential multicollinearity issues
- Relationships between **Amount**, **Time**, and anonymized features (`V1`–`V28`)

---

### 🧪 Code to Generate Correlation Matrix

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Compute the correlation matrix
corrmat = data.corr()

# Plot the heatmap
plt.figure(figsize=(12, 9))
sns.heatmap(corrmat, vmax=0.8, square=True, cmap='coolwarm')
plt.title("Correlation Matrix Heatmap", fontsize=16)
plt.tight_layout()
plt.show()
````

---

### 🖼️ Visual Snapshot

 <img width="901" height="782" alt="Image" src="https://github.com/user-attachments/assets/d1e4d3d2-4d32-40ba-8f57-f46d54c8f747" />

---

### 🧠 Key Observations

* Most features (like `V1`–`V28`) show **low correlation** with each other — which is expected since they were generated using **PCA** (Principal Component Analysis).
* A few features like **`V2`** and **`V5`** show a **negative correlation** with `Amount`, suggesting a potential relationship worth exploring in feature selection.
* The `Class` column (target) does not show strong direct correlations, emphasizing the complexity of identifying fraud and the need for machine learning.

---

### 📌 Why It Matters

* **Correlation analysis** helps detect **redundant features** or those that could **confuse models**.
* Helps in **feature selection**, **feature engineering**, and in understanding **data behavior** before modeling.
