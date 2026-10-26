# Google-Cloud
AI and Machine Learning on Google Cloud

### Data Cleaning on Google Cloud

Google Cloud offers several tools and methods for data cleaning (also known as data preparation, preprocessing, or scrubbing), depending on whether you want a code-free visual interface, an automated AI-driven workflow, or code-based engineering pipelines.
The primary Google Cloud services and methods used for data cleaning include:

1. Cloud Dataprep by Alteryx (No-Code Visual Cleaning)

Cloud Dataprep is an intelligent, serverless data preparation service that lets you visually explore, clean, and prepare data without writing code.
• Anomaly Detection: Automatically flags mismatched data types, missing values, duplicates, and outliers.
• Smart Suggestions: Uses machine learning to suggest transformation rules based on your data patterns.
• Integrations: Smoothly imports raw datasets from Google Cloud Storage or BigQuery and exports the cleaned results back into BigQuery for analytics.

2. BigQuery (SQL-Based Data Cleaning)

For data that is already stored or ingested into Google Cloud's data warehouse, BigQuery is highly effective for running massive, scalable data scrubbing queries.
• Built-in Functions: Use SQL functions like REGEXP_REPLACE, COALESCE, SAFE_CAST, and TRIM to fix formatting errors, manage null values, and strip unwanted characters.
• Deduplication: Run QUALIFY ROW_NUMBER() OVER (PARTITION BY ...) to rapidly isolate and remove duplicate rows across billions of data points.

3. Dataflow & Dataproc (Code-Heavy & Advanced Pipelines)

When dealing with streaming data or massive Apache Spark/Hadoop workflows, Google provides managed infrastructure engines:
• Dataflow (Apache Beam): Ideal for unifying batch and streaming pipelines. You can write custom cleaning logic in Python or Java to parse incoming JSON logs, filter out corrupted telemetry, or normalize real-time records.
• Dataproc: A fully managed service for running Spark and Hadoop clusters. Perfect for data engineers who prefer Spark SQL or PySpark scripts to perform large-scale distributed data cleansing.

4. Gemini in Google Data Cloud (AI-Assisted Curation)

Google leverages generative AI to streamline complex data ingestion and processing.
• Automated Code Generation: AI agents can automatically write the necessary SQL or Python transformation code required to clean fragmented, complex "dark data" sitting in Cloud Storage.
• Semantic Cleaning: Moves beyond simple structural formatting to fix data based on a conceptual understanding of the information.

https://cloud.google.com/blog/products/data-analytics/bigquery-data-clean-rooms-now-available-in-public-preview</br>
https://cloud.google.com/use-cases/data-clean-rooms</br>
https://medium.com/@williamwarley/mastering-the-cloud-the-ultimate-guide-to-harnessing-google-clouds-data-analytics-powerhouse-b1aa57cea0c0</br>
https://cloud.google.com/blog/products/ai-machine-learning/what-google-cloud-announced-in-ai-this-month</br>
https://www.linkedin.com/pulse/google-clouds-bigquery-clean-room-comprehensive-guide-prateek-shekhar-mbocc</br>
<a href="https://cloud.google.com/blog/products/data-analytics/data-curation-accelerators-for-google-data-cloud">Accelerating data curation with Google Data Cloud</a></br>
https://cloud.google.com/discover/what-is-data-processing</br>
https://docs.cloud.google.com/bigquery/docs/data-clean-rooms</br>
https://cloud.google.com/blog/products/gcp/google-cloud-platform-adds-new-tools-for-easy-data-preparation-and-integration