# 🚀 Task 5 — Predictive Model: Linear Regression

**DecodeLabs Data Analytics Internship | Batch 2026**  
**Intern:** Umm-e-Abiha

---

## 🎯 Objective

Design, train, and rigorously evaluate a supervised machine learning model to predict `TotalPrice` from customer and order features, and extract actionable business insights from the model's learned parameters.

---

## 🤖 Model Overview

| Attribute | Detail |
|-----------|--------|
| Algorithm | Linear Regression |
| Target Variable | `TotalPrice` |
| Train / Test Split | 80% / 20% (random_state=42) |
| **R² Score** | **~0.89** |
| **RMSE** | **~$288** |
| Model Rating | Excellent (R² > 0.85) |

---

## 📋 What Was Done

| Step | Action |
|------|--------|
| 5.1 | Feature engineering: Label encoding for categorical columns; `HasCoupon` binary flag |
| 5.2 | Feature and target variable selection |
| 5.3 | Reproducible 80/20 train-test split |
| 5.4 | Linear Regression training with `scikit-learn` |
| 5.5 | Model evaluation using R² and RMSE |
| 5.6 | Feature importance analysis via absolute coefficients |
| 5.7 | Sample prediction review with error annotation |
| 5.8 | 3-panel model performance visualisation |

---

## 🏗️ Feature Engineering

| Feature | Type | Transformation |
|---------|------|----------------|
| `Quantity` | Numeric | Used as-is |
| `UnitPrice` | Numeric | Used as-is |
| `ItemsInCart` | Numeric | Used as-is |
| `Product` | Categorical | Label Encoded → `Product_enc` |
| `PaymentMethod` | Categorical | Label Encoded → `PaymentMethod_enc` |
| `CouponCode` | String | Binary flag → `HasCoupon` (0/1) |
| `Month` | Numeric | Extracted from Date in Task 2 |

---

## 🏆 Feature Importance (Ranked)

| Rank | Feature | Role |
|------|---------|------|
| 1 | **Quantity** | Strongest driver — more units = higher bill |
| 2 | **Product_enc** | Product type significantly influences price |
| 3 | **HasCoupon** | Coupon usage measurably affects order value |
| 4 | **UnitPrice** | Per-unit cost drives total |
| 5 | **Month** | Minimal but present seasonal signal |

---

## 📊 Model Performance

| Metric | Value | Benchmark |
|--------|-------|-----------|
| R² Score | ~0.89 | >0.85 = Excellent |
| RMSE | ~$288 | Avg error on $1,054 orders (~27%) |

**Residual Analysis:** Residuals follow a near-normal distribution centred at zero, indicating the model is unbiased and errors are random — a sign of a well-fitted model.

---

## 💡 Business Recommendation

> **Quantity is the most powerful revenue lever.** To increase average order value, businesses should implement:
> - **Bundle offers** (buy 3, get 1 at half price)
> - **Volume discounts** for multi-unit orders
> - **Cross-sell recommendations** at checkout

---

## 📁 Output

| File | Description |
|------|-------------|
| `Task_05_Predictive_Model.ipynb` | Notebook for this task |
| `task5_model.png` | Actual vs Predicted · Residuals · Feature Importance |

---

## 🛠️ Libraries Used

`pandas` · `numpy` · `scikit-learn` · `matplotlib`

---

*DecodeLabs Industrial Training Program | Batch 2026*
