# ARTI308-Lab11  
# Credit Card Customer Segmentation

## About the Project

This project uses machine learning to group credit card customers into different segments based on their financial behavior. The main goal is to understand customer patterns and help businesses improve their marketing strategies and customer retention.

The project applies **K-Means Clustering**, which is an unsupervised machine learning algorithm used to divide customers into meaningful groups.

---

## Project Goal

The main goals of this project are to:

- Analyze customer financial behavior
- Group similar customers together
- Identify different customer segments
- Support better business and marketing decisions

---

## Dataset Description

The dataset contains credit card customer information related to spending, payments, and account activity.

### Main Features

Some of the important features in the dataset are:

- Balance
- Purchases
- Cash Advance
- Credit Limit
- Payments
- Purchase Frequency
- Cash Advance Frequency
- Tenure

### Dataset Size

- Rows: 8950
- Columns: 18

---

## Tools and Libraries

The following tools and libraries were used in this project:

| Tool / Library | Purpose |
|---|---|
| Python | Programming language |
| Pandas | Data loading and analysis |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Machine learning and clustering |

---

## Project Workflow

### Step 1: Load the Data

The dataset was loaded using **Pandas** to begin the analysis.

### Step 2: Clean the Data

The data was prepared by:

- Removing the `CUST_ID` column
- Checking for missing values
- Filling missing values using the mean

### Step 3: Explore the Data

Exploratory Data Analysis was performed to better understand the dataset.

This included:

- Viewing dataset information
- Checking statistical summaries
- Creating histograms
- Creating a correlation heatmap
- Studying relationships between important features

### Step 4: Scale the Features

Since clustering is affected by feature values, the data was normalized using **StandardScaler**. This step helps ensure that all features contribute equally to the clustering process.

### Step 5: Apply K-Means Clustering

K-Means clustering was used to group customers into different segments based on their financial behavior.

The best number of clusters was selected using:

- Elbow Method
- Silhouette Score

The selected number of clusters was:

```text
K = 3
