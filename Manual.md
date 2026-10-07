E-Commerce Sales Analytics — Power BI

A comprehensive E-Commerce Sales Analytics project built with Excel, Power Query, Power BI and DAX to analyze sales performance, products, customers, sales channels, regional performance, orders, returns and revenue targets.

The project transforms transactional e-commerce data into an interactive five-page business intelligence dashboard designed to help management understand what is driving revenue, which products and customers matter most, where sales are concentrated, which channels perform best, and where operational issues require attention.

Dashboard Preview

Page 1 — E-Commerce Overview



The overview page provides a management-level summary of the business, including:

Net Sales

Gross Profit

Total Orders

Units Sold

Average Order Value

Gross Margin

Monthly Net Sales Trend

Revenue by Category

Order Status Distribution

Actual Revenue vs Target

Sales by Channel

Page 2 — Product & Category Analysis



This page evaluates product and category performance through:

Top 10 Products by Units Sold

Top 10 Products by Revenue

Revenue vs Gross Profit

Gross Profit by Category

Gross Margin

Average Selling Price

Category Performance

Category Revenue

Page 3 — Customer Analysis



This page focuses on customer value and purchasing behavior:

Unique Customers

Revenue by Membership

Customer Orders vs Revenue

Average Order Value

Sales per Customer

Revenue by Customer Segment

Customer Detail

Top 10 Customers by Revenue

Customers by State

Page 4 — Regional & Channel Analysis



This page analyzes geographic and channel performance:

Revenue by Zone

Monthly Revenue by Channel

Revenue by State

Channel Performance by Zone

Revenue by Sales Channel

Orders by Payment Method

Average Order Value

Regional Sales Performance

Page 5 — Orders, Returns & Management



This page focuses on operational performance and management risks:

Return Units by Reason

Monthly Return Trend

Order Status Distribution

Category Performance & Risk Summary

Monthly Cancelled Orders

Revenue Target Achievement

Cancelled Order Rate

Return Rate

Revenue Achievement

1. Project Overview

E-Commerce Sales Analytics is a Power BI business intelligence project developed to provide a multi-dimensional view of an e-commerce business.

Rather than focusing only on revenue, the project connects commercial and operational analysis across:

Sales → Products → Customers → Regions → Channels → Orders → Returns → Targets

The dashboard is structured around five analytical areas:

E-Commerce Overview

Product & Category Analysis

Customer Analysis

Regional & Channel Analysis

Orders, Returns & Management

The central objective is to transform raw transaction-level information into business insights that can support better decisions around products, customers, sales channels, regional performance and operational efficiency.

2. Business Problem

E-commerce businesses generate large volumes of transaction, customer, product and operational data.

Looking at total sales alone does not answer important management questions such as:

Which product categories generate the most revenue?

Which products sell the most units?

Which products generate the strongest gross profit?

Which customer segments contribute the most sales?

Which membership groups generate the highest revenue?

Which regions drive the most business?

Which sales channels perform best?

Which payment methods are most frequently used?

How many orders are cancelled or returned?

Why are products being returned?

Are actual revenues meeting the defined targets?

Where are operational problems appearing over time?

This project addresses these questions by combining multiple business dimensions into a single interactive Power BI reporting solution.

3. Project Objectives

The primary objectives of the project are to:

Analyze overall e-commerce sales performance.

Measure gross profit and gross margin.

Evaluate product and category performance.

Identify top-performing products.

Analyze customer segments and membership levels.

Measure customer purchasing behavior.

Compare sales performance across geographic zones and states.

Analyze sales-channel contribution.

Analyze payment-method usage.

Monitor order statuses.

Identify cancellation and return patterns.

Analyze return reasons.

Compare actual revenue with target revenue.

Provide management-oriented insights and recommendations.

4. Key Business Questions

Sales Performance

What is the total net sales value?

What is the total gross profit?

What is the gross margin?

What is the average order value?

How does sales performance change month by month?

Which categories contribute the most revenue?

Product Performance

Which products sell the most units?

Which products generate the highest revenue?

Which categories generate the highest gross profit?

Which categories have the strongest margins?

Are high-revenue products also high-profit products?

Customer Analysis

How many unique customers are purchasing?

Which customer segments generate the most revenue?

Which membership levels contribute the most sales?

What is the average order value?

Which customers generate the highest revenue?

Where are customers geographically concentrated?

Regional & Channel Analysis

Which zone generates the most revenue?

Which states are the strongest contributors?

Which sales channel generates the highest sales?

How does channel performance change over time?

Which payment methods are used most frequently?

Operations

How many orders are delivered, shipped, processing, cancelled or returned?

