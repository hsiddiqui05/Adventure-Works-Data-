# Azure Data Engineering Project – AdventureWorks

## Project Overview
This project demonstrates an end-to-end Azure Data Engineering pipeline using
Azure Data Factory, Azure Data Lake Gen2, Azure Databricks, and SQL Serverless.

The pipeline follows the Medallion Architecture:
Bronze → Silver → Gold.

## Architecture
- Source: AdventureWorks CSV files
- Ingestion: Azure Data Factory
- Storage: Azure Data Lake Gen2
- Transformation: Azure Databricks (PySpark)
- Serving Layer: Azure Synapse Serverless SQL
- Visualization: Power BI (optional)

## Architecture Diagram
(attach image here)

## Tools & Services Used
- Azure Data Factory
- Azure Data Lake Gen2
- Azure Databricks
- Azure Synapse Analytics (Serverless SQL)
- PySpark
- SQL
- GitHub

## Medallion Architecture
### Bronze Layer
- Raw CSV files ingested using ADF
- No transformation

### Silver Layer
- Data cleaning and transformation using PySpark
- Converted to Parquet
- Stored in Silver container

### Gold Layer
- SQL views created using OPENROWSET
- Optimized for analytics and reporting

## Key Transformations
- Date parsing and type casting
- Union of yearly sales data (2015–2017)
- Derived columns (Month, Year, FullName)
- Schema standardization

## Status
⚠ Azure services were provisioned using a free trial and are currently inactive.
All scripts, architecture, and logic are available in this repository.
Data_Engineering_Project
