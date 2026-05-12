# Retail Intelligence Suite: Predictive Forecasting & Customer Analytics

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Prophet](https://img.shields.io/badge/Forecasting-Prophet-orange.svg)](https://facebook.github.io/prophet/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📌 Project Overview
This project delivers an end-to-end Business Intelligence solution for a multi-category retail operation. By integrating **Holt-Winters Seasonal Forecasting**, **RFM Churn Modeling**, and a high-performance **Market Basket Recommendation Engine**, the suite transforms transactional data into actionable growth strategies.

### Key Business Objectives
* **Stabilize Forecasting:** Use Logistic Growth and Triple Exponential Smoothing to predict Q4 revenue peaks.
* **Customer Health:** Monitor high-value "Outlier" segments to identify churn risk before it happens.
* **Maximize Basket Value:** Identify missed cross-sell opportunities using high-lift association rules.

---

## 🛠️ Tech Stack
* **Core Analysis:** `Pandas`, `NumPy`
* **Time-Series Models:** `Prophet` (Facebook/Meta), `Statsmodels` (Holt-Winters)
* **Performance Optimization:** `Scipy.sparse` (Sparse matrix math for sub-second recommendations)
* **Visualization:** `Plotly`, `Pandas Styler` (Interactive Dashboards)

---

## 🚀 Project Modules

### 1. Customer Segmentation & Outlier Analysis
Instead of treating all customers equally, the system isolates **"High-Value Outliers"** (Wholesale/B2B) from **"Normal"** retail shoppers. 
* **Insight:** High-value customers drive 70% of revenue but have distinct purchasing cycles compared to the holiday-driven retail segment.

### 2. Time-Series Revenue Forecasting
The project implements dual forecasting methods to map out the 2012 fiscal year.
* **Home Decor:** Captures massive Q4 seasonality, predicting a milestone **£700k+ month** in November.
* **Kitchenware:** Identifies a front-loaded pattern with peaks in January, allowing for better inventory rotation.

### 3. Market Basket Analysis (MBA)
Using a custom-built, sparse-matrix-powered recommendation engine, the system calculates **Lift** and **Confidence** for product pairings.
* **The "Missed Item" Hook:** Automatically identifies products a high-value customer has *not* purchased that have a high statistical affinity (Lift > 4.0) with their current inventory.

### 4. Account Health and Churn 
A proactive monitoring tool that cross-references **Recency** against a customer's unique **Average Purchase Interval (API)**.
* **Risk Factor:** Flags customers who miss their natural ordering cycle (e.g., Risk Factor > 2.0 = High Risk).
* **Outcome:** A prioritized lead list for sales teams to initiate "Win-Back" campaigns using the recommendations from the MBA module.

---

## 📊 Key Results
| Metric | Value |
| :--- | :--- |
| **Projected Peak Monthly Revenue** | £1.09M (Consolidated Nov 2012) |
| **High-Risk Accounts Identified** | 20% of High-Value Segment |
| **Recommendation Engine Speed** | Optimized for 5,000+ SKUs using Sparse Matrices |
| **Top Cross-Sell Opportunity** |  High Lift Cluster |

---

