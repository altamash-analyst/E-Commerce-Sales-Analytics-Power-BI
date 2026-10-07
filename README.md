# E-Commerce Sales Analytics — Power BI

A Power BI business intelligence project analyzing e-commerce sales, products, customers, sales channels, regional performance, orders, returns, profitability, and revenue targets using Excel, Power Query, Power BI, and DAX.

The project transforms transactional e-commerce data into a five-page interactive dashboard designed to help understand revenue drivers, product performance, customer behavior, regional sales, channel performance, and operational issues.

---

## Dashboard Preview

### 1. E-Commerce Overview

![E-Commerce Overview](Dashboard/Dashboard%201.PNG)

Executive-level overview covering Net Sales, Gross Profit, Total Orders, Units Sold, Average Order Value, Gross Margin, monthly sales trends, category revenue, order status, targets, and sales channels.

### 2. Product & Category Analysis

![Product & Category Analysis](Dashboard/Dashboard%202.PNG)

Analyzes top products, category revenue, gross profit, gross margin, average selling price, and the relationship between revenue and profitability.

### 3. Customer Analysis

![Customer Analysis](Dashboard/Dashboard%203.PNG)

Analyzes customer value, customer segments, membership levels, orders, revenue, Average Order Value, sales per customer, top customers, and customer geography.

### 4. Regional & Channel Analysis

![Regional & Channel Analysis](Dashboard/Dashboard%204.PNG)

Analyzes revenue by zone and state, sales-channel performance, monthly channel trends, payment methods, and regional performance.

### 5. Orders, Returns & Management

![Orders, Returns & Management](Dashboard/Dashboard%205.PNG)

Focuses on order status, cancellations, returns, return reasons, monthly trends, revenue achievement, and operational risks.

---

## Project Overview

The analytical flow of the project is:

**Sales → Products → Customers → Regions → Channels → Orders → Returns → Targets**

The dashboard is structured into five analytical areas:

1. E-Commerce Overview
2. Product & Category Analysis
3. Customer Analysis
4. Regional & Channel Analysis
5. Orders, Returns & Management

The objective is to transform transaction-level data into actionable business intelligence for management decision-making.

---

## Business Questions

This project answers key business questions such as:

- What is driving revenue?
- Which products generate the highest sales and profit?
- Which categories perform best?
- Which customer segments contribute the most revenue?
- Which membership groups generate the most sales?
- Which regions and states perform best?
- Which sales channels generate the most revenue?
- What are the most common payment methods?
- How many orders are cancelled or returned?
- Why are products being returned?
- Are actual revenues meeting targets?
- Where are operational issues occurring?

---

## Dataset

The Excel workbook contains seven analytical datasets:

| Dataset | Records | Purpose |
|---|---:|---|
| Products | 100 | Products, categories, brands and pricing |
| Customers | 2,000 | Customer profiles, segments and geography |
| Orders | 20,000 | Transaction-level order data |
| Returns | 1,000 | Returns, quantities, dates and reasons |
| Regions | 10 | Region, state and zone mapping |
| Targets | 100 | Revenue and order targets |
| Project_Info | 10 | Project metadata |

---

## Key KPIs

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

## Core Business Calculations

### Net Sales

