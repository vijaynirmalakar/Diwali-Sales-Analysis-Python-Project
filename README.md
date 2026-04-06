# Diwali Sales Analysis — Python EDA Project
> Performed exploratory data analysis on 11,239 Diwali sales orders (₹10.6 Cr revenue) using Python to uncover customer demographics, regional trends, and top-performing product categories.

---

## Problem
A retail business running Diwali season sales had no clear picture of:
- Who their actual buyers are (gender, age group, marital status, occupation)
- Which states and regions generate the most revenue and orders
- Which product categories dominate sales during the festive season

This project answers all three questions through a structured EDA using Python.

---

## Dataset
- **Source:** Diwali Sales internal transaction data
- **Size:** 11,251 rows | 15 columns (11,239 after cleaning)
- **Fields:** User ID, Customer Name, Product ID, Gender, Age Group, Age, Marital Status, State, Zone, Occupation, Product Category, Orders, Amount

---

## Tools & Libraries
`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn` `Jupyter Notebook`

---

## Process

1. **Data Loading** — Imported CSV with unicode_escape encoding; confirmed 11,251 rows × 15 columns
2. **Data Cleaning** — Dropped 2 fully empty columns (Status, unnamed1); removed 12 null rows from Amount column; converted Amount dtype from float64 to int64
3. **EDA — Gender Analysis** — Countplot + grouped bar chart (Amount by Gender)
4. **EDA — Age Group Analysis** — Countplot with gender hue; bar chart of Amount by Age Group
5. **EDA — State-wise Analysis** — Top 10 states by Orders; Top 5 states by Amount
6. **EDA — Marital Status** — Countplot; grouped analysis by Marital Status × Gender
7. **EDA — Occupation Analysis** — Order count and revenue by occupation
8. **EDA — Product Category** — Top categories by count and revenue; Top 10 products by orders

---

## Key Findings

- **Women drive 70% of total revenue** — ₹7.43 Cr vs ₹3.19 Cr for men — and place significantly more orders
- **Age group 26–35 is the dominant buyer segment** — 11,395 orders (40.7% of all orders), far ahead of the 36–45 group (5,687 orders)
- **Uttar Pradesh is the #1 state** with ₹1.94 Cr in revenue and 4,807 orders — followed by Maharashtra (₹1.44 Cr) and Karnataka (₹1.35 Cr)
- **Food is the top product category** at ₹3.39 Cr (32% of revenue) — ahead of Clothing & Apparel (₹1.65 Cr) and Electronics & Gadgets (₹1.56 Cr)
- **IT Sector buyers spend the most** — ₹1.48 Cr in total purchases, followed by Healthcare (₹1.30 Cr) and Aviation (₹1.26 Cr)
- **Unmarried women are the highest-spending segment** — ₹4.38 Cr — nearly double the spend of married men

---

## Business Recommendations

1. Target women aged 26–35 with personalized Diwali campaigns — they are the single most valuable customer segment
2. Focus inventory and promotions on Food, Clothing, and Electronics — these 3 categories = 62% of total revenue
3. Concentrate marketing spend in Uttar Pradesh, Maharashtra, and Karnataka — top 3 states contribute ₹4.73 Cr combined
4. Build occupation-specific offers for IT Sector and Healthcare professionals — highest average spend per buyer
5. Create unmarried women-targeted bundles — the highest-spending demographic in the dataset

---

## Project Structure
```
diwali-sales-analysis/
├── Diwali_Sales_Analysis.ipynb    # Main Jupyter notebook (EDA + charts)
├── Diwali_Sales_Data.csv          # Raw dataset
└── README.md                       # This file
```

---

## Author
**Vijay Nirmalakar**
[[LinkedIn Profile](https://www.linkedin.com/in/vijaynirmalakar/)] | [[GitHub Profile](https://github.com/vijaynirmalakar)]

*Tools: Python, Pandas, NumPy, Matplotlib, Seaborn | Skills: EDA, Data Cleaning, Data Visualization, Business Analysis*