What are the most common return reasons?

How do returns change over time?

How many orders are cancelled?

Which categories have the highest target achievement?

Is actual revenue exceeding the defined target?

5. Dataset Overview

The Excel workbook contains seven sheets supporting the Power BI analysis.

Sheet

Records

Purpose

Products

100

Product, category, brand and pricing information

Customers

2,000

Customer profiles, segments, membership and geography

Orders

20,000

Transaction-level order data

Returns

1,000

Returned orders, quantities, dates and reasons

Regions

10

Regional, state and zone mapping

Targets

100

Revenue and order targets by category/month

Project_Info

10

Project metadata and information

6. Dataset Structure

Products

The Products table contains product-level information including:

Product_ID

Product_Name

Category

Sub_Category

Brand

Cost_Price

Selling_Price

This table supports product ranking, category analysis, revenue analysis and profitability analysis.

Customers

The Customers table contains customer information including:

Customer_ID

Customer_Name

Gender

Age

Customer_Segment

Membership_Level

City

State

Region_ID

This table supports customer segmentation, membership analysis and geographic customer analysis.

Orders

The Orders table is the primary transaction table and contains:

Order_ID

Order_Date

Customer_ID

Product_ID

Quantity

Unit_Price

Discount

Shipping_Cost

Sales_Channel

Payment_Method

Order_Status

Region_ID

This table provides the foundation for sales, order, customer, channel and operational analysis.

Returns

The Returns table contains:

Return_ID

Order_ID

Product_ID

Return_Date

Return_Quantity

Return_Reason

This table supports return-rate analysis, return-reason analysis and monthly return trends.

Regions

The Regions table maps geography using:

Region_ID

Region

State

Zone

This enables regional and state-level sales analysis.

Targets

The Targets table provides target values used for performance comparison, including:

Month

Category

Target_Revenue

Target_Orders

This enables actual-versus-target analysis.

7. Analytical Data Model

The project combines transactional data with descriptive dimensions.

                         ┌────────────────────┐
                         │      Customers     │
                         │                    │
                         │ Customer_ID        │
                         │ Customer Segment   │
                         │ Membership         │
                         │ Geography          │
                         └─────────┬──────────┘
                                   │
                                   │ Customer_ID
                                   ▼
                         ┌────────────────────┐
                         │       Orders       │
                         │                    │
                         │ Order_ID           │
                         │ Order_Date         │
                         │ Customer_ID        │
                         │ Product_ID         │
                         │ Quantity           │
                         │ Unit_Price         │
                         │ Discount           │
                         │ Channel            │
                         │ Payment            │
                         │ Status             │
                         └───────┬──────┬─────┘
                                 │      │
                     Product_ID  │      │ Region_ID
                                 ▼      ▼
                       ┌────────────┐  ┌────────────┐
                       │ Products   │  │  Regions   │
                       │            │  │            │
                       │ Product    │  │ Region     │
                       │ Category   │  │ State      │
                       │ Brand      │  │ Zone       │
                       │ Cost       │  └────────────┘
                       │ Price      │
                       └────────────┘

                         ┌────────────────────┐
                         │      Returns       │
                         │                    │
                         │ Return_ID          │
                         │ Order_ID           │
                         │ Product_ID         │
                         │ Return_Date        │
                         │ Return_Quantity    │
                         │ Return_Reason      │
                         └────────────────────┘

                         ┌────────────────────┐
                         │      Targets       │
                         │                    │
                         │ Month              │
                         │ Category           │
                         │ Target Revenue     │
                         │ Target Orders      │
                         └────────────────────┘

Note: This is a conceptual representation of the analytical structure based on the supplied workbook fields. The exact Power BI relationship configuration should be verified in the .pbix model before being documented as the final physical schema.

8. KPI Framework

The dashboard focuses on several major business KPIs.

KPI

Reported Value

Business Purpose

Net Sales

₹494.38M

Measures sales after discounts

Gross Profit

₹143.05M

Measures gross profitability

Gross Margin

28.94%

Measures gross profit as a percentage of sales

Total Orders

20K

Measures order volume

Units Sold

41K

Measures product quantity sold

Average Order Value

₹24.72K

Measures average revenue per order

Unique Customers

2K

Measures customer reach

Sales per Customer

₹260.89K

Measures average sales contribution per customer

Return Rate

3.73%

Reported return-rate KPI

Cancelled Orders

1K

Measures cancelled-order volume

Cancelled Order Rate

6.13%

Measures cancellation level

Revenue Achievement

373.57%

Measures actual revenue relative to target

Source: dashboard values visible in the supplied Power BI PDF.

