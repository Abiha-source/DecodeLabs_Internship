# 📈 Task 4 — Data Visualisation Dashboard

**DecodeLabs Data Analytics Internship | Batch 2026**  
**Intern:** Umm-e-Abiha

---

## 🎯 Objective

Design and build a comprehensive, publication-quality analytics dashboard that communicates the E-Commerce dataset's key business insights through carefully chosen, well-labelled visualisations.

---

## 📋 What Was Done

A 6-panel dashboard was constructed using `matplotlib`, with each chart type deliberately selected to best represent the underlying data structure.

| Panel | Chart Type | Insight Communicated |
|-------|-----------|----------------------|
| 1 | Line Chart | Monthly revenue trend over 2.5 years |
| 2 | Scatter Plot | Relationship between Quantity and TotalPrice by product |
| 3 | Horizontal Bar | Top 5 customers by total lifetime revenue |
| 4 | Bar Chart | Revenue contribution by coupon code |
| 5 | Violin Plot | Unit price distribution spread per product |
| 6 | Grouped Bar | Order status breakdown by product type |

---

## 🎨 Design Decisions

| Decision | Rationale |
|----------|-----------|
| Dark theme (#0d0d0d background) | Professional, modern analytics aesthetic |
| Cyan accent colour (#00d4ff) | High contrast on dark background; easy readability |
| Value labels on bars | Eliminates the need for readers to estimate values |
| Distinct colour per series | Enables clear product/status differentiation |
| 150 DPI output | Publication-quality resolution for reports |

---

## 💡 Dashboard Insights

- **Monthly Revenue:** Stable with fluctuations; no strong seasonality observed
- **Scatter Plot:** Higher unit prices correlate strongly with higher total bills
- **Top Customers:** Small customer cohort drives disproportionate revenue (Pareto principle)
- **Coupon Revenue:** Customers without coupons generate the most revenue overall
- **Violin Plot:** Chair, Laptop, and Tablet show the widest price distributions
- **Status by Product:** Return/cancellation rates are consistent across all products

---

## 📁 Output

| File | Description |
|------|-------------|
| `Task_04_Visualization.ipynb` | Notebook for this task |
| `task4_visualization.png` | 6-panel analytics dashboard (saved at 150 DPI) |

---

## 🛠️ Libraries Used

`pandas` · `matplotlib` · `numpy`

---

*DecodeLabs Industrial Training Program | Batch 2026*
