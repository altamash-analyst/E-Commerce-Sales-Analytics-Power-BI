# E-Commerce Sales Analytics — Power BI

A portfolio-ready **Power BI E-Commerce Sales Analytics Dashboard** built with **Excel, Power Query, Power BI, and DAX**. The project analyzes sales, products, customers, regions, sales channels, orders, returns, profitability, and revenue targets through five interactive dashboard pages.

## Dashboard Preview

### 1. E-Commerce Overview
![E-Commerce Overview](PNG/Dashboard%201.PNG)

Executive view of sales, profit, orders, units sold, AOV, gross margin, category performance, channels, and order status.

### 2. Product & Category Analysis
![Product & Category Analysis](PNG/Dashboard%202.PNG)

Product and category performance using revenue, units sold, gross profit, gross margin, and top-product analysis.

### 3. Customer Analysis
![Customer Analysis](PNG/Dashboard%203.PNG)

Customer segments, membership levels, revenue, orders, AOV, sales per customer, and customer performance.

### 4. Regional & Channel Analysis
![Regional & Channel Analysis](PNG/Dashboard%204.PNG)

Regional, state, sales-channel, payment-method, and monthly channel analysis.

### 5. Orders, Returns & Management
![Orders, Returns & Management](PNG/Dashboard%205.PNG)

Order status, cancellations, returns, return reasons, revenue achievement, and operational performance.

---

## Project Overview

**Analytical Flow:**

`Sales → Products → Customers → Regions → Channels → Orders → Returns → Targets`

The project transforms transaction-level e-commerce data into actionable **business intelligence, KPI reporting, and management insights**.

### Key Business Questions

- Which products and categories generate the most revenue?
- Which products contribute the most profit?
- Which customer segments drive sales?
- Which regions and states perform best?
- Which sales channels generate the most revenue?
- What is the order and cancellation performance?
- Why are products being returned?
- How does actual revenue compare with targets?

---

## Dataset

| Dataset | Records | Purpose |
|---|---:|---|
| Products | 100 | Products, categories, brands and pricing |
| Customers | 2,000 | Customer profiles and segments |
| Orders | 20,000 | Transaction-level sales |
| Returns | 1,000 | Returns and return reasons |
| Regions | 10 | Regional and state mapping |
| Targets | 100 | Revenue and order targets |

---

## Key Performance Indicators

| KPI | Value |
|---|---:|
| Net Sales | ₹494.38M |
| Gross Profit | ₹143.05M |
| Gross Margin | 28.94% |
| Total Orders | 20K |
| Units Sold | 41K |
| Average Order Value | ₹24.72K |
| Unique Customers | 2K |
| Sales per Customer | ₹260.89K |
| Return Rate | 3.73% |
| Cancelled Orders | 1K |
| Cancelled Order Rate | 6.13% |
| Revenue Achievement | 373.57% |

---

## Key Insights

### Product Performance
**Beauty** is the highest-revenue category at approximately **₹147.93M**, followed by Fashion at ₹110.88M and Home & Kitchen at ₹92.35M.

### Customer Performance
**Regular customers** contribute approximately **₹232M** in revenue and represent the largest displayed customer segment.

### Regional Performance
The **South zone** is the strongest region with approximately **₹196M** in revenue.

### Channel Performance

| Sales Channel | Net Sales |
|---|---:|
| Social Commerce | ₹127M |
| Website | ₹125M |
| Marketplace | ₹122M |
| Mobile App | ₹120M |

### Order Performance

| Order Status | Orders |
|---|---:|
| Delivered | 13,996 |
| Shipped | 1,978 |
| Processing | 1,637 |
| Cancelled | 1,225 |
| Returned | 1,164 |

Major return reasons include **Late Delivery, Wrong Product, Damaged Product, Product Quality, Size/Fit Issue, and Changed Mind**.

---

## Power BI & DAX Analysis

The dashboard uses measures for core business metrics such as:

- Net Sales
- Gross Profit
- Gross Margin
- Average Order Value
- Units Sold
- Total Orders
- Sales per Customer
- Return Rate
- Cancellation Rate
- Revenue Achievement
- Target vs Actual Analysis