9. Core Business Calculations

The transaction data supports the following analytical logic.

Net Sales

Net Sales =
Quantity × Unit Price × (1 − Discount)

Net sales represents the transaction value after the applied discount.

Gross Profit

The report's gross-profit result is consistent with a product-cost calculation:

Gross Profit =
Net Sales − Product Cost

where product cost is based on quantity and product cost price.

Gross Margin

Gross Margin =
DIVIDE(Gross Profit, Net Sales, 0)

The dashboard reports a gross margin of approximately 28.94%.

Average Order Value

Average Order Value =
DIVIDE(Net Sales, Total Orders, 0)

The dashboard reports approximately ₹24.72K.

10. Page 1 — E-Commerce Overview

The first page acts as the executive dashboard.

Main KPIs

Net Sales — ₹494.38M

Total Orders — 20K

Units Sold — 41K

Average Order Value — ₹24.72K

Gross Profit — ₹143.05M

Gross Margin — 28.94%

Return Rate — 3.73%

Main Visuals

Revenue by Category

Order Status Distribution

Monthly Net Sales Trend

Actual Revenue vs Target

Sales by Channel

Category Revenue

Category

Net Sales

Beauty

₹147.93M

Fashion

₹110.88M

Home & Kitchen

₹92.35M

Electronics

₹77.12M

Sports

₹66.10M

Total

₹494.38M

Business Interpretation

Beauty is the largest revenue-generating category in the supplied report.

The overview also provides a monthly view of revenue, allowing management to identify periods of higher or lower sales performance.

The actual-versus-target visual is particularly useful because it moves the dashboard beyond descriptive reporting into performance management.

11. Page 2 — Product & Category Analysis

The second page focuses on the product portfolio.

Key Analysis

Top 10 Products by Units Sold

Top 10 Products by Revenue

Revenue vs Gross Profit

Gross Profit by Category

Category Performance

Gross Margin

Average Selling Price

Top Products by Units Sold

The report identifies products such as:

Core Skincare 090

Orbit Smartphones 097

UrbanEdge Haircare 075

Vertex Haircare 074

Zenith Smartphones 089

Vertex Outdoor 053

Vertex Smartphones 001

Vibe Haircare 065

Zenith Equipment 054

Nova Appliances 013

Core Skincare 090 is reported at approximately 492 units, while the other leading products range from approximately 463 to 484 units.

Top Products by Revenue

The top revenue-producing products include:

Core Skincare 090 — ₹12.2M

Apex Skincare 012 — ₹11.4M

Vibe Skincare 051 — ₹10.4M

Vertex Outdoor 053 — ₹10.1M

Nova Skincare 076 — ₹10.0M

Zenith Footwear 084 — ₹9.8M

Zenith Home Decor 010 — ₹9.8M

Zenith Laptops 072 — ₹9.5M

Core Mens Wear 091 — ₹9.5M

UrbanEdge Home Decor 016 — ₹9.4M

Category Gross Profit

Category

Gross Profit

Beauty

₹43M

Fashion

₹33M

Home & Kitchen

₹24M

Electronics

₹22M

Sports

₹20M

Business Interpretation

This page allows the business to separate sales volume from profitability.

A product with high units sold may not necessarily generate the highest profit. Similarly, a product with high revenue may have a lower margin.

Therefore, product decisions should consider:

Units Sold + Net Sales + Gross Profit + Gross Margin

rather than relying on one metric.

12. Page 3 — Customer Analysis

The third page examines customer behavior and value.

Key KPIs

Unique Customers — approximately 2K

Net Sales — ₹494.38M

Total Orders — 20K

Average Order Value — ₹24.72K

Sales per Customer — ₹260.89K

Revenue by Customer Segment

The report shows approximately:

Customer Segment

Net Sales

Regular

₹232M

Occasional

₹135M

Premium

₹67M

New

₹61M

Revenue by Membership

Membership

Net Sales

Silver

₹170M

Bronze

₹156M

Gold

₹111M

None

₹58M

None should be interpreted as customers without a recorded membership value unless the business defines it as an explicit membership category.

Customer Analysis

The page also provides:

Customer orders versus revenue.

Top 10 customers by revenue.

Customer distribution by state.

Customer segment detail.

Business Interpretation

The dashboard indicates that Regular customers contribute the largest total revenue among the displayed segments.

However, total segment revenue should not be confused with individual customer value.

For customer strategy, it is useful to compare:

Number of customers

Orders per customer

Average Order Value

Sales per customer

Segment revenue

Customer profitability

13. Page 4 — Regional & Channel Analysis

The fourth page examines where sales happen and through which channels.

