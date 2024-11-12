# AWS Data Engineering Tools and Lifecycle Summary

## Source Systems

### Databases
- **Amazon RDS (Relational Database Service)**
  - Provisions database instances (MySQL, PostgreSQL)
  - Handles operational overhead, patching, upgrades
  
- **Amazon DynamoDB**
  - Serverless NoSQL database
  - Virtually unlimited table size
  - Flexible schema
  - Ideal for: gaming, IoT, mobile apps, real-time analytics

### Streaming Sources
- **Amazon Kinesis Data Streams**
  - Used for real-time user activity streaming
  
- **Additional Options**
  - Amazon SQS (Simple Queue Service) for message handling
  - Apache Kafka / Amazon MSK (Managed Streaming for Kafka)

## Data Ingestion

- **Amazon Database Migration Service (DMS)**
  - Automated data migration and replication
  
- **AWS Glue ETL**
  - Primary tool for data integration processes
  
- **Streaming Ingestion Tools**
  - Kinesis Data Streams
  - Amazon Data Firehose
  - SQS
  - Kafka

## Storage Solutions

- **Data Warehouse**
  - Amazon Redshift
  
- **Data Lake**
  - Amazon S3 (Simple Storage Service)
  
- **Lakehouse**
  - Combined approach for accessing structured and unstructured data

## Data Transformation

- **Primary Tools**
  - AWS Glue
  - Apache Spark
  - DBT

## Data Serving

### Business Intelligence & Analytics
- **Query Tools**
  - Amazon Athena
  - Amazon Redshift
  
- **Visualization Options**
  - Jupyter Notebooks
  - Amazon QuickSight
  - Apache Superset (open-source)
  - Metabase (open-source)

### AI/Machine Learning Use Cases
- Batch data for model training
- Vector databases for:
  - Product recommenders
  - Large language model applications

## Note
This summary covers the specific tools mentioned in the courses, but there are numerous other open-source and managed service options available for each stage of the data engineering lifecycle.
