# Vendor Performance Analysis

This project analyzes vendor performance, inventory turnover, and purchasing strategies using **Python**, **SQL**, and **Power BI**. It simulates a real-world retail scenario to identify underperforming vendors, optimize pricing strategies, and improve procurement efficiency.

---

##  Objectives

- Identify vendors with **low sales and high inventory holding**.
- Analyze the contribution of **top vendors** to total purchases and sales.
- Evaluate the impact of **bulk purchasing** on unit costs.
- Examine **profit margins** of top-performing vs. low-performing vendors.
- Provide actionable recommendations to reduce unsold inventory.

---

##  Key Insights

- **$2.71M in unsold inventory** due to low-turnover vendors.
- **Top 10 vendors** contribute **65.7% of total purchases**, indicating supplier dependency.
- **Bulk purchasing** reduces unit cost by ~72%.
- **Low-performing vendors** have higher margins but weaker sales volumes.
- **441.41M in sales**, **134.07M gross profit**, and **38.7% average profit margin** (as per dashboard metrics).

>  **[View Full PDF Report](./Vendor%20Performance%20Report.pdf)**

---

##  Project Files

```bash
├── Vendor Performance Analysis.ipynb    # Jupyter Notebook for analysis
├── ingestion_db.py                      # Script to load data into SQLite
├── vendor_sales_summary.csv             # Sample dataset
├── vendor_performance.pbix              # Power BI dashboard
├── Vendor Performance Report.pdf        # Final report with insights
└── README.md
