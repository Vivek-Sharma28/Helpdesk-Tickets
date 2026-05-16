# Helpdesk-Tickets
Freshdesk Ticket Analytics Pipeline & Power BI Dashboard
## Project Overview

This project demonstrates an end-to-end Data Engineering + Business Intelligence solution built using the Freshdesk API, Azure cloud services, Databricks, Synapse Analytics, and Power BI.

The solution extracts customer support ticket data from Freshdesk, processes and transforms it through a scalable Azure Data Engineering pipeline, and delivers interactive business insights through Power BI dashboards.

### The project focuses on:

Automated API data ingestion
Incremental data loading
Cloud-based ETL pipelines
Scalable data transformation using PySpark
Enterprise Data Warehouse design
Real-time business reporting & analytics

Freshdesk API endpoints used in this project include Tickets, Contacts, Agents, and Companies.

## 🏗️ Architecture

Freshdesk API

      ↓
      
Azure Data Factory (ADF)

      ↓
      
Azure Data Lake Storage Gen2 (RAW Layer)

      ↓
      
Azure Databricks (PySpark Transformations)

      ↓
      
Azure Data Lake Storage Gen2 (Transformed Layer)

      ↓
      
Azure Synapse Analytics (Data Warehouse)

      ↓
      
Power BI Dashboard

## ⚙️ Technologies Used

- Data Engineering
-  Azure Data Factory (ADF)
- Azure Databricks
- PySpark
- Azure Data Lake Storage Gen2
- Azure Synapse Analytics
- REST API Integration
- Incremental Loading
= Reporting & Visualization
= Power BI
- DAX
- Interactive Dashboards
- KPI Monitoring

##  📌 Features Implemented

### 🔹 API Data Ingestion

- Connected with Freshdesk REST APIs
- Automated extraction using ADF pipelines
- Dynamic pagination handling
- Incremental data loading using updated_since

### 🔹 Data Lake Architecture

- RAW layer storage for source JSON files
- Transformed layer for curated datasets
- Date-wise partitioning strategy

### 🔹 Data Transformation

- PySpark-based transformations in Databricks
- Schema flattening
- Data cleansing & enrichment
- Null handling and business logic implementation

### 🔹 Data Warehouse

- Structured analytical tables in Synapse
- Optimized for Power BI reporting
- Historical ticket analysis support

### 🔹 Power BI Dashboard

Interactive dashboards built for:

- Ticket Volume Analysis
- SLA Monitoring
- Agent Performance
- Resolution Trends
- Query Type Analysis
- Customer Support KPIs
  
## 📊 Dashboard Insights

The Power BI dashboard provides:

- Total Tickets
- Open vs Closed Tickets
- Agent-wise Performance
- Average Resolution Time
- Priority Analysis
- Company-wise Ticket Distribution
- Daily/Monthly Ticket Trends
  
## 🔄 Incremental Loading Strategy

Implemented incremental loading using Freshdesk API parameters to fetch only newly updated records instead of full loads, improving:

-  Performance
- Scalability
- Pipeline efficiency
- Cost optimization

### Example API:

/api/v2/tickets?include=stats&updated_since=2025-04-01
📁 API Endpoints Used
Entity	Endpoint
Tickets	/api/v2/tickets?include=stats
Contacts	/api/v2/contacts
Agents	/api/v2/agents
Companies	/api/v2/companies

🔐 Freshdesk API Reference
Freshdesk Account URL:
Freshdesk API Documentation:
🎯 Business Use Case

### This solution helps organizations:

- Monitor customer support operations
- Improve SLA compliance
- Track agent productivity
- Identify ticket trends
- Make data-driven support decisions
  
## 👨‍💻 Developed By

### Vivek Sharma
#### Data Engineer | Azure | Databricks | PySpark | Power BI
