# 🛒 E-Commerce Sales Analysis

A complete **E-Commerce Sales Analysis project using Python and Pandas**, built on the **USA Sales Product Dataset**. The notebook focuses on cleaning real-world sales data, transforming columns, performing business-oriented analysis, and extracting insights about products, cities, time periods, and customer orders.

## 📊 Dataset

**USA Sales Product Dataset**  
Kaggle: https://www.kaggle.com/datasets/kushagra1211/usa-sales-product-datasetcleaned

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
```

- Extracted additional date features:
  - Month
  - Day
  - Year

- Converted order time into four time ranges:
  - Morning
  - Afternoon
  - Evening
  - Night

### 3. Sales & Revenue Analysis

The notebook calculates and analyzes:

- **Total Revenue**
- **Best-selling products** based on quantity sold
- **Top 10 best-selling products**
- **Top product types** based on quantity sold
- **Product revenue** to identify products generating the highest revenue
- **Average selling price** of each product

### 4. City-wise Analysis

Analyzed sales performance across cities by finding:

- Cities with the highest number of products sold
- Cities generating the highest revenue
- Product popularity across different cities using `City × Product` analysis

### 5. Monthly & Daily Sales Analysis

Used the extracted date features to analyze sales over time:

- Monthly quantity sold
- Best-performing month
- Monthly sales across different years
- Monthly revenue
- Top-performing days based on quantity sold
- Highest-revenue days

### 6. Time-based Sales Analysis

Converted order times into broader periods and analyzed the quantity of products sold during:

**Morning → Afternoon → Evening → Night**

This helps identify which part of the day has the highest sales activity.

### 7. Average Order Value (AOV)

Calculated **Average Order Value** using:

```text
AOV = Total Revenue / Number of Unique Orders
```

This measures the average amount spent per order.

The notebook also analyzes how many products customers purchase within individual orders using `Order ID` and `Quantity Ordered`.

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**

## 📁 Project Files

```text
E-Commerce-Sales-Analysis/
│
├── E_Commerce_Sales_Analysis.ipynb
└── README.md
```

## ▶️ How to Run

1. Open `E_Commerce_Sales_Analysis.ipynb` in **Google Colab** or **Jupyter Notebook**.
2. Download the dataset from Kaggle.
3. Place/provide the required CSV file in the notebook environment.
4. Run the notebook cells from top to bottom.

## 🎯 Learning Focus

This project is designed as a **Pandas practice and data-analysis project**, covering practical operations such as data cleaning, type conversion, feature creation, `groupby()`, aggregation, sorting, date-time analysis, and business-oriented sales analysis.
