# Hi, I'm Airat Khaziev

**Data Engineer | 17+ years in software and database development**

I'm transitioning from senior Oracle and Delphi development to Data Engineering, building on extensive experience with SQL, PL/SQL, business logic, and system integration.

I build personal projects focused on batch ingestion, change data capture, data warehouses, and analytical data modeling. My focus is on reliable pipelines, reproducible environments, and clear documentation.

## Projects

### [Financial Data Platform](https://github.com/airzonex/financial-data-platform)

An end-to-end batch pipeline for analyzing the relationship between the Bank of Russia key rate and the MOEX RGBI government bond index.

- Ingests data from the MOEX API and the Bank of Russia website.
- Stores original responses in MinIO and loads source data into PostgreSQL.
- Uses dbt for SQL transformations, type conversion, date gap filling, and an analytical mart.
- Orchestrates workflows with Airflow and tracks incremental ingestion through run metadata.
- Runs in Docker Compose for a reproducible local setup.

**Stack:** Python, PostgreSQL, Airflow, dbt, MinIO / S3, Docker.

### [E-commerce Data Platform — in progress](https://github.com/airzonex/ecommerce-data-platform)

A CDC-based pipeline that captures changes from an e-commerce PostgreSQL database and ingests them into a warehouse event log.

**Current pipeline:** PostgreSQL OLTP → Debezium → Kafka → Python consumer → PostgreSQL DWH.

- Models customers, products, orders, order items, and payments in the source database.
- Parses CDC events, including deletes and Kafka tombstones.
- Uses an idempotent event log keyed by Kafka topic, partition, and offset.
- Commits Kafka offsets after the database transaction succeeds.
- Includes parser unit tests and scripts for checking CDC and end-to-end ingestion.

**Next steps:** warehouse models, dbt transformations, and customer/order data marts. A ClickHouse real-time analytics branch is planned.

**Stack:** Python, PostgreSQL, Debezium, Kafka, Docker, pytest.

## Technical background

| Area | Technologies |
| --- | --- |
| Data pipelines | Python, SQL, Airflow, dbt, REST APIs |
| Databases and analytics | PostgreSQL, Oracle / PL/SQL, ClickHouse |
| CDC and streaming | Kafka, Debezium |
| Storage and development | MinIO / S3, Docker Compose, Git, Linux |
| Additional hands-on practice | Apache Spark, Apache NiFi, HDFS |

My professional background includes enterprise application development, database business logic, system integration, and participation in Oracle-to-PostgreSQL migration activities.

## Connect

- [LinkedIn](https://www.linkedin.com/in/airat-khaziev-692783407/)
- [Telegram](https://t.me/airatkhaziev)

Open to full-time remote Data Engineer and DWH Developer opportunities.
