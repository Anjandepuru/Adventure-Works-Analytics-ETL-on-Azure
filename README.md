
## 🚀 Project Overview

This project implements a full-scale **data pipeline architecture** based on the **Modern Data Lakehouse approach**. It ingests data from various sources, processes it through multiple transformation stages—**Bronze, Silver, and Gold layers**—and makes the data available for analytics and business reporting.

The pipeline uses:
- **Azure Data Factory (ADF)** for orchestration
- **Azure Data Lake Storage Gen2** for scalable raw/transformed data storage
- **Databricks** for data transformation and cleansing
- **Azure Synapse Analytics** for the serving layer
- **Power BI** for visualization and insights

---

## 🏗️ Architecture Overview

The pipeline follows a structured and modular flow:

1. **🔹 Data Source**  
   Raw data is collected from various HTTP endpoints or APIs.

2. **🔸 Data Ingestion (ADF)**  
   Azure Data Factory orchestrates the ingestion, storing the raw data in the Bronze layer.

3. **🪵 Bronze Layer (Raw Storage)**  
   Unprocessed data is saved in **Azure Data Lake Gen2** as-is for traceability and auditing.

4. **🔁 Transformation (Databricks)**  
   Using PySpark and Delta Lake, data is cleansed, joined, and enriched within **Databricks Notebooks**.

5. **🔑 Silver Layer (Cleaned & Modeled Data)**  
   Transformed data is saved back into Data Lake Gen2 in a normalized, analytical format.

6. **🏅 Gold Layer (Aggregated / Star Schema)**  
   Final curated datasets are loaded into **Azure Synapse SQL pools** for performant querying.

7. **📊 Reporting (Power BI)**  
   Power BI connects to **Azure Synapse** to build interactive dashboards and reports for stakeholders.

---

This layered approach ensures **data lineage**, **auditability**, **flexibility**, and **performance** across each stage of the pipeline.


![DALL·E 2025-02-12 13 12 22 - A professional and structured data architecture diagram titled 'Adventure Works Analytics   ETL on Azure'  The diagram should include_ - 'Data Ingesti](https://github.com/user-attachments/assets/30ee58a5-04ad-4b42-a5e4-83f85b9c1d6f)
