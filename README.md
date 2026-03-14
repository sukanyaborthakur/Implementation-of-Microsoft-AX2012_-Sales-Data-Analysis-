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
  <br/>