Revenue by Zone

Zone

Net Sales

South

₹196M

North

₹140M

West

₹107M

East

₹52M

South is the strongest zone by revenue.

Revenue by State

The leading states shown in the report include:

State

Net Sales

Rajasthan

₹57M

Gujarat

₹56M

West Bengal

₹52M

Karnataka

₹52M

Maharashtra

₹51M

Telangana

₹50M

Tamil Nadu

₹50M

Delhi

₹47M

Kerala

₹43M

Uttar Pradesh

₹36M

Revenue by Sales Channel

The four channels contribute approximately:

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

Payment Methods

The dashboard compares:

Net Banking

UPI

Wallet

Credit Card

Debit Card

Cash on Delivery

Business Interpretation

The channel results are relatively balanced, while the geographic distribution shows a stronger concentration in the South.

This makes the page useful for:

Regional strategy

Channel optimization

Marketing allocation

Geographic expansion

Payment experience analysis

14. Page 5 — Orders, Returns & Management

The fifth page focuses on operational performance.

Order Status

The report shows:

Status

Orders

Share

Delivered

13,996

69.98%

Shipped

1,978

9.89%

Processing

1,637

8.19%

Cancelled

1,225

6.13%

Returned

1,164

~5.82%

Return Reasons

The report identifies:

Late Delivery — 284

Wrong Product — 263

Damaged Product — 262

Product Quality — 259

Size/Fit Issue — 240

Changed Mind — 226

Business Interpretation

Returns are not only a customer-service metric; they can indicate problems across:

Logistics

Product quality

Product descriptions

Warehouse operations

Packaging

Product sizing

Customer expectations

The dashboard therefore helps management move from:

"How many products were returned?"

to:

"Why are products being returned?"

15. Key Business Insights

1. Beauty is the strongest revenue category

Beauty generates approximately ₹147.93M, making it the largest category in the report.

This category should be investigated further to understand whether its performance comes from:

Higher unit volume

Higher prices

Product mix

Customer demand

Channel distribution

2. Gross profitability is significant

The dashboard reports:

Gross Profit — ₹143.05M

Gross Margin — 28.94%

This indicates that profitability is a major analytical dimension of the project rather than the report focusing only on sales.

3. Regular customers are a major revenue contributor

Regular customers contribute approximately ₹232M in net sales.

This indicates the importance of understanding repeat purchasing behavior and customer retention.

4. South is the leading zone

South contributes approximately ₹196M in sales.

The business can compare this against customer count, order volume, product mix and average order value to understand why the zone performs strongly.

5. Sales channels are relatively balanced

Social Commerce, Website, Marketplace and Mobile App each generate approximately ₹120M–₹127M.

This suggests the business does not depend overwhelmingly on a single sales channel.

6. Cancellations are an operational concern

The dashboard reports:

1,225 cancelled orders

6.13% cancellation rate

This creates an opportunity to investigate the causes of cancellations.

7. Returns require root-cause analysis

The dashboard identifies multiple return reasons, with Late Delivery, Wrong Product and Damaged Product among the largest categories.

These results can support targeted operational improvements.

8. Target achievement requires validation

The report displays 373.57% revenue achievement.

This is a very high achievement ratio and should be validated against the target definitions before being presented as a definitive business success.

The dashboard shows the metric, but the exported report alone does not establish whether the target framework is correctly aligned with the actual sales period.

16. Data Quality & Validation Notes

A strong analytics project should document data-quality considerations rather than hiding them.

Return Rate

The dashboard reports a 3.73% return rate.

However, the underlying workbook contains:

20,000 orders

1,000 return records

1,164 orders marked as Returned

These figures imply different possible return-rate definitions.

Therefore, the exact business definition of the 3.73% KPI should be verified in the Power BI model.

Target Achievement

The report displays 373.57% revenue achievement.

The target table should be checked to confirm:

Target granularity

Date alignment

Category alignment

Filter behavior

Target units

Membership

The customer data contains customers without a recorded membership value.

These customers should be treated as missing/unassigned membership unless the business intentionally defines None as a business category.

Returns vs Order Dates

The return dataset extends beyond the latest order date.

This can be legitimate because customers may return purchases after the reporting period closes, but the documentation should clearly distinguish:

Order reporting period

from

Return activity period

Gross Profit Definition

The report's gross profit is consistent with:

Net Sales − Product Cost

The workbook also contains shipping cost information.

Therefore, documentation should clarify whether shipping is intentionally excluded from gross profit or whether another profitability measure should be created.

17. Business Recommendations

Product Strategy

Prioritize high-revenue and high-margin products.

