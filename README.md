# Sales Performance Analysis
This project is an end-to-end Sales Analytics and Performance Monitoring dashboard built using Power BI on top of ERP transactional data from Microsoft Dynamics AX
    
The dashboard enables business stakeholders to monitor:
    
   <br/> Current vs Last Year Sales
   <br/> YoY, MTD, and YTD growth trends
    <br/> Dealer-wise and executive-wise performance
    <br/> Target vs Actual and Budget analysis
    <br/> Regional, warehouse, customer, and product insights

 ***Data Architechture***
 
   <br/> **Data Source**
    <br/> *Excel
    <br/> *Microsoft SQL Server
    <br/> *ERP System : Dynamics AX(Production Database)
    
  **Core Fact Table**
    <br/> *Sales Transaction(Query1)
    <br/> *Dealer Target
    <br/> *Executive Budget
    <br/> *Product Sheet

  **Dimension Table**
    <br/>*Calendar(Custom Fiscal year calendar using dax)

  **Built Relationships**
    <br/>The model follows star-schema principles, with a centralized date dimension connected to all fact tables.
    
  **KPI Measured**
    <br/>Total Sales
    <br/>Last Year Sales
    <br/>Last Year Qty
    <br/>Qty value in Lak(CY)
    <br/>Qty value in Lak(LY)
    <br/>Growth
    <br/>Growth%(Sales)
    <br/>Growth%(Qty)
    <br/>Sales 
    <br/>Sales Amount last year
    <br/>Sales YTD
    <br/>YTD Last Year Sales
    <br/>MTD Current Year
    <br/>MTD Previous Year
    <br/>MTD Current VS Previous Year
    <br/>Sales FYTD
    <br/>Sales FYTD Previous
    <br/>YOY Sales growth
    <br/>YTD Sales Current Year in Lak
    <br/>YTD Sales Last Year in Lak
    <br/>Yoy Growth percentage(Lak)

   **Dashboard Pages**
    <br/>Overview
    <br/>Dealer
    <br/>Sales Analysis
    <br/>Sales Details Report 
    <br/>Warehouse Sales Analysis
    <br/>Daily Sales Analysis
    <br/>Item Sales Analysis
    <br/>Sales Person Analysis
  
    
  **Tools and Technologies**
     <br/> ***Excel***
     <br/> ***SQL Server***
     <br/> ***Power BI Desktop***
     <br/> ***Microsoft Dynamics AX(Source ERP)***


**Business Value**
  <br/>-Track sales growth and performance trends
  <br/>-Monitor targets and budgets effectively
  <br/>-Identify high and low performing regions, warehouses, and dealers
  <br/>-Enable data-driven decision-making for Sales Executives






  # Executive Sales Vs Target Analysis
 **Project Overview**

This project focuses on analyzing sales performance against targets using an interactive Power BI dashboard. The report enables stakeholders to monitor business performance across executives, customers, locations, and product groups, helping identify top performers, underperforming regions, and customer contribution to overall sales.


**Business Problem**

Sales teams often struggle to quickly evaluate performance against targets across multiple regions and executives. Static reports make it difficult to identify performance gaps and understand the drivers behind sales achievement.

This dashboard solves that problem by providing a dynamic and interactive performance monitoring tool that enables faster decision-making.

***Data Architechture***
 
   <br/> **Data Source**
    <br/> *Excel
    <br/> *Microsoft SQL Server
    <br/> *ERP System : Dynamics AX(Production Database)

**Core Fact Table**
    <br/> *Sales Transaction(Query1)
    <br/> *Target_Data23-24
    
    

**Dimension Table**
    <br/>*Calendar(Custom Fiscal year calendar using dax)
    
 **Built Relationships**
    <br/>The model follows star-schema principles. 
     <br/>Query1[Custinvoicetrans Date]  →  Calendar[Date]
     <br/>Cardinality: Many-to-One
     <br/>Cross Filter: Single
     <br/>This relationship allows sales data to be filtered by date, enabling visuals like:
<br/>-Monthly sales trends
<br/>-Yearly comparisons
<br/>-Fiscal year analysis
     <br/>Query1[Unique ID] → Target_Data23-24[UniqueID]
     <br/>Cardinality: Many-to-One
     <br/>Cross Filter: Single
     <br/>This relationship connects actual sales with target values.
<br/>This allows calculation of:
<br/>-Achievement %
<br/>-Variance
<br/>-Sales vs Target

 **KPI Measured**
  <br/>Achievement
  <br/>Variance
  <br/>Variance Color
  <br/>Top 10 Executive Color
  <br/>Top 5 Location
  <br/>GRP Target Total
  <br/>Monthly Target
  <br/>Last Year Sales
  <br/>Actual Sales
  <br/>Button label
  <br/>KPI Executive Title
  <br/>KPI Location Title

  **Dashboard Pages**
    <br/>Executive Overview
    <br/>Location wise customer Sales vs Target
    <br/>DTCustomer details
    <br/>DTexecutive details  

   **Tools and Technologies**
     <br/> ***Excel***
     <br/> ***SQL Server***
     <br/> ***Power BI Desktop***
     <br/> ***Microsoft Dynamics AX(Source ERP)***  

