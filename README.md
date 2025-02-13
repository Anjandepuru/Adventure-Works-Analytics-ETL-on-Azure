## Project Overview
This project implements a data pipeline that ingests data from various sources, processes it through multiple transformation stages (Bronze, Silver, and Gold layers), and provides the data for reporting and analytics. The pipeline leverages Azure Data Factory for ingestion, Azure Data Lake Gen2 for storage, Databricks for transformation, Azure Synapse for serving, and Power BI for reporting.
### Architecture
The data pipeline follows a structured flow:
Data Source: Data is collected from various HTTP endpoints.
Data Ingestion: Azure Data Factory orchestrates the ingestion process.
Raw Data Store (Bronze Layer): Raw data is stored in Azure Data Lake Gen2.
Transformation (Databricks): Data is processed and transformed in Databricks.
Transformed Data Store (Silver Layer): Transformed data is stored in Azure Data Lake Gen2.
Serving Layer (Gold Layer): Data is aggregated and stored in Azure Synapse for efficient querying.
Reporting: Power BI connects to Azure Synapse to generate reports and dashboards.
