# WALMART DATA ENGINEERING PROJECT
Building My Walmart Data Pipeline Project End‑to‑End Architecture

Over the past few days, I’ve been developing a Walmart inspired data pipeline project not as part of Walmart, but as a personal build to demonstrate enterprise grade architecture and automation.

Data Sources:
I used Ghost as my main operational database (Agentic DB) and AWS S3 for file storage. Data flows through Change Data Capture (CDC) to ensure real time synchronization between transactional systems and the lakehouse.

Transformation & Modeling:
Within Databricks, I implemented incremental data models and a one‑big‑table approach for optimized querying. dbt handles modular transformations, lineage tracking, and data quality checks.

Orchestration:
Apache Airflow automates the entire workflow from ingestion to transformation ensuring reliability and scalability.

Key Concepts Explained:
• CDC (Change Data Capture): Tracks and applies only changed records, enabling near‑real‑time updates without full reloads.
• SDP (Streaming Data Processing): Processes data continuously as it arrives, improving latency and responsiveness for analytics.
• CI/CD (Continuous Integration/Continuous Deployment): Automates testing and deployment of dbt models and Airflow DAGs, ensuring every change is validated and version controlled.

Outcome:
A fully automated, scalable data pipeline that demonstrates how modern data engineering principles can power retail analytics at scale.