Example calculation logic:

```text
Net Sales =
Quantity × Unit Price × (1 − Discount)

Gross Profit =
Net Sales − Product Cost

Gross Margin =
Gross Profit ÷ Net Sales

Average Order Value =
Net Sales ÷ Total Orders
```

---

## Data Quality & Validation

The project documents important validation considerations:

- Dashboard Return Rate differs from simple return-record and Returned-status calculations.
- Revenue Achievement of **373.57%** should be validated against target definitions and reporting periods.
- Some customer membership values are missing.
- Return activity extends beyond the latest order date.
- Gross Profit should be clearly defined regarding Shipping Cost.
- Some dashboard visuals may represent filtered subsets rather than complete dataset totals.

These checks are included to maintain transparency in the analytical workflow.

---

## Business Recommendations

- Prioritize high-revenue and high-margin products.
- Monitor high-volume products with lower profitability.
- Retain high-value and Regular customers.
- Investigate lower-performing regions.
- Compare channels using revenue, orders, and AOV.
- Investigate cancellation and return causes.
- Reduce late-delivery, damaged-product, and wrong-product returns.
- Validate target definitions and reporting periods.

---

## Project Workflow

```text
Excel Data
    ↓
Power Query
    ↓
Data Cleaning & Transformation
    ↓
Data Modeling
    ↓
DAX Measures
    ↓
KPI Development
    ↓
Power BI Dashboard
    ↓
Business Insights
    ↓
Recommendations
```

---

## Tools & Technologies

| Technology | Purpose |
|---|---|
| Microsoft Excel | Source data |
| Power Query | Data cleaning and transformation |
| Power BI Desktop | Data modeling and visualization |
| DAX | KPI and business calculations |
| GitHub | Portfolio and version control |

---

## Skills Demonstrated

**Power BI · DAX · Power Query · Excel · Data Modeling · Data Analysis · Business Intelligence · KPI Development · E-Commerce Analytics · Sales Analytics · Product Analytics · Customer Analytics · Regional Analysis · Channel Analysis · Return Analysis · Target vs Actual Analysis · Data Visualization · Business Storytelling**

---

## Repository Structure

```text
E-Commerce-Sales-Analytics-Power-BI/
│
├── Ecommerce_Sales_Analytics.pbix
├── Ecommerce_Sales_Analytics.xlsx
├── README.md
│
├── Background/
│   ├── 1.png
│   ├── 2.png
│   ├── 3.png
│   ├── 4.png
│   └── 5.png
│
└── PNG/
    ├── Ecommerce_Sales_Analytics.pdf
    ├── Dashboard 1.PNG
    ├── Dashboard 2.PNG
    ├── Dashboard 3.PNG
    ├── Dashboard 4.PNG
    └── Dashboard 5.PNG
```

---

## Future Enhancements

- Customer Lifetime Value
- Customer Cohort Analysis
- Churn Prediction
- Sales Forecasting
- Return Prediction
- Cancellation Prediction
- Channel ROI Analysis
- Inventory Analysis
- Power BI Service Deployment
- Row-Level Security

---

## AI Assistance

AI tools were used as development and documentation assistance for project planning, troubleshooting, business interpretation, and dashboard storytelling.

The final analysis is based on the implemented Power BI report, source workbook, and documented analytical logic.

---

## Author

**Altamash Nizamuddin**  
Data Analyst  
**Power BI · Python · MySQL**  
Mumbai, India

GitHub: **[@altamash-analyst](https://github.com/altamash-analyst)**

Open to opportunities in:

**Data Analytics · Business Analysis · Business Intelligence · Power BI Development**

---

## GitHub SEO

### Repository Description

> Power BI e-commerce analytics dashboard analyzing sales, products, customers, channels, regional performance, orders, returns, profitability and revenue targets using Excel, Power Query and DAX.

### Recommended Topics

`power-bi` `power-bi-dashboard` `dax` `power-query` `excel` `ecommerce-analytics` `sales-analytics` `customer-analytics` `product-analytics` `business-intelligence` `data-analysis` `data-visualization` `retail-analytics` `kpi-dashboard`
