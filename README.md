# ECommerce-DataAnalysis
🛒 This project analyzes e-commerce transaction data using pandas. It covers data cleaning, customer trends, sales insights, and RFM analysis. Ideal for learning real-world data analysis with Python and visualizing business metrics.

---

## 📘 Project Overview

**Project Title**: E-Commerce Data Analysis  
**Level**: Beginner to Intermediate  
**Tool**: Jupyter Notebook  
**Libraries Used**: `pandas`,`numpy`

This notebook demonstrates how to clean, explore, and analyze a dataset from an online retail platform. It focuses on identifying trends, high-value customers, revenue patterns, and potential areas for business improvement.

---

## 🎯 Objectives

1. Load and preprocess raw e-commerce data.
2. Analyze customer orders and purchasing trends.
3. Perform RFM (Recency, Frequency, Monetary) analysis.
4. Visualize sales patterns across products, categories, and time.
5. Identify KPIs such as top customers, total revenue, and return rates.

---

## 🏗️ Project Structure (Q&A Format)

---

### ❓ Q1: Display the top 10 rows of the dataset

```python
df.head(10)
```

✅ **Explanation**:  
The `.head(10)` function shows the first 10 rows in the dataset. This helps you preview the structure and values in each column.

---

### ❓ Q2: Display the last 10 rows of the dataset

```python
df.tail(10)
```

✅ **Explanation**:  
`.tail(10)` returns the last 10 rows. It’s useful to check how data entries look toward the end (sometimes includes nulls or strange entries).

---

### ❓ Q3: What is the shape of the dataset?

```python
df.shape
```

✅ **Explanation**:  
This returns a tuple with `(rows, columns)`. You’ll know how many data entries and features are present in the dataset.

---

### ❓ Q4: Show dataset info (column types, non-null counts)

```python
df.info()
```

✅ **Explanation**:  
`.info()` provides data types, memory usage, and how many non-null values are in each column — useful for spotting nulls or bad formats.

---

### ❓ Q5: Check for null values in the dataset

```python
df.isnull().sum()
```

✅ **Explanation**:  
This shows how many missing (null) values each column has. Helps decide whether to clean or drop certain columns.

---

### ❓ Q6: Drop columns `notes`, `agency`, and `status`

```python
df.drop(['notes', 'agency', 'status'], axis=1, inplace=True)
```

✅ **Explanation**:  
These columns are dropped because they’re either not useful for analysis or contain redundant info. `inplace=True` applies the change directly to `df`.

---

### ❓ Q7: Show basic statistics for numerical columns

```python
df.describe()
```

✅ **Explanation**:  
`.describe()` gives statistics like mean, median, standard deviation, min, and max for numeric columns — good for getting quick insights.

---

### ❓ Q8: Which employee name occurs the most in the dataset?

```python
df['employee_name'].value_counts().head(1)
```

✅ **Explanation**:  
`.value_counts()` counts how often each name appears. This shows the most frequent employee name (often due to duplicate entries or popular roles).

---

### ❓ Q9: How many unique job titles are there?

```python
df['job_title'].nunique()
```

✅ **Explanation**:  
`.nunique()` tells how many distinct job titles exist in the dataset. Useful for understanding job diversity.

---
