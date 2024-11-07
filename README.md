
<!---
minhstd/minhstd is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

The project contains several components:
- Data Source: here lies the original/business data, coming out from DBMS and other sources like IoT, sensor, etc
- Data Lake: a centralized repository for to store all incoming data
  - Lakehouse: a combination of Data Lake and Data Warehouse, with the ability to store multiple types of data, while still bring the capabiltiy of versioning, log-tracing
- Processing Engine: to ETL/ELT data (in batches), or streaming data from source to target, generally
- Serving Engine: to query/interact with the processed data, with the purpose of analysing, modeling, reporting

The technologies:
- Delta Lake (with Delta Table as part of Spark Lib): the open-source technology / implementation of the Lakehouse concept
- PostgreDB: to store table-like data, and to store metadata of data in Lakehouse
- Minio: Storage engine for data lake
- Kafka: open-source stream processing platform
- Spark: processing engine for huge amount of data
- 
