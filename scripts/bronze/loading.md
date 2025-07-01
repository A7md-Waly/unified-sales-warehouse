# Bronze Layer - Data Loading (SSIS)

This layer contains the raw data extracted directly from the source systems (CRM & ERP). The data is ingested in its original structure using **SQL Server Integration Services (SSIS)**.

---

## 🔄 Data Sources

- 📁 Excel files from CRM system
- 📁 Excel files from ERP system

---

## 🚀 Loading Approach

- SSIS packages are used to automate the extraction and loading process.
- Data is loaded into staging tables in the `bronze` schema.
- No transformation is applied at this stage to preserve data lineage.
- Loading pattern: **Full Load** using `TRUNCATE + INSERT`.
