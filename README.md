# 🛒 RetailPulse
### Data-Driven Insights for Seasonal Retail Optimization

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-data%20wrangling-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-visualization-11557C)
![Seaborn](https://img.shields.io/badge/Seaborn-statistical%20plots-4C72B0)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)

*An exploratory data analysis of ~2.75 years of retail transactions, revealing when to advertise, when to discount, and which categories win each season.*

</div>

---

## 📌 Project Overview

**RetailPulse** applies **Exploratory Data Analysis (EDA)** to **RetailMart**, a mid-sized US retail chain operating **150 stores** across **four regions** (North, South, East, West) and trading in **three product categories** (Electronics, Apparel, Home Goods).

Using **Pandas, Matplotlib, and Seaborn**, the project explores **daily transaction data from January 2022 to September 2024** to understand how **seasonality**, **advertising spend**, and **discounting** drive **sales, customer activity, and profit** — and turns those patterns into concrete, actionable business decisions.


---

## ❓ Problem Statement

RetailMart's leadership lacks a clear, data-driven view of how seasonal patterns, advertising spend, and discount strategies translate into measurable outcomes such as **profit** and **customer satisfaction**. The analysis is built to answer three core business questions:

- **Advertising** — Are budgets allocated effectively to maximise sales?
- **Seasonality & discounts** — How do they affect customer purchasing behaviour and profitability?
- **Prioritisation** — Which product categories and regions should be the focus, and *when*?

---

## 🎯 What the Analysis Covers

- **Visualise key business metrics** — sales, profit, advertising, and customer-count trends over time.
- **Understand seasonal trends** — how sales and customer activity vary across months and seasons.
- **Assess advertising effectiveness** — how spend relates to sales, and how to time it better.
- **Evaluate discount strategy** — the impact of discounts on footfall, sales, and margin.
- **Identify high performers** — the leading categories and regions for sales and profit.
- **Correlation analysis** — quantify the relationships between every numeric metric.

---

## 📊 Key Findings

| Theme | Finding | Evidence |
|---|---|---|
| 🍂 **Seasonality** | Sales & customer activity **peak Sep–Dec** (Winter & Fall) and **dip in Spring/Summer**; **Winter is the most profitable season**. | Monthly & seasonal trend charts |
| 📣 **Advertising works** | Advertising spend is a **genuine driver** of sales and profit. | **r ≈ 0.60** (sales), **r ≈ 0.51** (profit) |
| ⏱️ **Timing mismatch** | Ad budget was historically **reduced during peak season** — a missed opportunity. In 2023, raising it during a slump pushed sales to an **all-time high**. | Advertising vs. sales over time |
| 🏷️ **Discounts ≠ profit** | Discounts **strongly attract customers** but barely move revenue or margin. | **r ≈ 0.99** (footfall) vs **0.28** (sales), **0.22** (profit) |
| 💰 **Sales → Profit** | Growing sales **reliably grows profit**. | **r ≈ 0.86** |
| 📦 **Category leaders** | **Electronics** lead on sales; **Home Goods** lag. | Category bar charts |
| 🌍 **Regional leaders** | The **East** region slightly outperforms on **both** sales and profit. | Region bar charts |

**The three that matter most:**

1. **Advertising is being mistimed.** The data shows spend is strongest when it should be tapering and weakest during the holiday peak — yet advertising clearly lifts sales. Re-timing this is the single biggest quick win.
2. **Deep discounting erodes value.** Discounts almost perfectly track customer count but have little effect on profit, meaning blanket discounts buy footfall at the expense of margin.
3. **Demand is predictable.** Clear, repeatable seasonal peaks make budgets, inventory, and promotions plannable months in advance.

---

## 💡 Business Recommendations

- **🎯 Re-time advertising to match demand.** Move more budget into the high-demand **Sep–Dec / Winter** window instead of cutting it, and protect a baseline spend year-round to avoid Spring slumps like 2023.
- **🏷️ Use discounts surgically, not broadly.** Target discounts at **off-peak seasons (Spring/Summer)** to lift naturally low traffic, and avoid deep discounts at peak when customers already convert at full price.
- **📦 Lead peak season with Electronics.** Prioritise the top category in holiday campaigns and inventory, and test **cross-category bundles** (e.g. Apparel/Home Goods with Electronics) to lift weaker lines.
- **🌍 Replicate the East region's edge.** Investigate what drives its higher sales and profit, then roll those practices out to **North, South, and West**.
- **🤝 Support weak areas with margin-aware promotions.** Pair targeted advertising with selective offers in lagging categories/regions rather than blanket discounting.
- **📈 Monitor with a seasonal dashboard.** Track sales, profit, advertising, and customer count by **month, season, category, and region** to tune decisions in near-real time.

---

## 🛠️ Tech Stack

| Area | Tools |
|---|---|
| **Language** | Python |
| **Data wrangling** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Environment** | Jupyter Notebook |

---

## 🗂️ Dataset

A simulated daily-transaction dataset for the fictional **RetailMart** chain (case-study data), spanning **2022-01-01 → 2024-09-30**.

<details>
<summary><b>Data dictionary (click to expand)</b></summary>

| Column | Description | Type |
|---|---|---|
| `Date` | Transaction date | DateTime |
| `Category` | Electronics, Apparel, Home Goods | Categorical |
| `Region` | North, South, East, West | Categorical |
| `Weather` | Weather condition on the day | Categorical |
| `Advertising` | Advertising spend ($) | Numerical |
| `Discount` | Discount offered (%) | Numerical |
| `Sales` | Total sales ($) | Numerical |
| `Customer_Count` | Number of customers | Numerical |
| `Profit` | Profit ($) | Numerical |
| `Month` | Month name | Categorical |
| `Season` | Winter, Spring, Summer, Fall | Categorical |
| `Year` | Year of transaction | Numerical |

</details>

---

## 🚀 Getting Started

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/retailpulse-seasonal-eda.git
cd retailpulse-seasonal-eda

# 2. Install the dependencies
pip install pandas numpy matplotlib seaborn jupyter

# 3. Launch the notebook
jupyter notebook Project-RetailMart.ipynb
```

> **Note:** update the dataset path in the notebook to point to `retailmart_data.csv` in this repo.

---



---

## 👤 Author

**Marc Ntjam**


---
