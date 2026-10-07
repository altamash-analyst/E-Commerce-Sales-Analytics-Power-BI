Done. I regenerated the complete README.md and included the five dashboard PNGs from your repository structure using the correct relative paths:

PNG/Dashboard 1.PNG
PNG/Dashboard 2.PNG
PNG/Dashboard 3.PNG
PNG/Dashboard 4.PNG
PNG/Dashboard 5.PNG

It also includes the project overview, business problem, dataset, data model, KPIs, segmentation, RFM analysis, dashboard documentation, insights, recommendations, limitations, workflow, repository structure, author section, GitHub description, topics, and SEO keywords.

Download the regenerated README:

Download README.md

Important: Put this README.md in the root of your GitHub repository, alongside the PNG, Background, .pbix, and .xlsx files. The dashboard images will then render automatically on GitHub. 

README.md
Document
Yesterday 6:42 PM
Ecommerce_Sales_Analytics.pbix
File
Ecommerce_Sales_Analytics.xlsx
Spreadsheet
Ecommerce_Sales_Analytics.pdf
PDF
Analyst this in depth and summarize it what is it about because I will me writing a documentation about it
Ecommerce_Sales_Analytics_README(2).md
File
Use this and summarize it so I can use it in GitHub but keep it under 300 Lines and I want Screenshots in it as well 

Yes. I reviewed the README you uploaded. It is currently 1,223 lines, so it is much longer than what you need for a GitHub project README.

I recommend reducing it to around 150–200 lines while keeping the important portfolio content and all 5 dashboard screenshots.

Here is the summarized GitHub-ready version:

# E-Commerce Sales Analytics — Power BI

A Power BI business intelligence project analyzing e-commerce sales, products, customers, sales channels, regional performance, orders, returns, profitability, and revenue targets using Excel, Power Query, Power BI, and DAX.

The project transforms transactional e-commerce data into a five-page interactive dashboard designed to answer key business questions around revenue, profitability, customers, products, channels, regions, and operational performance. :contentReference[oaicite:1]{index=1}

---

## Dashboard Preview

### 1. E-Commerce Overview

![E-Commerce Overview](PNG/Dashboard%201.PNG)

Executive-level overview covering Net Sales, Gross Profit, Total Orders, Units Sold, Average Order Value, Gross Margin, monthly sales trends, category revenue, order status, targets, and sales channels. :contentReference[oaicite:2]{index=2}

### 2. Product & Category Analysis

![Product & Category Analysis](PNG/Dashboard%202.PNG)

Analyzes top products, category revenue, gross profit, gross margin, average selling price, and the relationship between revenue and profitability. :contentReference[oaicite:3]{index=3}

### 3. Customer Analysis

![Customer Analysis](PNG/Dashboard%203.PNG)

Analyzes customer value, customer segments, membership levels, orders, revenue, Average Order Value, sales per customer, top customers, and customer geography. :contentReference[oaicite:4]{index=4}

### 4. Regional & Channel Analysis

![Regional & Channel Analysis](PNG/Dashboard%204.PNG)

Analyzes revenue by zone and state, sales-channel performance, monthly channel trends, payment methods, and regional performance. :contentReference[oaicite:5]{index=5}

### 5. Orders, Returns & Management

![Orders, Returns & Management](PNG/Dashboard%205.PNG)

Focuses on order status, cancellations, returns, return reasons, monthly trends, revenue achievement, and operational risks. :contentReference[oaicite:6]{index=6}

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

The objective is to transform transaction-level data into actionable business intelligence for management decision-making. :contentReference[oaicite:7]{index=7}

---

## Business Questions

This project answers questions such as:

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

---

## Dataset

The Excel workbook contains seven analytical tables:

| Dataset | Records | Purpose |
|---|---:|---|
| Products | 100 | Products, categories, brands and pricing |
| Customers | 2,000 | Customer profiles, segments and geography |
| Orders | 20,000 | Transaction-level order data |
| Returns | 1,000 | Returns, quantities, dates and reasons |
| Regions | 10 | Region, state and zone mapping |
| Targets | 100 | Revenue and order targets |
| Project_Info | 10 | Project metadata |

The Orders table provides the primary transactional foundation, while Products, Customers, Regions, Returns, and Targets support the broader analytical model. :contentReference[oaicite:8]{index=8}

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

These are the reported dashboard values from the supplied project documentation. :contentReference[oaicite:9]{index=9}

---

## Core DAX / Business Calculations

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

The dashboard reports approximately ₹24.72K Average Order Value and 28.94% Gross Margin.

Key Business Insights
Product Performance

Beauty is the highest-revenue category at approximately ₹147.93M, followed by Fashion at ₹110.88M and Home & Kitchen at ₹92.35M.

The project compares product performance using:

Units Sold + Net Sales + Gross Profit + Gross Margin

rather than relying on a single KPI.

Customer Performance

