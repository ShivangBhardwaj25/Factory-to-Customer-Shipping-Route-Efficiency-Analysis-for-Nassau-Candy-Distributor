# Factory-to-Customer-Shipping-Route-Efficiency-Analysis-for-Nassau-Candy-Distributor
End-to-end Supply Chain Analytics project with Python, Power BI, and interactive dashboards to analyze shipping route efficiency, logistics KPIs, and operational performance.

# 🍬 Nassau Candy Distributor — Shipping Route Efficiency Analysis

An end-to-end **Supply Chain & Logistics Analytics** project that analyzes factory-to-customer shipping performance for **Nassau Candy Distributor**, a national distributor serving customers across the United States and Canada.

This project transforms raw shipment data into actionable logistics insights by identifying efficient shipping routes, operational bottlenecks, and regional performance differences. The analysis is presented through both an **interactive web dashboard** and a **Power BI dashboard**, enabling business users to monitor shipping efficiency and make data-driven decisions.

---

## 📌 Project Overview

Nassau Candy Distributor operates multiple manufacturing facilities that ship products to customers across North America. Although the company collects extensive order and shipment data, it lacked a centralized analytical framework to evaluate shipping route performance.

Without route-level visibility, logistics decisions become reactive rather than data-driven, making it difficult to identify operational inefficiencies and optimize distribution.

This project addresses those challenges by analyzing shipping routes, delivery performance, and geographic trends using Python and Power BI.

---

## ❓ Problem Statement

The organization currently lacks visibility into:

- Factory-to-customer shipping efficiency
- Delivery performance across regions and states
- Route-specific operational bottlenecks
- Shipping method effectiveness
- Cost versus delivery time trade-offs
- Geographic variations in logistics performance

As a result, logistics planning becomes reactive, increasing transportation costs and reducing operational efficiency.

---

## 🎯 Business Objectives

### Primary Objectives

- Evaluate shipping efficiency across factory-to-customer routes
- Identify high-performing and underperforming shipping routes
- Analyze delivery performance by region, state, and shipping method
- Measure operational bottlenecks using route-level KPIs

### Secondary Objectives

- Support logistics planning
- Improve shipment scheduling
- Optimize shipping route performance
- Enable data-driven operational decision-making

---

# 📊 Dataset Description

The dataset contains approximately **10,200 shipment records** covering deliveries across the United States and Canada.

### Dataset Features

- Order Date
- Ship Date
- Factory
- Product
- Customer
- State / Province
- Region
- Ship Mode
- Sales
- Profit
- Quantity

The analysis covers:

- **5 Factories**
- **59 States / Provinces**
- **4 Shipping Methods**
- **15 Product Categories**

---

# 🔄 Project Workflow

```
Raw Shipment Data
        │
        ▼
Data Cleaning
        │
        ▼
Feature Engineering
        │
        ▼
Route Mapping
        │
        ▼
Exploratory Data Analysis
        │
        ▼
KPI Development
        │
        ▼
Dashboard Development
        │
        ▼
Business Insights
        │
        ▼
Recommendations
```

---

# 🧹 Data Cleaning & Feature Engineering

The following preprocessing steps were performed:

- Cleaned shipment records
- Validated date fields
- Calculated Lead Time
- Created Factory → State routes
- Created Factory → Region routes
- Calculated Profit Margin (%)
- Added Year and Month columns
- Created Delay Indicators
- Mapped products to manufacturing factories

---

# 📈 Analytical Methodology

## 1. Route Performance Analysis

Shipping routes were analyzed at both:

- Factory → State level
- Factory → Region level

Metrics calculated include:

- Shipment Volume
- Average Lead Time
- Lead Time Variability
- Route Efficiency Score

---

## 2. Route Benchmarking

More than **180 shipping routes** were benchmarked using a normalized **Route Efficiency Score (0–100)**.

The analysis identified:

- Top 10 Most Efficient Routes
- Bottom 10 Least Efficient Routes

---

## 3. Geographic Analysis

Regional performance was evaluated to identify:

- High-volume regions
- High-delay regions
- Geographic bottlenecks
- Factory performance by region

