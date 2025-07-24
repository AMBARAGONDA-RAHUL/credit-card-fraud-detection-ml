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
![Image](https://github.com/user-attachments/assets/7e46dd11-5f6b-4912-931e-b3097d23ba0c)
### Code to Load and Preview the Dataset

```python
import pandas as pd

# Load dataset into pandas DataFrame
data = pd.read_csv("creditcard.csv")

# Display the first 5 rows to preview the data
print(data.head())
