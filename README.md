# Apple Global Sales Analysis

An end-to-end data analysis project exploring Apple's global sales performance using **Python** for data processing and visualization, and **Power BI** for interactive dashboarding.

## 📊 Dashboard Preview

![Apple Sales Dashboard](dashboard.png)

## Project Overview

This project analyzes Apple's global sales dataset to uncover trends across products, regions, time periods, customer segments, and sales channels. The goal is to derive actionable business insights from the data using both exploratory analysis and visual storytelling.

## Key Insights

| Metric | Value |
|---|---|
| Total Revenue | $18.04M |
| Total Units Sold | 23K |
| Avg Units Per Order | 2.02 |
| Avg Discount | 3.84% |
| Avg Customer Rating | 4.00 |

- **Best Product:** Mac ($8.4M) led revenue, followed by iPhone ($5.7M) and iPad ($1.8M)
- **Best Month:** October was the top-performing month, followed by December and March
- **Best Region:** Europe dominated sales ($6.2M), followed by Asia ($5.4M) and South America
- **Customer Segments:** Education, Government, Business, and Individual segments all contributed nearly equally (~$4.5M each)
- **Return Rate:** 87.35% of items were kept, with only 4.46% returned and 8.19% exchanged

---

## Tools & Technologies

- **Python** — Data cleaning, EDA, and visualization
  - `pandas` — Data manipulation
  - `numpy` — Numerical operations
  - `matplotlib` — Plotting
  - `seaborn` — Statistical visualization
- **Power BI** — Interactive dashboard and business reporting

---

## Project Structure

```
apple-sales-analysis/
│
├── apple_analysis.py           # Python EDA and visualization script
├── Apple_Sales_Dashboard.pbix  # Power BI dashboard file
├── apple_global_sales_dataset.csv  # Dataset
├── dashboard.png               # Dashboard screenshot
└── README.md
```

---

## Analysis Performed

**Python (EDA & Visualization)**
- Null value detection and imputation (customer ratings filled using product-level mean)
- Total revenue by product, country, region, month, and year
- Units sold by year, region (pie chart), and discount tier
- Sales by channel, customer age group, and product color

**Power BI (Dashboard)**
- KPI cards for high-level metrics
- Category vs Sales and Category vs Units Sold bar charts
- Month vs Sales trend line
- Age group and customer segment breakdowns
- Geographic map of sales by country
- Return status breakdown (Kept / Returned / Exchanged)
- Year slicer (2022, 2023, 2024)

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/apple-sales-analysis.git
   cd apple-sales-analysis
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

3. Run the Python analysis:
   ```bash
   python apple_analysis.py
   ```

4. Open `Apple_Sales_Dashboard.pbix` in **Power BI Desktop** to explore the interactive dashboard.

---

## Dataset

- **Source:** [Kaggle – Apple Global Sales Dataset](https://www.kaggle.com/datasets/ashyou09/apple-global-product-sales-dataset?resource=download)
- **Records:** Global Apple product sales transactions
- **Key Columns:** `product_name`, `revenue_usd`, `units_sold`, `country`, `region`, `month`, `year`, `sales_channel`, `customer_age_group`, `customer_rating`, `discount_pct`, `color`, `return_status`

---
