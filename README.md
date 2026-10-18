# 🪔 Diwali Sales Analysis (Python EDA)

An exploratory data analysis of Diwali festive-season retail sales using **Python (Pandas, NumPy, Matplotlib, Seaborn)** — uncovering which customers, regions, occupations, and product categories drive sales, and turning those findings into business recommendations.

---

## 📌 Problem Statement

Diwali is one of the biggest sales seasons for Indian retailers. To plan campaigns, stock, and ad spend effectively, a business needs to know:
- Who are the highest-spending customers (gender, age group, marital status, occupation)?
- Which states and zones generate the most revenue?
- Which product categories sell the most?

This project analyzes festive sales data to answer these questions and recommend where to focus marketing and inventory.

---

## 🗂️ Dataset

Diwali sales data with **11,251 customer records** (11,239 after cleaning) and the following fields:
- **Customer:** User ID, Name, Gender, Age, Age Group, Marital Status
- **Location:** State, Zone
- **Profile:** Occupation
- **Purchase:** Product ID, Product Category, Orders, Amount

---

## 🛠️ Tools & Tech Stack

| Tool | Purpose |
|------|---------|
| **Python** | Core language |
| **Pandas** | Data cleaning, grouping, aggregation |
| **NumPy** | Numerical operations |
| **Matplotlib & Seaborn** | Data visualization |
| **Jupyter Notebook** | Analysis environment |

---

## ⚙️ Approach

1. **Data Loading & Inspection** — Loaded the CSV, checked shape, data types, and summary statistics
2. **Data Cleaning**
   - Dropped unrelated/blank columns (`Status`, `unnamed1`)
   - Found and removed 12 rows with missing `Amount` values
   - Converted `Amount` from float to integer
3. **Exploratory Data Analysis** — Analyzed sales and order counts by:
   - Gender
   - Age Group (and Age Group × Gender)
   - State (orders and sales)
   - Marital Status (× Gender)
   - Occupation
   - Product Category and Product ID
4. **Insights & Recommendations** — Summarized findings into a conclusion with actionable business suggestions

---

## 🔑 Key Findings

- **Dataset size:** 11,239 customers, 27,981 orders, ₹10.62 crore (106.2M) in total sales, averaging ~₹9,454 per customer
- **Women drive sales:** ~70% of buyers and ~70% of total sales are female customers
- **26-35 is the core age group:** contributes ~40% of sales; together with 36-45 it accounts for ~61%. Women aged 26-35 alone make up ~29% of total sales
- **Sales are geographically concentrated:** Uttar Pradesh (18.2%), Maharashtra (13.6%) and Karnataka (12.7%) together account for ~44.5% of sales. Central zone leads with ~39%
- **Top occupations:** IT Sector (13.9%), Healthcare (12.3%), Aviation (11.9%), and Banking (10.1%)
- **Product categories:** Food leads with ~32% of sales, followed by Clothing & Apparel (15.5%), Electronics & Gadgets (14.7%), and Footwear (14.7%). The top 3 categories contribute ~62% of revenue

---

## 💡 Business Recommendations

- **Target women aged 26-35** with Diwali campaigns, gift bundles, and festive offers
- **Prioritize Uttar Pradesh, Maharashtra, and Karnataka** for ad spend and inventory, as they drive nearly half of all sales
- **Stock up on Food, Clothing, and Electronics** ahead of the festive season
- **Run occupation-based campaigns**, such as corporate gifting for IT and Healthcare professionals
- **Explore low-share zones** (Eastern ~6.6%, Northern ~11.9%) as growth opportunities with targeted promotions

---

## 🚀 How to Run This Project

1. Clone this repository
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. Make sure the CSV file is in the same folder as the notebook
4. Open `main.ipynb` in Jupyter Notebook or VS Code and run all cells

---

## 📁 Repository Structure

```
├── main.ipynb              # Full analysis notebook
├── Diwali Sales Data.csv   # Dataset
└── README.md
```

---

## 👤 Author

**Farhan Adil**
Data Scientist | Ai Automation Specialist
