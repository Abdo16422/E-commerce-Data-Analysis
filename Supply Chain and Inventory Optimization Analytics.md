#  Supply Chain & Inventory Optimization Analytics

##  Project Overview

This project presents an end-to-end **Supply Chain Analytics and Inventory Optimization System** designed to improve operational efficiency, reduce costs, and enhance decision-making using data-driven techniques.

The solution integrates **demand forecasting, inventory optimization, supplier performance evaluation, and cost analysis** into a unified analytics pipeline.

---

##  Objectives

* Detect **stockout and overstock situations**
* Optimize **reorder points and order quantities**
* Evaluate **supplier performance**
* Forecast demand using **time series models**
* Minimize **total inventory cost**

---

##  Key Features

###  1. Exploratory Data Analysis (EDA)

* Demand distribution and variability analysis
* Identification of trends and seasonality

---

###  2. Demand Forecasting

* Implemented:

  * ARIMA model
  * Prophet model
* Captured:

  * Trend
  * Seasonality
  * Demand uncertainty (prediction intervals)

---

###  3. Inventory Optimization Engine

* Dynamic calculation of:

  * Reorder Point (ROP)
  * Safety Stock
  * Order Quantity
* Integrated:

  * Lead Time variability
  * Demand variability
* Automated replenishment decisions

---

###  4. Supplier Performance Evaluation

* Measured KPIs:

  * Lead Time
  * Cost Efficiency
  * Defect Rate
  * On-Time Delivery
* Built a **Supplier Scoring Model**
* Segmented suppliers into performance tiers

---

###  6. Cost Optimization

* Applied **Economic Order Quantity (EOQ)**
* Balanced:

  * Holding Cost
  * Ordering Cost
  * Stockout Cost
* Identified cost trade-offs and optimal policies

---

##  Key Formulas Used

* Reorder Point:
  ROP = (Demand × Lead Time) + Safety Stock

* Safety Stock:
  SS = Z × σ × √L

* Economic Order Quantity:
  EOQ = √(2DS / H)

---

##  Dataset Description

The dataset was synthetically generated to simulate real-world supply chain operations and includes:

* **Products / Inventory Data**
* **Sales Transactions (Time Series)**
* **Supplier Information**
* **Procurement Data**

---

##  Tools & Technologies

* Python (Pandas, NumPy)
* Data Visualization: Matplotlib, Plotly
* Time Series Modeling:

  * Statsmodels (ARIMA)
  * Prophet
* Jupyter Notebook

---

##  Key Insights

* Demand exhibits both **stable and volatile patterns**, requiring adaptive inventory strategies
* A small percentage of products drives the majority of sales (**Pareto principle**)
* Forecasting models reveal **significant demand fluctuations** and uncertainty
* Supplier performance varies significantly, impacting supply reliability
* Inventory mismatches lead to both **overstock and stockout risks**
* Optimized policies significantly reduce total operational cost

---

##  Business Impact

* Reduced stockout risk through predictive planning
* Improved inventory turnover and cost efficiency
* Enhanced supplier selection and procurement strategy
* Enabled data-driven decision-making through scenario simulation





