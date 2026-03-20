# 📊 Sales Analytics Dashboard (Power BI)

## 🚀 Project Overview

This project presents a **Sales Analytics Dashboard** built using **Power BI** to provide a centralized view of sales performance and business insights.

It enables stakeholders to monitor key metrics, compare performance across different dimensions, and make data-driven decisions using a single interactive dashboard.

---

## 🎯 Business Problem

The organization faced several challenges:

* Sales data was scattered across multiple systems
* No clear visibility into revenue and deal performance
* Difficulty tracking sales team effectiveness
* Lack of centralized reporting

👉 This dashboard solves these problems by providing a **single source of truth for sales analytics**.

---

## 🛠️ Tools & Technologies

* Power BI (Data Visualization)
* DAX (Data Analysis Expressions)
* Power Query (Data Transformation)

---

## 📊 Dashboard Overview

This dashboard provides a comprehensive view of sales performance using the following components:

### 🔢 Key Metrics (KPIs)

* **Total Revenue**
* **Won Deals**
* **Lost Deals**
* **Win Rate (%)**

---

### 📈 Visualizations

* **Revenue by Account**
  Identifies top customers contributing to revenue

* **Total Sales Overview**
  Shows overall sales distribution and variation

* **Revenue by Office Location (Map)**
  Displays geographic distribution of revenue

* **Sales by Agent (Won vs Lost)**
  Compares performance of sales representatives

* **Product Performance**
  Shows number of won deals by product

* **Revenue by Sector**
  Highlights contribution from different industries

---

## 🧠 Key KPIs (DAX)

### Total Revenue

```DAX id="0cbozj"
Total Revenue = SUM(sales_pipeline[revenue])
```

### Won Deals

```DAX id="7qf0r3"
Won Deals = 
CALCULATE(
    COUNTROWS(sales_pipeline),
    sales_pipeline[deal_stage] = "Won"
)
```

### Lost Deals

```DAX id="y4t0ot"
Lost Deals = 
CALCULATE(
    COUNTROWS(sales_pipeline),
    sales_pipeline[deal_stage] = "Lost"
)
```

### Win Rate

```DAX id="1t6o0h"
Win Rate = 
DIVIDE(
    [Won Deals],
    [Won Deals] + [Lost Deals],
    0
)
```

---

## 🎛️ Features

* Interactive and user-friendly dashboard
* Cross-filtering between visuals
* Clear KPI representation
* Business-focused insights

---

## 📈 Insights Derived

* The business has a **63% win rate**, indicating strong sales performance
* A few **key accounts contribute significantly** to total revenue
* Certain **products drive more successful deals**
* Sales performance varies across **agents and regions**

---

## 🧠 Business Impact

* Improves visibility into sales performance
* Helps identify high-value customers and products
* Enables better performance comparison across teams
* Supports faster and more informed decision-making

---

## 🏁 Conclusion

This dashboard provides a **complete view of sales performance** in a single page, helping stakeholders analyze key metrics and identify opportunities for business growth.

---

## 👨‍💻 Author

Sai Teja
Python Full Stack Developer | Data Engineer Enthusiast
