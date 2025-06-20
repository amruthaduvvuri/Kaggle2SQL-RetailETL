
# 🔄 Retail Orders ETL & SQL Analytics Project

This project is an **end-to-end ETL (Extract, Transform, Load)** pipeline built using Python and MySQL. It automates the process of extracting a retail dataset via Kaggle API, transforming it using `pandas`, and loading it into a MySQL database. Post-load, business-critical SQL queries are executed to derive key insights.

---

## 📦 Dataset

- **Source:** [Retail Orders Dataset on Kaggle](https://www.kaggle.com/datasets/ankitbansal06/retail-orders)
- **Accessed via:** Kaggle API
- **File used:** `orders.csv`

---

## 🧰 Tools & Technologies

| Stage      | Tool / Technology               |
|------------|---------------------------------|
| Extract    | Kaggle API                      |
| Transform  | Python (`pandas`, `numpy`)      |
| Load       | SQLAlchemy + PyMySQL → MySQL    |
| Analysis   | MySQL Workbench + SQL queries   |
| Interface  | Jupyter Notebook (`.ipynb`)     |
| Versioning | Git & GitHub                    |

---


## 🔄 ETL Flow Diagram
<img width="958" alt="Screenshot 2025-06-20 at 11 31 54 PM" src="https://github.com/user-attachments/assets/cd506b7a-d739-41bd-ba43-3028aa1d435a" />

## 🚀 ETL Process Overview

### ✅ 1. Extract
- Used Kaggle API to programmatically download the dataset  
- Unzipped and loaded `orders.csv` into a pandas DataFrame

### ✅ 2. Transform
- Cleaned missing or invalid values  
- Converted data types (dates, floats, etc.)  
- Derived useful features (e.g., year, month from `order_date`)

### ✅ 3. Load
- Connected to MySQL using SQLAlchemy + PyMySQL  
- Loaded transformed DataFrame into a table (`df_orders`)  
- Verified the load with basic sanity queries

## 📊 Business Questions Answered

-  **Top 10 highest revenue-generating products**

-  **Top 5 highest selling products in each region**

-  **Month-over-month growth comparison for 2022 and 2023 sales**  
  *(e.g., Jan 2022 vs Jan 2023, Feb 2022 vs Feb 2023, etc.)*

- **For each category, identify the month with the highest sales**

-  **Which sub-category had the highest growth in profit in 2023 compared to 2022**
