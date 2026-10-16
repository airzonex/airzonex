# Hi, I'm Airat Khaziev

**Data Engineer | 17+ years in software and database development**

I build end-to-end Data Engineering projects focused on data pipelines, DWH, CDC, and analytical data modeling.

My background includes Oracle, SQL, PL/SQL, enterprise application development, business logic, and system integration. I now apply this experience to modern data platforms using Python, PostgreSQL, Airflow, dbt, Kafka, and related technologies.

## Projects

### [Financial Data Platform](https://github.com/airzonex/financial-data-platform)

An end-to-end batch data pipeline for analyzing the relationship between the Bank of Russia key rate and the MOEX RGBI government bond index.

- Ingests financial data from external sources and stores original responses in MinIO.
- Uses PostgreSQL and dbt for staging, intermediate transformations, and analytical marts.
- Orchestrates ingestion and transformations with Apache Airflow.
- Supports incremental processing, ingestion metadata, and idempotent loading.
- Includes automated unit, integration, and end-to-end tests with CI in GitHub Actions.

**Stack:** Python, PostgreSQL, Apache Airflow, dbt, MinIO / S3, Docker Compose, pytest, GitHub Actions.

### [E-commerce Data Platform](https://github.com/airzonex/ecommerce-data-platform)

An end-to-end CDC data platform that captures changes from a PostgreSQL OLTP system and transforms them into analytical dimensions and fact tables.

**Pipeline:** PostgreSQL OLTP → Debezium / Kafka → Python ingestion → PostgreSQL DWH → dbt

- Captures changes from customers, products, orders, order items, and payments using PostgreSQL logical replication and Debezium.
- Implements Kafka-to-DWH ingestion with manual offset management, at-least-once processing, idempotent writes, and replay-safe duplicate handling.
- Stores CDC events in an append-only raw layer with source and Kafka metadata.
- Uses dbt to reconstruct current entity state, handle hard deletes, and build SCD Type 2 dimensions and fact tables.
- Includes unit, integration, CDC streaming, replay/idempotency, and end-to-end pipeline validation.

**Stack:** Python, PostgreSQL, Apache Kafka, Kafka Connect, Debezium, dbt, Docker Compose, pytest.

## Technical Background

| Area | Technologies |
| --- | --- |
| Data pipelines | Python, SQL, Apache Airflow, dbt, REST APIs |
| Databases and DWH | PostgreSQL, Oracle / PL/SQL, ClickHouse |
| CDC and streaming | Apache Kafka, Kafka Connect, Debezium |
| Storage and development | MinIO / S3, Docker Compose, Git, Linux |
| Additional hands-on practice | Apache Spark, Apache NiFi, HDFS |

My professional background includes enterprise application development, database business logic, system integration, and participation in Oracle-to-PostgreSQL migration activities.

## Connect

- [LinkedIn](https://www.linkedin.com/in/airat-khaziev-692783407/)
- [Telegram](https://t.me/airatkhaziev)

Open to full-time remote Data Engineer and DWH Developer opportunities.