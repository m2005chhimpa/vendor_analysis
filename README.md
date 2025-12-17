# vendor_analysis

# Vendor Performance & Profitability Analysis

## 📊 Project Overview
This project analyzes vendor-related data to evaluate purchase efficiency, sales performance, and profitability. It integrates inventory, purchase, sales, and invoice records to generate insights into vendor contribution, margins, and stock turnover.

## 📂 Dataset
The dataset consists of six tables:
- **begin_inventory**: Opening stock levels, prices, and start dates.
- **end_inventory**: Closing stock levels, prices, and end dates.
- **purchases**: Purchase orders with vendor details, costs, and quantities.
- **purchase_prices**: Vendor purchase prices vs. retail prices.
- **sales**: Sales transactions with excise tax and vendor mapping.
- **vendor_invoice**: Vendor invoices with freight costs and payment dates.

## 🛠️ Workflow
1. **Data Cleaning & Wrangling**
   - Merge purchases, sales, and invoices by VendorNumber.
   - Handle missing values and normalize vendor names.
   - Standardize date formats.

2. **Feature Engineering**
   - Calculate gross profit, profit margin, stock turnover, and sales-to-purchase ratio.
   - Aggregate freight costs per vendor.
   - Identify unsold inventory value.

3. **Exploratory Data Analysis**
   - Top vendors by sales contribution.
   - Vendor profitability vs. purchase contribution (Pareto analysis).
   - Freight cost impact on margins.
   - Brands with low sales but high margins.
   - Confidence intervals and t-tests for profit margin differences.

4. **Insights**
   - Highlight vendors driving >60% of purchases.
   - Identify vendors with locked capital in unsold inventory.
   - Recommend vendors/products for optimization.

## 📈 Visualizations
- Pareto chart of vendor purchase contribution.
- Donut chart of top 10 vendors vs. others.
- Scatter plot of sales vs. profit margin.
- Boxplot of unit purchase price by order size.
- Heatmap of correlation among profitability metrics.

## 🚀 Technologies Used
- Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy)
- Jupyter/Colab Notebooks
- SQLAlchemy (for saving results to SQLite)
- Power BI (for dashboarding)

## 📑 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/vendor-analysis.git
