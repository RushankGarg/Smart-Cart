# SmartCart Customer Segmentation using Machine Learning

A complete Machine Learning project that performs customer segmentation on SmartCart customers using **K-Means Clustering** and **Agglomerative Hierarchical Clustering**. The project includes data preprocessing, feature engineering, exploratory data analysis (EDA), dimensionality reduction using PCA, clustering evaluation, and customer profiling to help businesses understand customer behavior and design targeted marketing strategies.

---

## Project Overview

Customer segmentation enables businesses to identify groups of customers with similar characteristics and purchasing behavior. This project analyzes customer demographics, spending habits, and campaign responses to create meaningful customer segments using unsupervised machine learning techniques.

The project workflow includes:

- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Feature Encoding
- Feature Scaling
- Principal Component Analysis (PCA)
- K-Means Clustering
- Agglomerative Clustering
- Cluster Evaluation
- Customer Profiling

---

## Dataset

The dataset contains customer information including:

- Customer ID
- Year of Birth
- Education
- Marital Status
- Income
- Number of Children
- Customer Registration Date
- Product Spending
- Campaign Responses
- Purchase Channels
- Recency

---

## Project Workflow

### 1. Data Loading

- Load the customer dataset using Pandas.
- Explore dataset dimensions, data types, and missing values.

---

### 2. Data Preprocessing

- Handle missing values using median imputation.
- Convert date columns into datetime format.
- Remove unnecessary features.
- Detect and remove outliers in Age and Income.

---

### 3. Feature Engineering

The following features are created to improve customer analysis:

- **Age**
- **Customer Tenure**
- **Total Spending**
- **Total Children**
- Simplified Education Categories
- Simplified Marital Status

These engineered features provide a more meaningful representation of customer behavior.

---

### 4. Exploratory Data Analysis (EDA)

Data visualization is performed to understand relationships and distributions within the dataset.

Visualizations include:

- Correlation Heatmap
- Pair Plot
- Income Distribution
- Spending Distribution
- Cluster Visualizations

---

### 5. Feature Encoding

Categorical variables are transformed using **One-Hot Encoding**.

Encoded features include:

- Education
- Living Status

---

### 6. Feature Scaling

Numerical features are standardized using **StandardScaler** to ensure all features contribute equally during clustering.

---

### 7. Principal Component Analysis (PCA)

PCA is applied to reduce dimensionality while preserving most of the information.

Benefits include:

- Reduced dimensionality
- Faster clustering
- Improved visualization
- Reduced feature redundancy

---

### 8. Optimal Number of Clusters

Two methods are used to determine the optimal number of clusters:

#### Elbow Method

Uses Within-Cluster Sum of Squares (WCSS) to identify the optimal value of K.

#### Silhouette Score

Measures cluster quality by evaluating cohesion and separation.

---

### 9. Clustering Algorithms

#### K-Means Clustering

Partitions customers into distinct groups based on similarity.

#### Agglomerative Hierarchical Clustering

Creates hierarchical customer clusters using Ward linkage.

---

### 10. Cluster Analysis

Each customer is assigned to a cluster for further analysis.

Cluster profiling includes:

- Average Income
- Average Spending
- Age Distribution
- Customer Tenure
- Family Size

These insights help identify customer segments with different purchasing behaviors.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Kneed

---

## Required Libraries

```python
pandas
numpy
matplotlib
seaborn
scikit-learn
kneed
```

Install the required packages:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn kneed
```

---

## Machine Learning Techniques

- Missing Value Imputation
- Feature Engineering
- One-Hot Encoding
- Standard Scaling
- Principal Component Analysis (PCA)
- K-Means Clustering
- Agglomerative Clustering
- Elbow Method
- Silhouette Score
- Cluster Profiling

---

## Results

The clustering models successfully grouped customers into distinct segments based on demographic information and purchasing behavior.

These customer segments can be used to:

- Identify high-value customers
- Design personalized marketing campaigns
- Improve customer retention
- Optimize promotional strategies
- Support data-driven business decisions

---

## Project Structure

```
SmartCart/
│
├── SmartCart.ipynb
├── smartcart_customers.csv
├── README.md
└── requirements.txt
```

---

## How to Run

1. Clone the repository.

```bash
git clone https://github.com/yourusername/SmartCart-Customer-Segmentation.git
```

2. Navigate to the project directory.

```bash
cd SmartCart-Customer-Segmentation
```

3. Install the required dependencies.

```bash
pip install -r requirements.txt
```

4. Launch Jupyter Notebook.

```bash
jupyter notebook
```

5. Open **SmartCart.ipynb** and execute all notebook cells.

---
