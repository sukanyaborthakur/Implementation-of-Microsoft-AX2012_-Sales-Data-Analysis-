# Sales Performance Target & Budget Analysis
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
