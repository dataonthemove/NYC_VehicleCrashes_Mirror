# NYC Motor Vehicle Collisions — Microsoft Fabric

Portfolio copy (Active Repo in Azure DevOps) of an end-to-end analytics build on NYC Open Data collision records
(~2.3M crashes, ~6M persons, ~4.5M vehicles). Primary development happens in Azure DevOps;
this mirror is published for demonstration.

**Pipeline:** Socrata API → Lakehouse Delta ingestion (watermark-driven CDC) → Warehouse
Kimball star schema with a contributing-factor bridge → Direct Lake semantic model with a
29-measure DAX layer → Power BI reports.

**Stack:** Fabric Lakehouse & Warehouse, PySpark, T-SQL stored procedures, Data Factory
pipelines, TMDL, Git integration.

Code-first throughout — notebooks, DDL, pipeline JSON, and semantic model TMDL are all
authored locally and version-controlled.

`1_DDL` · `2_Ingest` · `3_Transform` · `4_Model` · `5_Reports`
