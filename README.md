# 📊 ShopClues India Sales Performance Dashboard

A professional **Business Intelligence (BI)** project developed in **Power BI** to analyze ShopClues India's sales performance using interactive dashboards and executive-level KPIs.

This project demonstrates end-to-end data analytics skills, including data preparation, data modeling, DAX calculations, dashboard development, and business insight generation.

---

## 📌 Project Overview

The objective of this project is to provide ShopClues management with a centralized dashboard for monitoring sales performance, profitability, customer behavior, and product trends.

Using transactional sales data, the dashboard enables decision-makers to identify business opportunities, monitor KPIs, and perform interactive analysis through filters and slicers.

---

## 🎯 Business Objectives

- Monitor overall sales performance
- Track profit and order quantity
- Analyze customer purchasing behavior
- Identify top-performing states and customers
- Understand category and sub-category profitability
- Evaluate payment method preferences
- Support data-driven business decisions

---

# 📁 Dataset Information

The project uses two CSV datasets.

### Orders.csv

Contains order-level information including:

- Order ID
- Order Date
- Customer Name
- State

**Total Records:** 500

---

### Details.csv

Contains transaction-level details including:

- Order ID
- Amount
- Profit
- Quantity
- Category
- Sub-Category
- Payment Mode

**Total Records:** 1,500

---

# 🛠 Tools & Technologies

- Microsoft Power BI Desktop
- Power Query
- DAX
- CSV Files
- Data Modeling
- Data Visualization

---

# 🔄 Project Workflow

```text
CSV Files
      │
      ▼
Power Query
(Data Cleaning & Transformation)
      │
      ▼
Data Modeling
(Orders ↔ Details)
      │
      ▼
DAX Measures
      │
      ▼
Interactive Dashboard
      │
      ▼
Business Insights
```

---

# 📊 Dashboard Features

The dashboard provides the following business insights:

### Executive KPIs

- Total Sales Amount
- Total Profit
- Total Quantity Sold
- Average Order Value (Custom DAX Measure)

---

### Interactive Visualizations

- Monthly Profit-Loss Analysis
- Top States by Sales
- Top Customers
- Profit by Sub-Category
- Quantity by Product Category
- Quantity by Payment Mode
- Quarter Slicer
- Interactive Filtering

---

# 📈 Data Model

A **One-to-Many** relationship was created between the two datasets.

```text
Orders
(Order ID)
      │
      │ 1
      ▼
Details
(Order ID)
```

This relationship enables accurate aggregation and cross-filtering across all visualizations.

---

# ⚙ Power Query Transformations

The following transformations were performed during data loading:

- Data type validation
- Column formatting
- Data transformation
- Data model preparation
- Relationship creation

---

# 📐 DAX Measures

### Average Order Value

Custom DAX Measure

```DAX
Average Order Value =
DIVIDE(
    SUM(Details[Amount]),
    DISTINCTCOUNT(Orders[Order ID])
)
```

Other KPIs such as Total Sales, Total Profit, and Total Quantity were generated using Power BI aggregation functions.

---

# 📊 Dashboard Preview

> *(Add your dashboard screenshot here)*

Example:

```
images/dashboard.png
```

Then display it using

```markdown
![Dashboard](images/dashboard.png)
```

---

# 🔍 Key Business Insights

- Maharashtra generated the highest sales.
- Clothing contributed the highest sales quantity.
- Printers were the most profitable sub-category.
- Cash on Delivery (COD) remained the most preferred payment method.
- Monthly profitability showed noticeable seasonal fluctuations.
- Interactive filtering allows management to quickly drill down into business performance.

---

# 💼 Business Recommendations

- Increase inventory for high-performing categories.
- Promote digital payment methods to reduce COD dependency.
- Expand successful product categories into underperforming states.
- Develop customer retention programs for high-value customers.
- Investigate causes of profit decline during low-performing months.

---

# 📚 Project Learnings

During this project, I gained practical experience in:

- Building interactive Power BI dashboards
- Data modeling using relationships
- Power Query data transformation
- Creating custom DAX measures
- Business KPI development
- Dashboard storytelling
- Executive reporting
- Interactive visualization design
- Business insight generation

---

# 🚀 Future Improvements

- Real-time database integration
- SQL Server connectivity
- Predictive sales forecasting
- Customer segmentation analysis
- Profit Margin KPI
- Drill-through reports
- Mobile-optimized dashboard
- Row-Level Security (RLS)

---

# 📂 Repository Structure

```text
ShopClues-India-Sales-Performance-Dashboard/
│
├── Dataset/
│   ├── Orders.csv
│   └── Details.csv
│
├── Dashboard/
│   └── ShopClues Dashboard.pdf
│
├── Documentation/
│   └── Project Documentation.docx
│
├── Images/
│   └── Dashboard.png
│
├── README.md
│
└── LICENSE
```

---

# 👨‍💻 About Me

**Himanshu Gupta**

B.Tech Information Technology

Data Analyst | AWS Cloud Solutions Architect | Aspiring Business Analyst

### Technical Skills

- Power BI
- SQL
- Python
- Excel
- Power Query
- DAX
- AWS Cloud
- Data Visualization
- Business Analytics

---

# ⭐ If you found this project helpful

Please consider giving this repository a **Star ⭐**.

Feedback and suggestions are always welcome!
