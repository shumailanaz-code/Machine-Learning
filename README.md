# 💄 Cosmetic Sales Deal Size Classification using KNN and Decision Tree

## 📖 Project Overview

A cosmetic company is looking to boost its market value by offering value-based promotional deals. 
Each customer purchase qualifies for a **deal size (Small, Medium, or Large)** based solely on the **total value of the transaction**, not the product type.

The company has transaction data and wants to use it to:
- Analyze and classify current deal sizes
- Introduce additional deal types in the future
- Build a system to assist in **long-term promotional planning**

To address this, we use two **supervised machine learning classification algorithms**:
- **K-Nearest Neighbors (KNN)**
- **Decision Tree Classifier**

---

## 🗃️ Dataset Description

- **File Name**: `sales_data.csv`
- **Source**: Kaggle

### 🔹 Features

| Feature Name       | Data Type   | Description                                  |
|--------------------|-------------|----------------------------------------------|
| `Order_No`         | Numerical   | Unique ID for each order                     |
| `Qty_Ordered`      | Numerical   | Quantity of items ordered                    |
| `Price`            | Numerical   | Price per item                               |
| `Sales`            | Numerical   | Total transaction value                      |
| `Status`           | Categorical | Order status (e.g., shipped, pending)        |
| `Product_Line`     | Categorical | Category of product                          |
| `Product_Code`     | Categorical | Unique code of the product                   |
| `Deal_Size`        | Categorical | Label to classify: Small, Medium, or Large   |

> **Input Variables**: `Qty_Ordered`, `Price`, `Sales`  
> **Output Variable**: `Deal_Size` (Target for classification)

---

## 🧪 Approach

1. **Data Cleaning** — Handle missing values, standardize types
2. **Feature Selection** — Selected key input variables: Quantity Ordered, Price, Sales
3. **Encoding** — Converted categorical target variable to numeric
4. **Modeling**:
   - Trained **KNN Classifier** (tested different values of k)
   - Trained **Decision Tree Classifier**
5. **Evaluation**:
   - Compared accuracy, confusion matrix, and classification reports
6. **Visualization** — Plotted decision boundaries and feature importance

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**, **NumPy** — Data manipulation
- **Scikit-learn** — ML models and preprocessing
- **Matplotlib**, **Seaborn** — Visualization
- **Jupyter Notebook**

---

## 🚀 How to Run

1. Clone the repository or download the files.
2. Place the dataset `sales_data.csv` in the working directory.
3. Install required packages:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
4. Open the notebook (decisiontree_classification_ml.ipynb & KNN_classification_ml.ipynb)
5. Run all cells to train models and view evaluation metrics and plots.
---
