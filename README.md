# Retail Sales Analysis

An end-to-end data analysis project on a retail sales dataset, covering data cleaning, exploratory data analysis (EDA), visualizations, and a simple sales prediction model.

## Project Overview

This project analyzes retail order data across multiple regions, product categories, and time periods to uncover sales trends, profitability patterns, and top-performing products. The goal is to apply core data science skills — cleaning, analysis, visualization, and prediction — to a real-world style retail dataset.

## Dataset

The dataset (`data/retail_sales_dataset.csv`) contains retail order records with the following fields:

- **Order Info:** Order ID, Order Date, Ship Date, Ship Mode
- **Customer Info:** Customer ID, Segment
- **Location:** Region, State, City
- **Product Info:** Category, Sub-Category, Product Name
- **Metrics:** Quantity, Discount, Sales, Profit

## Project Workflow

1. **Data Loading & Exploration** — Loaded the dataset with Pandas and inspected structure, data types, and summary statistics.
2. **Data Cleaning** — Handled missing values in the `Discount` column, removed duplicate rows, and converted date columns to proper datetime format.
3. **Exploratory Data Analysis (EDA)** — Visualized:
   - Category-wise total sales
   - Month-wise sales trend
   - Region-wise total profit
   - Top 5 best-selling products
4. **Prediction Model** — Built a simple Linear Regression model to predict `Sales` based on `Quantity` and `Discount`.
5. **Insights & Conclusion** — Summarized key findings and business recommendations based on the analysis.

## Key Insights

- **Technology** generates the highest total sales, followed by **Furniture**.
- Sales show clear seasonal variation across months.
- The **West** region is the most profitable; the **North** region has the lowest profit.
- **Desktop Copier**, **Shipping Labels**, and **All-in-One Printer** are the top-selling products by quantity.

## Tools & Libraries

- Python 3
- Pandas, NumPy — data manipulation
- Matplotlib, Seaborn — visualization
- Scikit-learn — prediction model
- Jupyter Notebook

## Project Structure

```
retail-sales-project/
│
├── data/
│   └── retail_sales_dataset.csv
├── notebooks/
│   └── analysis.ipynb
├── outputs/
│   └── (saved charts, if any)
└── README.md
```

## How to Run

1. Clone this repository
   ```
   git clone <your-repo-url>
   cd retail-sales-project
   ```
2. Create a virtual environment and install dependencies
   ```
   python -m venv venv
   venv\Scripts\activate      # Windows
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```
3. Open `notebooks/analysis.ipynb` in VS Code or Jupyter and run all cells.

## Future Improvements

- Include additional features (Category, Region, Segment) in the prediction model to improve accuracy.
- Try more advanced models (Random Forest, XGBoost) for better sales forecasting.
- Add customer segmentation analysis using clustering techniques.
