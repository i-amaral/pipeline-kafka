# Pipeline - Kafka / S3

This repository contains a practical, end-to-end Data Engineering solution. The goal is to orchestrate and process a continuous ETL flow, integrating relational databases to a cloud Data Lake, using an event-driven architecture and distributed processing structured in the Medallion architecture.

### Architecture and Technologies Used

* **Data Source:** Locally deployed PostgreSQL.
* **Messaging and Ingestion:** Apache Kafka operating together with Kafka Connect to extract data from the database and load it into the destination storage.
* **Data Processing:** Apache Spark (via Spark SQL API) for data transformation and refinement.
* **Storage (Data Lake):** Amazon S3, logically structured into Bronze (raw data), Silver (cleaned and filtered data), and Gold (aggregated business data) layers.
* **Infrastructure:** Orchestration of all services (PostgreSQL, Kafka, Connect, etc.) managed via Docker Compose.
