# Diwali Sales Analysis

**Project type:** Exploratory Data Analysis (EDA) & Sales Insights using Python (pandas)

---

## Project Overview

This project explores a retail dataset (Diwali sales) to uncover customer and product-level patterns that can help improve sales strategy and inventory planning. Using `pandas` for data cleaning and manipulation and visualization libraries for charting, the analysis identifies top-selling products, high-value age groups, and customer segments across states, genders and occupations.

---

## Objectives

- Clean and prepare the Diwali sales dataset for analysis.
- Perform Exploratory Data Analysis (EDA) to understand sales distribution and customer demographics.
- Identify top products, product categories, and customer segments to inform inventory and marketing decisions.
- Produce clear visualizations and actionable insights for stakeholders.

---

## Key Learnings from the Project

- Performed thorough data cleaning and manipulation (missing values, data types, duplicates, date parsing).
- Conducted EDA using `pandas` and plotting libraries to summarize trends and distributions.
- Identified potential customer segments across **states, occupations, gender, and age groups** to target marketing and personalize offers.
- Identified most-selling product categories and products to help plan inventory and meet demand.

---

## Files in this repository

- `Diwali Sales Data.csv` — Raw dataset used for the analysis.
- `Diwali_sales_analysis.ipynb` — Jupyter notebook containing the full analysis, visualizations and code.
- `README.md` — This file.

---

## Tools & Libraries

- Python 3.x
- pandas — data cleaning and manipulation
- numpy — numerical operations
- matplotlib / seaborn / plotly.express — visualization

Install required packages with pip if needed:

```bash
pip install pandas numpy matplotlib seaborn plotly
```

---

## Quick Start (how to run)

1. Clone or download this repository.
2. Put `Diwali Sales Data.csv` in the same folder as the notebook (if not already).
3. Open `Diwali_sales_analysis.ipynb` with Jupyter Notebook or VS Code and run the cells.

Example starting code used in the notebook:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

# load data
df = pd.read_csv('Diwali Sales Data.csv')

# quick preview
df.head()

# basic cleaning example
df = df.drop_duplicates()
df['Order_Date'] = pd.to_datetime(df['Order_Date'], errors='coerce')

# aggregate example: top products by orders
top_products = df.groupby('Product_ID', as_index=False)['Orders'].sum().sort_values('Orders', ascending=False).head(10)

# plotting example
plt.figure(figsize=(10,6))
sns.barplot(x='Product_ID', y='Orders', data=top_products, palette='Set2')
plt.title('Top 10 Products by Orders')
plt.xticks(rotation=45)
plt.tight_layout()
plt.show()
```

---

## Example analysis steps (what the notebook covers)

1. **Load & inspect** the dataset (`.head()`, `.info()`, `.describe()`).
2. **Clean**: handle missing values, drop duplicates, fix data types, standardize text columns.
3. **Feature engineering**: extract month/year from order date, create age buckets, compute revenue if applicable.
4. **Aggregate & group**: compute sales by state, product category, age group, gender, occupation.
5. **Visualize**: bar charts, stacked charts, heatmaps and distribution plots to reveal patterns.
6. **Insights**: list of actionable findings and recommended next steps.

---

## Suggested Insights (examples you can expand)

- Which **age groups** contribute the most to total sales.
- **Top 10 products** that generate the majority of orders/revenue.
- **States** with highest order volumes — useful for logistics and inventory planning.
- **Gender** and **occupation** breakdowns showing customer segments to target.

---

## Next steps & Recommendations

- Build a simple recommendation engine using purchase history for cross-sell/up-sell.
- Forecast demand for top products and plan inventory accordingly.
- Create a dashboard (Power BI / Tableau / Plotly Dash) for stakeholders to interact with these insights.
- Enrich the dataset with external signals (holidays, promotions) to measure campaign impact.

---

## Notes & Data Privacy

- Always check data privacy and sharing policies before publishing or sharing customer data. Mask personally identifiable information if required.

---

## Contact

If you have questions or want help customizing the analysis, feel free to reach out.

---

*End of README*

