# 📊 DecodeLabs Data Analytics Internship — Batch 2026

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-1.5-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/Scikit--Learn-1.2-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Matplotlib-3.7-11557C?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Status-Completed-39ff14?style=for-the-badge"/>
</p>

---

## 👩‍💻 Intern Information

| Field | Detail |
|-------|--------|
| **Intern** | Umm-e-Abiha |
| **Program** | DecodeLabs Industrial Data Analytics Internship |
| **Batch** | 2026 |
| **Domain** | Data Analytics |
| **Duration** | June 2026 |

---

## 📁 Repository Structure

```
DecodeLabs-DataAnalytics-Internship/
│
├── 📓 DecodeLabs_Complete_Analytics.ipynb    ← Full project (all 5 tasks in one file)
├── 📓 Task_01_Data_Collection.ipynb
├── 📓 Task_02_Data_Cleaning.ipynb
├── 📓 Task_03_EDA.ipynb
├── 📓 Task_04_Visualization.ipynb
├── 📓 Task_05_Predictive_Model.ipynb
│
├── 📊 Dataset_for_Data_Analytics.xlsx        ← Source dataset
│
├── 🖼️  task1_overview.png
├── 🖼️  task2_cleaning.png
├── 🖼️  task3_eda.png
├── 🖼️  task4_visualization.png
├── 🖼️  task5_model.png
│
├── 📄 README.md                              ← This file
├── 📄 README_Task01.md
├── 📄 README_Task02.md
├── 📄 README_Task03.md
├── 📄 README_Task04.md
└── 📄 README_Task05.md
```

---

## 🗂️ Dataset Overview

| Attribute | Detail |
|-----------|--------|
| **Name** | E-Commerce Orders Dataset |
| **Rows** | 1,200 |
| **Columns** | 14 |
| **Time Span** | January 2023 – June 2025 |
| **Domain** | Business-to-Consumer (B2C) E-Commerce |

### Columns
| Column | Type | Description |
|--------|------|-------------|
| `OrderID` | String | Unique order identifier |
| `Date` | Date | Order placement date |
| `CustomerID` | String | Unique customer identifier |
| `Product` | Categorical | Product type (7 categories) |
| `Quantity` | Integer | Units ordered per transaction |
| `UnitPrice` | Float | Price per unit (USD) |
| `TotalPrice` | Float | Total order value (Qty × UnitPrice) |
| `OrderStatus` | Categorical | Fulfilment status (5 categories) |
| `PaymentMethod` | Categorical | Payment channel |
| `CouponCode` | String | Discount coupon applied (nullable) |
| `ReferralSource` | Categorical | Customer acquisition channel |
| `ItemsInCart` | Integer | Total items in cart at checkout |

---

## ✅ Tasks Completed

| # | Task | Key Deliverable | Outcome |
|---|------|-----------------|---------|
| 1 | **Data Collection & Understanding** | Dataset profile, column documentation | 1,200 rows, 14 features documented |
| 2 | **Data Cleaning & Preprocessing** | Change log, imputation, validation | 0 missing, 0 duplicates, clean types |
| 3 | **Exploratory Data Analysis** | Stats, outliers, correlations, revenue trends | 8 TotalPrice outliers; UnitPrice strongest correlate |
| 4 | **Data Visualisation Dashboard** | 6-panel professional dashboard | Trend, scatter, violin, grouped bar charts |
| 5 | **Predictive Model** | Linear Regression — TotalPrice prediction | R² = 0.89 · RMSE = $288 |

---

## 🔑 Key Business Insights

1. 🪑 **Chair** is the top revenue-generating product
2. 📱 **Instagram** is the #1 customer acquisition channel
3. 💳 **Online payment** is the most preferred payment method
4. 📦 **Quantity** is the strongest predictor of order value
5. 🏷️ **~74% of orders** are placed without a discount coupon
6. 📈 **Revenue is right-skewed** — a small number of high-value orders pull the mean above the median
7. ↩️ Return and cancellation rates are **consistent across all product types** (no systemic issue)

---

## 🤖 Model Summary

| Metric | Value |
|--------|-------|
| Algorithm | Linear Regression |
| Features | Quantity, UnitPrice, ItemsInCart, Product, PaymentMethod, HasCoupon, Month |
| Train / Test Split | 80% / 20% |
| **R² Score** | **~0.89** |
| **RMSE** | **~$288** |
| Top Feature | Quantity (highest absolute coefficient) |

---

## 🛠️ Tools & Libraries

| Library | Version | Purpose |
|---------|---------|---------|
| Python | 3.10+ | Programming language |
| Pandas | 1.5+ | Data manipulation |
| NumPy | 1.23+ | Numerical computation |
| Matplotlib | 3.7+ | Visualisation |
| Seaborn | 0.12+ | Statistical plots |
| Scikit-learn | 1.2+ | Machine learning |
| OpenPyXL | 3.0+ | Excel file reading |

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/DecodeLabs-DataAnalytics-Internship.git
   cd DecodeLabs-DataAnalytics-Internship
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn openpyxl
   ```

3. **Run individual tasks**
   ```bash
   jupyter notebook Task_01_Data_Collection.ipynb
   ```

4. **Run the complete project**
   ```bash
   jupyter notebook DecodeLabs_Complete_Analytics.ipynb
   ```

> **Note:** Ensure `Dataset_for_Data_Analytics.xlsx` is in the same directory as the notebooks.

---

## 📊 Visual Outputs

| File | Contents |
|------|----------|
| `task1_overview.png` | Product distribution & order status pie chart |
| `task2_cleaning.png` | Missing value before/after & payment method bar chart |
| `task3_eda.png` | 6-panel EDA: histogram, revenue, heatmap, boxplot, status, referral |
| `task4_visualization.png` | Full 6-panel analytics dashboard |
| `task5_model.png` | Actual vs Predicted, Residuals, Feature Importance |

---

## 📬 Contact

**Intern:** Umm-e-Abiha  
**Program:** DecodeLabs Data Analytics Internship — Batch 2026

---

*© 2026 DecodeLabs Industrial Training Program. All rights reserved.*
