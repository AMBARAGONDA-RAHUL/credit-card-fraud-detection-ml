
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

### Now, let's explore more about the dataset using df.describe() method.
```python
print(data.describe())
````
 
| Word      | What it means                                                                                       |
| --------- | --------------------------------------------------------------------------------------------------- |
| **count** | How many people gave an answer (number of values in the column)                                     |
| **mean**  | The average — if we added all the numbers and divided by how many there are                         |
| **std**   | Are the numbers close to the average or jumping all around? This tells us how “spread out” they are |
| **min**   | The smallest number in the column                                                                   |
| **25%**   | A small number where 25% of values are even smaller than this (bottom quarter)                      |
| **50%**   | The middle number (half above, half below) — also called **median**                                 |
| **75%**   | A number where 75% of the data is smaller — only 25% are bigger                                     |
| **max**   | The biggest number in the column                                                                    |


<img width="1000" height="297" alt="Image" src="https://github.com/user-attachments/assets/39aec91b-3c6f-4727-8acc-54d9e40122f3" />
