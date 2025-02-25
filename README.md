## Project Overview
This project implements a data pipeline that ingests data from various sources, processes it through multiple transformation stages (Bronze, Silver, and Gold layers), and provides the data for reporting and analytics. The pipeline leverages Azure Data Factory for ingestion, Azure Data Lake Gen2 for storage, Databricks for transformation, Azure Synapse for serving, and Power BI for reporting.
### Architecture
The data pipeline follows a structured flow:
1. Data Source: Data is collected from various HTTP endpoints.
2. Data Ingestion: Azure Data Factory orchestrates the ingestion process.
3. Raw Data Store (Bronze Layer): Raw data is stored in Azure Data Lake Gen2.
4. Transformation (Databricks): Data is processed and transformed in Databricks.
5. Transformed Data Store (Silver Layer): Transformed data is stored in Azure Data Lake Gen2.
6. Serving Layer (Gold Layer): Data is aggregated and stored in Azure Synapse for efficient querying.
7. Reporting: Power BI connects to Azure Synapse to generate reports and dashboards.


![DALL·E 2025-02-12 13 12 22 - A professional and structured data architecture diagram titled 'Adventure Works Analytics   ETL on Azure'  The diagram should include_ - 'Data Ingesti](https://github.com/user-attachments/assets/30ee58a5-04ad-4b42-a5e4-83f85b9c1d6f)