**Business Value**
  <br/>-Real-time Performance Monitoring
  <br/>-Executive Performance Evaluation
  <br/>-Target Effectiveness Assessment
  <br/>-Regional Sales Insights
  <br/>-Customer Revenue Contribution
  <br/>-Data-Driven Sales Strategy
  <br/>-Improved Reporting Efficiency

  **Key Insights from this Dashboard**
  
<br/>Insight 1 — Sales far exceed targets
<br/>Total sales significantly surpass targets, indicating **very high achievement levels.**
<br/>This suggests either:
<br/>-Strong market demand
<br/>-Targets set conservatively

<br/>Insight 2 — Extreme achievement percentages
Some executives show **achievement above 4000%**.
<br/>Example:
<br/>Executive	Sales	Target	Achievement
<br/>Sanjay	435K	9K	4835%
<br/>This indicates **target imbalance**, where targets assigned to some executives are very small relative to their sales performance.

<br/>Insight 3 — Sales concentration among a few executives
<br/>Executive performance charts show that **a few executives contribute disproportionately to total sales.**
<br/>This suggests:
<br/>Unequal account allocation
<br/>Key executives managing high-value customers

<br/>Insight 4 — Location performance differences
<br/>Locations show different levels of performance.
<br/>Example:
<br/>Location	Variance
<br/>Delhi	+268%
<br/>Ahmedabad	+110%
<br/>Bangalore	+80%
<br/>This indicates varying **regional market performance.**

<br/>Insight 5 — Customer revenue concentration
<br/>A small number of customers generate a large portion of revenue, creating **customer concentration risk.**
<br/>Losing one major customer could significantly impact total sales.


**Based on Analysis**
<br/>*1️. Re-evaluate target allocation*
<br/>Targets should be redistributed so they reflect realistic sales potential for each executive or region.

<br/>Why this matters:
<br/>In your dashboard some executives show very high achievement (e.g., 4835%). This usually happens when the assigned target is too small compared to the actual sales potential.

<br/>Example:
<br/>Executive	Sales	Target	Achievement
<br/>Sanjay	₹4,35,211	₹9,000	4835%
<br/>Here the target is extremely low. Even moderate sales produce a very high achievement percentage.

<br/>Recommendation:
<br/>Targets should be distributed based on:
<br/>Past sales performance
<br/>Market potential
<br/>Customer portfolio size

<br/>For example:
<br/>Executive	New Target
<br/>Sanjay	₹3,50,000 instead of ₹9,000
<br/>This would create fairer performance evaluation.

<br/>*2️. Balance customer distribution*
<br/>High-value accounts should be distributed among multiple executives.
<br/>Some executives may be handling high-value customers, which gives them a large advantage over others.

<br/>Why this matters:
<br/>If one executive manages multiple high-revenue customers, their sales will naturally be higher than others.

<br/>Example:
<br/>Executive	Customer	Sales
<br/>Executive A	Customer X	₹50M
<br/>Executive A	Customer Y	₹40M
<br/>Executive B	Customer Z	₹5M
<br/>Executive A will always appear as the top performer, even if Executive B is working just as hard.

<br/>Recommendation:
<br/>Distribute large customers among multiple executives.

<br/>Example:
<br/>Executive	Customer
<br/>Executive A	Customer X
<br/>Executive B	Customer Y
<br/>This leads to balanced sales opportunities.

<br/>*3️. Improve regional strategies*
<br/>Dashboard shows differnct performance across locations. Locations which are not performing well or in underperforming stage should be focused on targeted sales strategies.


<br/>Example:
<br/>Location	Target	Sales	Achievement
<br/>Delhi	     ₹9M	₹36M	268%
<br/>Bangalore	 ₹57M	₹103M	80%
<br/>Delhi greatly exceeds expectations while Bangalore is below target.

<br/>Possible reasons:
<br/>   Market demand differences
<br/>   Competition levels
<br/>   Sales team performance
<br/>   Customer concentration

<br/>Recommendation:
<br/>For underperforming regions
<br/> -Introduce sales campaigns
<br/> -Offer promotional pricing
<br/> -Assign additional sales representatives
<br/> -This can help improve regional performance.

<br/>*4️. Expand customer base*
<br/>Reducing dependency on a few large customers will reduce revenue risk.
<br/>The dashboard suggests that a few customers contribute a large portion of total revenue.

<br/>Why this is risky:
<br/>If one major customer stops buying, total sales could drop significantly.

<br/>Example:
<br/>Customer	Sales Contribution
<br/>Customer A	₹100M
<br/>Customer B	₹90M
<br/>Customer C	₹5M
<br/>  Here Two customers are responsible for most of the revenue. If Customer A leaves, sales could drop from ₹195M to ₹95M.

<br/>Recommendation:
<br/>Businesses should
<br/>  -Acquire new customers
<br/>  -Expand into new markets
<br/>  -Diversify customer segments
<br/>  -This reduces revenue dependency risk.
