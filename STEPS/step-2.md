
## Step 2: Loading the Data

In this step, we load the credit card fraud dataset into a pandas DataFrame and take a first look at its structure. This allows us to understand the data we will be working with throughout the project.

### Dataset Overview

- The dataset contains **284,807** transactions with **31 features**.
- Key features include:

  - **Time**: Number of seconds elapsed since the first transaction in the dataset.
  - **V1 – V28**: Anonymized features generated using Principal Component Analysis (PCA) to protect sensitive information.
  - **Amount**: The transaction amount in dollars.
  - **Class**: The target variable —  
    - `0` = Normal transaction  
    - `1` = Fraudulent transaction

### Code to Load and Preview the Dataset

```python
import pandas as pd

# Load dataset into pandas DataFrame
data = pd.read_csv("creditcard.csv")

# Display the first 5 rows to preview the data
print(data.head())
````

### Visual Preview of the Data

![Dataset Preview](https://github.com/user-attachments/assets/7e46dd11-5f6b-4912-931e-b3097d23ba0c)

```

---

### Explanation:
- The image is **after the code block** with a descriptive heading.
- The image will render nicely under the code snippet on GitHub.
- Make sure your image URL is correct and accessible.

---

If you want me to help format more steps or add extra details, just let me know!
```