Investigate products with high unit volume but weaker profitability.

Monitor product-level gross margin.

Review category performance regularly.

Customer Strategy

Analyze Regular customers for retention opportunities.

Identify high-value customers.

Compare customer segments using both revenue and order frequency.

Improve membership-data completeness.

Regional Strategy

Maintain strong performance in the South zone.

Investigate lower-performing regions.

Compare customer density, order volume and AOV by region.

Channel Strategy

Continue monitoring all four major sales channels.

Compare channels using revenue, orders and AOV.

Avoid judging channels on revenue alone.

Operations

Investigate cancellation reasons.

Reduce late-delivery returns.

Investigate damaged-product returns.

Monitor wrong-product returns.

Track monthly return trends.

Target Management

Validate target definitions.

Ensure actual and target periods align.

Review targets at category and monthly levels.

18. Project Workflow

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
Interactive Visualizations
    ↓
Business Analysis
    ↓
Insights & Recommendations

19. Tools & Technologies

Technology

Purpose

Microsoft Excel

Source data and initial data inspection

Power Query

Data cleaning and transformation

Power BI Desktop

Data modeling and dashboard development

DAX

KPI and analytical calculations

GitHub

Version control and portfolio presentation

20. Skills Demonstrated

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

Operational Analytics

Target vs Actual Analysis

Data Visualization

Business Storytelling

Management Reporting

21. Repository Structure

E-Commerce-Sales-Analytics/
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

22. Project Information

Item

Details

Project Name

E-Commerce Sales Analytics

Project Type

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

Primary Tools

Excel, Power Query, Power BI, DAX

23. Limitations

Some dashboard KPIs require validation against their exact DAX definitions.

Return-rate calculation should be reconciled with the Returns and Orders tables.

Revenue target achievement should be validated against target definitions and periods.

Customer membership includes missing/unassigned values.

Gross profit should be documented clearly with respect to shipping costs.

Certain dashboard tables may be filtered subsets rather than complete dataset totals.

The dashboard is a portfolio/business intelligence analysis and is not presented as a live production reporting system.

24. Future Improvements

Potential improvements include:

Customer Lifetime Value (CLV)

Customer Cohort Analysis

Customer Churn Prediction

Product Recommendation Analysis

Product Affinity Analysis

Sales Forecasting

Return Prediction

Cancellation Prediction

Channel ROI Analysis

Customer Acquisition Cost

Marketing Campaign Analysis

Inventory Analysis

Automated Power BI refresh

Power BI Service deployment

Row-Level Security

Drill-through customer profiles

What-if target analysis

Advanced forecasting

25. Portfolio Value

This project demonstrates an end-to-end analytical workflow:

Raw Business Data
        ↓
Data Preparation
        ↓
Data Modeling
        ↓
DAX Calculations
        ↓
KPI Development
        ↓
Interactive Dashboard
        ↓
Business Insights
        ↓
Management Recommendations

The project is particularly relevant to roles such as:

Data Analyst

Business Analyst

BI Analyst

Power BI Developer

Business Intelligence Analyst

E-Commerce Analyst

26. AI Assistance

AI tools were used as development and documentation assistance during the project workflow, including support with:

Project planning

Analytical structure

Troubleshooting

Documentation

Business interpretation

Dashboard storytelling

The project should be evaluated based on the implemented Power BI report, source workbook and documented analytical logic.

27. Author

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

28. GitHub Repository Description

Power BI e-commerce analytics dashboard analyzing sales, products, customers, channels, regional performance, orders, returns, profitability and revenue targets using Excel, Power Query and DAX.

29. GitHub Topics

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

30. SEO Keywords

Altamash-Analyst · E-Commerce Sales Analytics · Power BI E-Commerce Dashboard · Power BI Sales Dashboard · E-Commerce Analytics · Sales Analytics · Customer Analytics · Product Analytics · DAX · Power Query · Excel Analytics · Business Intelligence · Data Analyst Portfolio · Power BI Dashboard · Retail Analytics

Conclusion

E-Commerce Sales Analytics is a comprehensive Power BI business intelligence project that brings together sales, products, customers, geography, channels and operational performance into a single analytical solution.

The project goes beyond simply answering "How much did we sell?"

It investigates:

What are we selling?

Who is buying?

Where are customers buying from?

Which channels are generating revenue?

Which products are most valuable?

How profitable are those sales?

What happens after an order is placed?

Why are products being returned?

Are we achieving our targets?

This makes the project a practical example of how Power BI can transform transactional e-commerce data into a structured business intelligence solution for performance monitoring, customer analysis, product strategy, channel management and operational decision-making.