---

## 4. Shipping Mode Analysis

Performance was compared across four shipping methods:

- Same Day
- First Class
- Second Class
- Standard Class

Comparison metrics included:

- Lead Time
- Shipment Volume
- Sales
- Profit
- Cost-Time Trade-off

---

# 📊 Dashboard Features

The interactive dashboard provides comprehensive logistics insights through multiple analytical views.

### KPI Cards

- Total Shipments
- Total Sales
- Total Profit
- Profit Margin
- Average Lead Time
- Delay Frequency

---

### Interactive Filters

Users can filter dashboard results by:

- Date Range
- Factory
- Region
- State / Province
- Ship Mode
- Delay Threshold

---

### Dashboard Pages

#### 📌 Overview

- KPI Summary
- Monthly Sales Trend
- Lead Time Trend
- Top 15 Shipping Routes
- Bottom 10 Shipping Routes
- Product Division Sales Distribution

---

#### 🌍 Geographic & Factory Analysis

- Regional Bottlenecks
- Factory Performance Comparison
- Shipment Volume by Region
- State/Province Lead Time Heatmap

---

#### 🚚 Ship Mode Analysis

- Average Lead Time by Ship Mode
- Shipment Volume Comparison
- Cost vs Time Bubble Chart
- Multi-Metric Radar Chart

---

#### 📍 Route Drill-Down

- Sortable Route Table
- Route Efficiency Scores
- Conditional Performance Indicators

---

# 📉 Data Quality Note

During the analysis, an important data quality issue was identified.

The **Ship Date** values in the source dataset do not represent realistic delivery durations.

Observed lead times range between **900 and 1,642 days**, even for **Same Day Shipping**, while:

- Order Dates fall between **2024–2025**
- Ship Dates extend to **2026–2030**

This indicates that the dataset is **synthetic** or contains artificially generated dates.

To maintain analytical integrity:

- No artificial corrections were applied.
- Lead Time was calculated exactly as defined.
- Relative comparisons between routes, regions, factories, and ship modes remain valid.
- Absolute Lead Time values should not be interpreted as real-world delivery durations.

This approach reflects professional data analysis practices by documenting data quality limitations rather than masking them.

---

# 📊 Dashboard Visualizations

The dashboard includes a variety of interactive visualizations, including:

- Horizontal Bar Charts
- Vertical Bar Charts
- Line Charts
- Bubble Charts
- Doughnut Charts
- Stacked Bar Charts
- Radar Charts
- Heatmaps
- KPI Cards
- Route Ranking Tables

---

# 💡 Key Findings

The analysis revealed several important logistics insights:

- Shipping efficiency varies significantly across factory-to-customer routes.
- Certain factories consistently achieve faster delivery performance.
- Regional bottlenecks increase average shipping lead times.
- Chocolate product divisions contribute the highest shipment volume and sales.
- Differences between shipping methods are relatively small after accounting for the dataset's date anomaly.
- Route-level KPIs provide valuable operational intelligence for logistics planning.

---

# 📋 Business Recommendations

Based on the analysis:

- Continuously monitor route efficiency using standardized KPIs.
- Investigate consistently underperforming shipping routes.
- Improve logistics planning in high-delay regions.
- Optimize factory-to-customer allocation strategies.
- Develop automated route performance dashboards.
- Improve data validation to prevent unrealistic shipment dates.
- Monitor shipping performance through interactive dashboards.

---

# 🚀 Future Enhancements

Potential improvements include:

- Real-time shipment tracking
- Predictive delivery delay modeling
- Machine Learning-based route optimization
- Interactive Streamlit dashboard
- SQL database integration
- Cloud deployment
- Automated reporting


---

# 👨‍💻 Author

**Shivang Sharma**

**Aspiring Data Analyst**

### Skills

- Python
- SQL
- Power BI
- DAX
- Pandas
- Data Visualization
- Business Intelligence

---

# 📄 License

This project uses a **synthetic/sample dataset** for educational and portfolio purposes only.

---

## ⭐ Support

If you found this project useful, consider giving this repository a **Star ⭐** on GitHub.
