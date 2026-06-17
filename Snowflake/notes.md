# Snowflake notes

## Learn Snowflake - Full 1-Hour crash course for complete beginners

### Overview 

What is snowflake --> It is a cloud native, data platform, SaaS. 

#### Data platform

Snowflake is defined like a cloud data warehousing company, now it is a unified platform and connected ecosystem of data tecnologies.
- At the beggining it was a data warehouse --> Structured and relational data. Data stored in databases, schemas and tables. ANSI Standard SQL. Complex queries.

- Data engineering -> COPY INTO and Snowpipe that streams cloud files into snowflake tables , tasks and streams, Openflow, managed DBT.

Openflow --> Ingest and transform data which connected bases on Apache 95.

Manage DBT --> data transformation steps within dbt call.

It as varios cibersecurity features to protect all the data.

Relational Database --> ACID transactions, High-levels of concurrency, Unistore (HTAP), Hybrid Tables that relates relational and analitycal capabilitical.

Data Lake --> Scalable storage and compute, schema-on-read, Native processing of semistructured data formats. Open lakehouse: Iceberg.

AI / Data Science --> Snowflake Cortex, Snowpark Python, Streamlit, End-to-end Machine Learning with Notebooks.

Data Applications --> Connectors and Drivers, User Defined Functions, External UDFs, Stored Procedures.

#### Cloud Native

Snowflake's software is purpose built for the cloud. Snowflake is not what is called a cloud-washed solution, a port of an older technology migrated to the cloud. 

All the Snowflake infrastructure runs on the cloud in either: original for AWS and expanding for AZURE and Google Cloud.

Snowflake makes use of the cloud's inherent benefits: High availability, scalability, elasticity and durability.

#### Software as a Service (SaaS)

No management of hardware. Transparent updates and patches. It ofers a subscription payment model. Ease of access. Automatic optimisation. 

### Snowflake Architecture

It has a multi-cluster shared data architecture. It has tree diferent architecture layers: Cloud Service Layer -> Query Processing Layer -> Data Storage Layer.

Cloud Services Layer --> Authentication and Access Control -> (Infrastucture management, query optimiser, transaction manager, security) -> Metadata

Query processing layer --> It splits from metadata into : Virtual warehouse. These are compute clusters managed by snowflake.

Data storage layer --> For example AWS S3 that is scalable, available and durable. Compute clases 

