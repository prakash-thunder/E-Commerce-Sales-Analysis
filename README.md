# 🛒 E-Commerce Sales Analysis

A complete **E-Commerce Sales Analysis project using Python and Pandas**, built on the **USA Sales Product Dataset**. The notebook focuses on cleaning real-world sales data, transforming columns, performing business-oriented analysis, and extracting insights about products, cities, time periods, and customer orders.

## 📊 Dataset

**USA Sales Product Dataset**  
Kaggle: [https://www.kaggle.com/datasets/kushagra1211/usa-sales-product-datasetcleaned](https://www.kaggle.com/datasets/kushagra1211/usa-sales-product-datasetcleaned)

The dataset contains sales information such as:

- Order ID
- Product
- Product Type
- Quantity Ordered
- Price
- Order Date
- Time
- City
- Purchase Address

## 🔍 What This Project Covers

### 1. Data Loading & Exploration

- Loaded the sales dataset using **Pandas**.
- Inspected the dataset using `head()`, `info()`, `describe()`, and `unique()`.
- Checked the structure and data types of the columns.
- Removed missing values using `dropna()`.

### 2. Data Cleaning & Transformation

- Converted the `Price` column from string/object format to numeric values by removing commas.
- Converted `Order Date` into Pandas datetime format.
- Created a new **Amount** column:

```text
Amount = Quantity Ordered × Price