```text
Net Sales =
Quantity × Unit Price × (1 − Discount)

Gross Profit



Gross Profit =
Net Sales − Product Cost

Gross Margin



Gross Margin =
DIVIDE(Gross Profit, Net Sales, 0)

Average Order Value



Average Order Value =
DIVIDE(Net Sales, Total Orders, 0)

Key Business Insights

Product Performance

Beauty is the highest-revenue category at approximately ₹147.93M, followed by Fashion at ₹110.88M and Home & Kitchen at ₹92.35M.

Product performance is evaluated using:

Units Sold + Net Sales + Gross Profit + Gross Margin

This provides a more complete view of product performance than relying on sales volume alone.

Customer Performance

Regular customers contribute approximately ₹232M in revenue, making them the largest displayed customer segment.

The dashboard also compares customer segments, membership levels, orders, Average Order Value, sales per customer, and top customers.

Regional Performance

The South zone is the strongest region with approximately ₹196M in revenue.

Channel Performance

Channel

Net Sales

Social Commerce

₹127M

Website

₹125M

Marketplace

₹122M

Mobile App

₹120M

Sales are relatively balanced across the four major channels.

Operational Performance

Order Status

Orders

Delivered

13,996

Shipped

1,978

Processing

1,637

Cancelled

1,225

Returned

1,164

Major return reasons include:

Late Delivery

Wrong Product

Damaged Product

Product Quality

Size/Fit Issue

Changed Mind

Data Quality & Validation

The project also documents important validation considerations:

The dashboard reports a 3.73% Return Rate, while the workbook contains 1,000 return records and 1,164 orders marked as Returned.

Revenue Achievement is reported as 373.57% and should be validated against target definitions and reporting periods.

Some customers have missing membership values.

Return activity extends beyond the latest order date.

Gross Profit should be clearly defined regarding Shipping Cost.

Some dashboard tables may represent filtered subsets rather than complete dataset totals.

These considerations are documented to maintain transparency in the analytical solution.

Business Recommendations

Product Strategy

Prioritize high-revenue and high-margin products.

Monitor products with high volume but lower profitability.

Track category-level gross margin.

Customer Strategy

Focus on retaining high-value and Regular customers.

Compare customer segments using revenue, orders, and AOV.

Improve membership-data completeness.

Regional Strategy

Maintain strong performance in the South.

Investigate lower-performing regions.

Compare regional customer density, order volume, and AOV.

Channel Strategy

Compare channels using revenue, orders, and AOV.

Continue monitoring all major sales channels.

Avoid judging channel performance using revenue alone.

Operations

Investigate cancellation causes.

Reduce late-delivery returns.

Investigate damaged and wrong-product returns.

Monitor monthly return trends.

Target Management

Validate target definitions.

Align actual and target reporting periods.

Review monthly and category-level targets.

Project Workflow



Excel Data
    ↓
Data Inspection
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

Tools & Technologies

Technology

Purpose

Microsoft Excel

Source data

Power Query

Data cleaning & transformation

Power BI

Data modeling & visualization

DAX

KPI calculations

GitHub

Version control & portfolio

Skills Demonstrated

Power BI Dashboard Development

Data Analysis

Business Intelligence

Power Query

DAX

Data Modeling

KPI Development

E-Commerce Analytics

Sales Analytics

Product Analytics

Customer Analytics

Regional Analysis

Channel Analysis

Return Analysis

Target vs Actual Analysis

Data Visualization

Business Storytelling

Management Reporting

Repository Structure



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

Project Information

Item

Details

Project

E-Commerce Sales Analytics

Type

Power BI Business Intelligence Project

Dashboard Pages

5

Customers

2,000

Orders

20,000

Products

100

Return Records

1,000

Regions

10

Target Records

100

Tools

Excel, Power Query, Power BI, DAX

Future Improvements

Potential extensions include:

Customer Lifetime Value

Customer Cohort Analysis

Churn Prediction

Product Recommendation Analysis

Sales Forecasting

Return Prediction

Cancellation Prediction

Channel ROI Analysis

Customer Acquisition Cost

Inventory Analysis

Power BI Service Deployment

Row-Level Security

Advanced Forecasting

AI Assistance

AI tools were used as development and documentation assistance for project planning, troubleshooting, documentation, business interpretation, and dashboard storytelling.

The final project is based on the implemented Power BI report, source workbook, and documented analytical logic.

Author

Altamash Nizamuddin

Data Analyst

Power BI • Python • MySQL

Mumbai, India

GitHub: @altamash-analyst

Open to opportunities in:

Data Analytics

Business Analysis

Business Intelligence

Power BI Development
