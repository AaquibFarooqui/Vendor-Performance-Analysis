# Vendor-Performance-Analysis
Simulated a real-world retail use case to analyze vendor performance, inventory turnover, and purchasing efficiency using Power BI, SQL, and Python.
# Vendor Performance Analysis

Analyze vendor contribution, profitability, and inventory risk using a curated retail dataset.  
Built with **Power BI** for the dashboard and **Python / Jupyter** for exploratory analysis and vendor-level summaries.

---

## Project Goals
This project explores how vendor mix, pricing, and purchasing behavior affect sales, profit, and working capital tied up in inventory. Specifically:

- Identify **top vendors** driving most purchases and sales.
- Surface **low-performing vendors** with weak contribution.
- Flag **target brands**: high profit margin but low sales volume (opportunity for promotion/price adjustment).
- Quantify **unsold capital** tied up in slow-moving inventory.
- Compare profit behavior across vendor tiers (top vs low-performing).

All insights come from the supplied dataset (`vendor_sales_summary.csv`) and are visualized in Power BI.

---

## Key Metrics Shown in the Dashboard
- **Total Sales ($)**
- **Total Purchase ($)**
- **Gross Profit ($)**
- **Profit Margin (%)**
- **Unsold Capital ($)**
- **Purchase Contribution %** (Top 10 vs others)
- **Top Vendors by Sales**
- **Top Brands by Sales**
- **Low-Performing Vendors** (relative contribution / score)
- **Target Brands: High Profit, Low Sales** (scatter)

> See the dashboard: open `vendor_performance.pbix` in Power BI Desktop.

---

## Data & Preparation
**Source:** Simulated / project dataset: `vendor_sales_summary.csv`.

**Cleaning & Filtering Steps (as used in analysis & report):**
- Reviewed negative / zero **gross profit** and **profit margin** values.
- Noted products with **zero sales** (potential inventory risk).
- Examined extreme values in **freight cost**, **purchase price**, and **stock turnover**.
- Created filtered views to focus on profitable, selling products where relevant to questions.
- Aggregated data to vendor and brand levels for visualization.

(Full exploratory work is in the notebook.)

---

## Files in This Repository

| File | What It Does |
|------|--------------|
| `Vendor Performance Analysis.ipynb` | Exploratory data analysis, cleaning notes, metric calculations used to support the dashboard/report. |
| `get_vendor_summary.py` | Small utility script to generate vendor-level summary metrics from the CSV. |
| `ingestion_db.py` | Script used during development to load / prepare data (kept for transparency; not required to view dashboard). |
| `vendor_sales_summary.csv` | Project dataset used in analysis and dashboard. |
| `vendor_performance.pbix` | Power BI dashboard (open in Power BI Desktop). |
| `Vendor Performance Report.pdf` | Short business-style report summarizing insights and recommendations. |
| `README.md` | You’re here. |

---

## How to View

- Open `vendor_performance.pbix` in Power BI Desktop to explore the dashboard.
- For deeper context, explore the Jupyter notebook and scripts used to generate summary metrics and insights.
