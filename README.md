# Cafe-sales-EDA
# ☕ Café Sales Data Cleaning & Exploratory Data Analysis (EDA)

A data science project focused on cleaning messy café sales data, performing exploratory data analysis (EDA), and discovering meaningful business insights using Python.

## 📌 Project Overview

This project transforms raw café sales data into a clean, structured dataset suitable for analysis. It addresses missing values, incorrect data types, inconsistent entries, and duplicate records before exploring sales performance, customer payment preferences, and revenue trends.

## 🎯 Objectives

- Clean and preprocess real-world-style sales data.
- Handle missing values and incorrect entries.
- Perform exploratory data analysis using statistical summaries and visualizations.
- Identify top revenue-generating products.
- Analyze customer payment methods and order locations.
- Explore monthly and weekday sales trends.
- Understand relationships between quantity, price, and total spending.

## 📂 Dataset Information

- **Original records:** 10,000
- **Records retained after cleaning:** 9,031
- **Menu items:** 8
- **Payment methods:** Cash, Credit Card, Digital Wallet

**Key columns:** Transaction ID, Item, Quantity, Price Per Unit, Total Spent, Payment Method, Location, and Transaction Date.

## 🧹 Data Cleaning Process

1. Replaced `"ERROR"` and `"UNKNOWN"` placeholders with proper missing values (`NaN`).
2. Converted numerical columns and transaction dates to appropriate data types.
3. Recovered missing numerical values wherever possible using:

   `Total Spent = Quantity × Price Per Unit`

4. Removed rows with missing item names when the product could not be identified.
5. Removed exact duplicate records and performed final data-quality checks.
6. Exported the cleaned dataset separately to preserve the original data.

## 📊 Exploratory Data Analysis

The project uses visualizations to investigate:

- **Item popularity:** Comparing order counts across café products.
- **Revenue by item:** Identifying products that generate the most revenue.
- **Payment preferences:** Comparing Cash, Credit Card, and Digital Wallet usage.
- **Order locations:** Analyzing In-store versus Takeaway orders.
- **Spending patterns:** Examining quantity, price, and total spending distributions.
- **Time-based trends:** Comparing monthly and weekday revenue.
- **Correlation analysis:** Understanding relationships between numerical variables.

## 💡 Key Insights

- **Revenue differs from order volume:** Salad, Sandwich, and Smoothie generate the highest revenue, while Cookie and Tea generate the lowest, despite relatively similar order counts.
- **Payment preferences are balanced:** Cash, Credit Card, and Digital Wallet are used at approximately equal rates.
- **In-store orders have a slightly higher average spend:** $9.10 compared with $8.79 for Takeaway.
- **Sales remain relatively stable:** Monthly and weekday revenue show no major sustained fluctuations.
- **Spending follows expected relationships:** Total spending increases with quantity and unit price, while quantity and price have almost no correlation.
- **Data quality matters:** Cleaning inconsistent values and recovering information improves the reliability of subsequent analysis.

## 🛠️ Tools & Technologies

- **Python** — data analysis and preprocessing
- **Pandas** — data manipulation and cleaning
- **NumPy** — numerical operations
- **Matplotlib** — data visualization
- **Seaborn** — statistical visualization
- **Jupyter Notebook** — interactive analysis and documentation

## 🚀 Business Recommendations

- Make payment method and order location mandatory fields during checkout.
- Promote lower-revenue products through combinations with popular, high-revenue items.
- Encourage larger takeaway orders through relevant add-on suggestions.
- Maintain flexible availability of all payment methods.
- Standardize the data-cleaning workflow for future sales datasets.

## 📁 Project Structure

```text
Cafe-Sales-EDA/
├── cafe_sales_eda.ipynb
├── dirty_cafe_sales.csv
├── cleaned_cafe_sales.csv
├── cafe_sales_presentation.pptx
└── README.md
```

*Update filenames and include only the files actually present in your repository.*

## ▶️ How to Run

1. Clone or download the repository.
2. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. Place the dataset in the appropriate project directory.
4. Open the notebook using Jupyter:

   ```bash
   jupyter notebook
   ```

5. Run the notebook cells sequentially to reproduce the cleaning process, visualizations, and analysis.

## 📌 Conclusion

This project demonstrates a complete data analysis workflow, from handling messy raw data to extracting actionable business insights. It highlights the importance of data quality, exploratory visualization, and statistical relationships in supporting informed business decisions.

**Domain:** Data Science & Analytics  
**Project Type:** Data Cleaning and Exploratory Data Analysis  
**Author:** Onkar Sonne