Regular customers contribute approximately ₹232M in revenue, making them the largest displayed customer segment.

Regional Performance

The South zone is the strongest region with approximately ₹196M in revenue.

Channel Performance

Sales are relatively balanced across:

Social Commerce — ₹127M
Website — ₹125M
Marketplace — ₹122M
Mobile App — ₹120M

Operational Performance

The dashboard reports:

13,996 Delivered orders
1,978 Shipped
1,637 Processing
1,225 Cancelled
1,164 Returned

Major return reasons include Late Delivery, Wrong Product, Damaged Product, Product Quality, Size/Fit Issue, and Changed Mind.

Data Quality & Validation

Several metrics should be validated before being treated as final business KPIs:

The dashboard reports a 3.73% Return Rate, while the workbook contains 1,000 return records and 1,164 orders marked as Returned.
Revenue Achievement is reported as 373.57% and should be validated against target definitions and reporting periods.
Some customers have missing membership values.
Return activity extends beyond the latest order date.
Gross Profit should be clearly defined regarding Shipping Cost.
Some dashboard tables may represent filtered subsets rather than complete dataset totals.

These points are documented to make the analytical solution transparent and reproducible.

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
Technology	Purpose
Microsoft Excel	Source data
Power Query	Data cleaning & transformation
Power BI	Data modeling & visualization
DAX	KPI calculations
GitHub	Version control & portfolio
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
Item	Details
Project	E-Commerce Sales Analytics
Type	Power BI Business Intelligence Project
Dashboard Pages	5
Customers	2,000
Orders	20,000
Products	100
Return Records	1,000
Regions	10
Target Records	100
Tools	Excel, Power Query, Power BI, DAX
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

AI tools were used as development and documentation assistance for project planning, troubleshooting, documentation, business interpretation, and dashboard storytelling. The final project is based on the implemented Power BI report, source workbook, and documented analytical logic.

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
GitHub Repository Description

Power BI e-commerce analytics dashboard analyzing sales, products, customers, channels, regional performance, orders, returns, profitability and revenue targets using Excel, Power Query and DAX.

Topics
power-bi
power-query
dax
excel
ecommerce-analytics
sales-analytics
customer-analytics
product-analytics
business-intelligence
data-analysis
power-bi-dashboard
retail-analytics
Conclusion

E-Commerce Sales Analytics demonstrates how transactional e-commerce data can be transformed into an interactive Power BI business intelligence solution.

The project goes beyond total sales to analyze:

What are we selling?
Who is buying?
Where are customers buying from?
Which channels generate revenue?
Which products are most valuable?
How profitable are sales?
What happens after an order is placed?
Why are products being returned?
Are targets being achieved?

This makes the project a practical portfolio example of Power BI, DAX, Power Query, Excel, data modeling, KPI development, business analysis, and management reporting.


### Important

Your screenshots will work on GitHub **only if this structure is preserved**:

```text
E-Commerce-Sales-Analytics-Power-BI/
│
├── README.md
│
└── PNG/
    ├── Dashboard 1.PNG
    ├── Dashboard 2.PNG
    ├── Dashboard 3.PNG
    ├── Dashboard 4.PNG
    └── Dashboard 5.PNG

The five screenshot paths in the README already match the PNG folder and filenames documented in your original README.

This version is much better for GitHub: it keeps the screenshots, KPIs, business insights, dataset, DAX logic, tools, skills, structure, author information, and SEO keywords without the 1,200+ line documentation becoming overwhelming.

Provide it as a single file so I will just copy it and paste it 

Absolutely. Copy everything below directly into your README.md file.

# E-Commerce Sales Analytics — Power BI

A Power BI business intelligence project analyzing e-commerce sales, products, customers, sales channels, regional performance, orders, returns, profitability, and revenue targets using Excel, Power Query, Power BI, and DAX.

The project transforms transactional e-commerce data into a five-page interactive dashboard designed to help understand revenue drivers, product performance, customer behavior, regional sales, channel performance, and operational issues.

---

## Dashboard Preview

### 1. E-Commerce Overview

![E-Commerce Overview](PNG/Dashboard%201.PNG)

Executive-level overview covering Net Sales, Gross Profit, Total Orders, Units Sold, Average Order Value, Gross Margin, monthly sales trends, category revenue, order status, targets, and sales channels.

### 2. Product & Category Analysis

![Product & Category Analysis](PNG/Dashboard%202.PNG)

Analyzes top products, category revenue, gross profit, gross margin, average selling price, and the relationship between revenue and profitability.

### 3. Customer Analysis

![Customer Analysis](PNG/Dashboard%203.PNG)

Analyzes customer value, customer segments, membership levels, orders, revenue, Average Order Value, sales per customer, top customers, and customer geography.

### 4. Regional & Channel Analysis

![Regional & Channel Analysis](PNG/Dashboard%204.PNG)

Analyzes revenue by zone and state, sales-channel performance, monthly channel trends, payment methods, and regional performance.

### 5. Orders, Returns & Management

![Orders, Returns & Management](PNG/Dashboard%205.PNG)

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
Channel	Net Sales
Social Commerce	₹127M
Website	₹125M
Marketplace	₹122M
Mobile App	₹120M

Sales are relatively balanced across the four major channels.

Operational Performance
Order Status	Orders
Delivered	13,996
Shipped	1,978
Processing	1,637
Cancelled	1,225
Returned	1,164

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
Technology	Purpose
Microsoft Excel	Source data
Power Query	Data cleaning & transformation
Power BI	Data modeling & visualization
DAX	KPI calculations
GitHub	Version control & portfolio
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
Item	Details
Project	E-Commerce Sales Analytics
Type	Power BI Business Intelligence Project
Dashboard Pages	5
Customers	2,000
Orders	20,000
Products	100
Return Records	1,000
Regions	10
Target Records	100
Tools	Excel, Power Query, Power BI, DAX
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
GitHub Repository Description

Power BI e-commerce analytics dashboard analyzing sales, products, customers, channels, regional performance, orders, returns, profitability and revenue targets using Excel, Power Query and DAX.

GitHub Topics
power-bi
power-query
dax
excel
ecommerce-analytics
sales-analytics
customer-analytics
product-analytics
business-intelligence
data-analysis
power-bi-dashboard
retail-analytics
Conclusion

E-Commerce Sales Analytics demonstrates how transactional e-commerce data can be transformed into an interactive Power BI business intelligence solution.

The project goes beyond total sales to analyze:

What are we selling?

Who is buying?

Where are customers buying from?

Which channels generate revenue?

Which products are most valuable?

How profitable are sales?

What happens after an order is placed?

Why are products being returned?

Are targets being achieved?

This project demonstrates practical skills in Power BI, DAX, Power Query, Excel, data modeling, KPI development, business analysis, data visualization, and management reporting.


This is the version I recommend you use as your actual GitHub `README.md`. The five screenshot references are already included and match the `PNG` folder structure from your uploaded README. :contentReference[oaicite:0]{index=0}

Available next action: :contentReference[oaicite:1]{index=1}
Pasted markdown.md
File
Provide this as a Readme.md 

Done. I’ve prepared the content as a README.md based on the file you provided, including all five dashboard screenshots and the GitHub-ready sections.

The direct file creation hit a runtime permission issue, so I can’t truthfully provide a download link for a newly created file yet. 



# E-Commerce Sales Analytics — Power BI

A Power BI business intelligence project analyzing e-commerce sales, products, customers, sales channels, regional performance, orders, returns, profitability, and revenue targets using Excel, Power Query, Power BI, and DAX.

The project transforms transactional e-commerce data into a five-page interactive dashboard designed to help understand revenue drivers, product performance, customer behavior, regional sales, channel performance, and operational issues.

---

## Dashboard Preview

### 1. E-Commerce Overview

![E-Commerce Overview](PNG/Dashboard%201.PNG)

Executive-level overview covering Net Sales, Gross Profit, Total Orders, Units Sold, Average Order Value, Gross Margin, monthly sales trends, category revenue, order status, targets, and sales channels.

### 2. Product & Category Analysis

![Product & Category Analysis](PNG/Dashboard%202.PNG)

Analyzes top products, category revenue, gross profit, gross margin, average selling price, and the relationship between revenue and profitability.

### 3. Customer Analysis

![Customer Analysis](PNG/Dashboard%203.PNG)

Analyzes customer value, customer segments, membership levels, orders, revenue, Average Order Value, sales per customer, top customers, and customer geography.

### 4. Regional & Channel Analysis

![Regional & Channel Analysis](PNG/Dashboard%204.PNG)

Analyzes revenue by zone and state, sales-channel performance, monthly channel trends, payment methods, and regional performance.

### 5. Orders, Returns & Management

![Orders, Returns & Management](PNG/Dashboard%205.PNG)

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
Channel	Net Sales
Social Commerce	₹127M
Website	₹125M
Marketplace	₹122M
Mobile App	₹120M

Sales are relatively balanced across the four major channels.

Operational Performance
Order Status	Orders
Delivered	13,996
Shipped	1,978
Processing	1,637
Cancelled	1,225
Returned	1,164

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
Technology	Purpose
Microsoft Excel	Source data
Power Query	Data cleaning & transformation
Power BI	Data modeling & visualization
DAX	KPI calculations
GitHub	Version control & portfolio
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
Item	Details
Project	E-Commerce Sales Analytics
Type	Power BI Business Intelligence Project
Dashboard Pages	5
Customers	2,000
Orders	20,000
Products	100
Return Records	1,000
Regions	10
Target Records	100
Tools	Excel, Power Query, Power BI, DAX
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
Close
