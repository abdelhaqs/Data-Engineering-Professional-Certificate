# Data Ingestion: Batch vs. Streaming

As a data engineer, the process of ingesting data from source systems into your data pipeline is a crucial and often challenging part of the data engineering lifecycle. The two main patterns for data ingestion are:

1. **Batch Ingestion**:
   - Batch ingestion involves moving data from source systems to your pipeline in large chunks, either on a predetermined time interval (e.g. once a day) or when the data reaches a pre-set size threshold.
   - Batch processing was the traditional default approach for a long time and remains a practical and popular choice, particularly for analytics and machine learning use cases.

2. **Streaming Ingestion**:
   - Streaming ingestion involves continuously ingesting and providing data to downstream systems in near real-time, with the data being available possibly less than a second after it's produced.
   - This requires the use of specialized tools like event streaming platforms or message queues to ingest the continuous stream of events.
   - Streaming ingestion has become more accessible and popular as the supporting technologies have become more ubiquitous.

When choosing between batch and streaming ingestion, there are several important considerations:

- **Business Use Case**: What actions can you take on real-time data that would be an improvement over batch data? Does the business justify the trade-offs of streaming?
- **Cost and Maintenance**: Will streaming ingestion cost more in terms of time, money, and maintenance compared to batch?
- **Pipeline Impact**: How will the choice of batch vs. streaming influence the rest of your data pipeline?

In many cases, the optimal architecture will involve a combination of both batch and streaming ingestion, rather than a purely streaming-only pipeline. The data engineer's role is to identify the appropriate boundaries between batch and streaming based on the specific requirements.

Other important ingestion considerations include using change data capture (CDC) to trigger ingestion based on source system changes, and deciding whether the source system will push data to you or you will pull it.

The key is to develop a thorough understanding of your source systems and carefully evaluate the trade-offs to determine the most appropriate ingestion approach for your use cases.