# Awesome-Distributed-SQL-Query-Engines

## Top Distributed SQL Query Engines Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Federated Queries, Lakehouse Analytics & Massive Parallel Processing*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Distributed SQL Query Engines**. These tools enable organizations to query massive datasets across data lakes, warehouses, and databases—from federated engines that read data where it lives to MPP warehouses that optimize storage and compute together.



**Examples** include Trino, Presto, AWS Athena, Starburst Galaxy, Dremio Cloud, Snowflake, Google BigQuery, Amazon Redshift, Databricks SQL, and Teradata Vantage (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, federated querying, and open lakehouse infrastructure—ideal for data engineers, analysts, and organizations seeking transparent, vendor-independent SQL analytics.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **AWS Athena**

  **Serverless interactive analytics service** for querying data in S3 using SQL or Apache Spark. **Pricing**: **$5 per TB scanned** for SQL queries (minimum 10MB per query); **Spark workloads** billed per DPU-hour . **Free tier**: **$5 per TB scanned** applies, but there is no perpetual free tier for Athena itself; AWS Free Tier includes 1 million Lambda requests/month for federated queries . **Best for**: ad-hoc queries on S3 data without infrastructure management.



- **Starburst Galaxy**

  **Fully managed Trino service** for federated analytics. **Pricing**: **Free tier** includes **3 clusters** with standard execution mode . **Pro at $0.50/credit**; **Enterprise at $0.75/credit**; **Mission-Critical at $1.00/credit** . **Free trial**: **30-day trial** with **$500 in compute credits** and access to Enterprise features . **Best for**: teams wanting managed Trino with a generous free tier.



- **Dremio Cloud**

  **Fully managed SaaS lakehouse on AWS** with consumption-based pricing (DCUs). Features **Autonomous Reflections**, **Elastic Engines that scale to zero**, and a **hosted MCP server**. **Free trial**: **$400 in credits** with all enterprise features included . **Best for**: teams wanting a managed Iceberg-native lakehouse.



- **Snowflake**

  **Cloud data warehouse with consumption-based pricing**. **Pricing**: **Standard at $2.00/credit** (AWS US East), **Enterprise at $3.00/credit**, **Business Critical at $4.00/credit** . **Free tier**: **30-day trial** with **$400 in credits**; no perpetual free tier. **Best for**: enterprises wanting a fully managed warehouse with broad ecosystem support.



- **Google BigQuery**

  **Serverless data warehouse with on-demand and flat-rate pricing**. **Pricing**: **On-demand at $6.25 per TiB scanned** (first 1 TiB/month free); **flat-rate editions** for predictable workloads . **Free tier**: **1 TiB of queries per month** and **10 GB of storage per month** for the lifetime of the project . **Best for**: teams wanting serverless analytics with a meaningful free tier.



- **Amazon Redshift**

  **Cloud data warehouse with provisioned and serverless options**. **Pricing**: **Provisioned starts at $0.543/hour**; **Redshift Serverless starts at $1.50/hour** (billed per second, 60-second minimum) . **Free tier**: **2-month free trial** with **$300 in credits** for provisioned clusters; Serverless has no perpetual free tier . **Best for**: AWS-native teams wanting a mature MPP warehouse.



- **Databricks SQL**

  **Serverless and classic SQL warehouses on the lakehouse**. **Pricing**: **Serverless SQL at $0.70/DBU** (includes cloud instance cost); **Classic SQL at $0.55/DBU**; **SQL Pro at $0.22/DBU** (instance costs billed separately) . **Free tier**: **14-day trial** with limited credits; **Community Edition** is free but limited to non-production use . **Best for**: teams already on Databricks wanting SQL analytics on Delta Lake.



- **Teradata Vantage**

  **Enterprise MPP data warehouse**. **Pricing**: **Quote-only** via Teradata or Azure Marketplace; overage billed at **$0.01/unit** beyond contractual amount . **Free tier**: No free tier; contact sales for evaluation. **Best for**: large enterprises with existing Teradata investments.



## Open-Source GitHub Projects



- **Trino**

  **Distributed SQL query engine for big data** (Apache-2.0) — **the federated query standard** . **13,217 GitHub stars** and actively maintained (last release **484, October 2026**) . **Connects to 40+ data sources** including Hive, Iceberg, Delta Lake, PostgreSQL, MySQL, Kafka, and Elasticsearch—**query data where it lives without moving it** . **Release 484** adds **Parquet selected-positions pushdown** for selective filters, **S3 checksum configuration**, and **DuckDB/Elasticsearch connector improvements** . **The reference implementation for federated SQL**—**choose when you need to query across heterogeneous sources without ETL** .



- **Presto (PrestoDB)**

  **Distributed SQL query engine for big data** (Apache-2.0) — **the original Presto implementation** . **16,700+ GitHub stars** . **Created at Facebook** and now maintained by the Presto Foundation. **The trade-off**: **benchmarks show Velox-accelerated Presto outperforms Trino** on single-node workloads, but **JVM-only stacks (including both Trino and Presto) are an order of magnitude slower than native engines like DuckDB and ClickHouse** for single-node analytics . **Best for**: teams already committed to the Presto ecosystem or needing Facebook-scale heritage.



- **Apache Calcite**

  **Dynamic data management framework** (Apache-2.0) — **the SQL parser and optimizer beneath many engines** . **Provides SQL parsing, validation, and query optimization** for Trino, Dremio, and others. **Best for**: developers building custom query engines.



- **Apache Doris**

  **Real-time analytical database** (Apache-2.0) — **the MySQL-compatible OLAP choice** . **Sub-second queries** on large datasets with lakehouse federation. **Best for**: real-time dashboards and interactive analytics.



- **StarRocks**

  **High-performance OLAP database** (Apache-2.0) — **the lakehouse-native choice** . **Sub-second queries on data lake and warehouse** with materialized views and CBO optimizer. **Best for**: teams wanting fast queries directly on Iceberg/Delta/Hudi.



- **DuckDB**

  **In-process analytical database** (MIT) — **the single-node benchmark leader** . **Benchmarks show native/vectorized engines like DuckDB achieve substantially lower runtimes than JVM-only stacks** on single-node workloads . **Best for**: local analytics and embedded query workloads.



### Additional Strong Open-Source Options



- **Velox** — **C++ vectorized database acceleration library** (Apache-2.0). **The engine behind Velox-accelerated Presto**—delivers order-of-magnitude speedups over JVM stacks .

- **Apache Arrow** — **Columnar in-memory format** (Apache-2.0). **The data exchange standard** beneath DuckDB, Velox, and modern engines.

- **ClickHouse** — **Column-oriented OLAP database** (Apache-2.0). **The fastest single-node analytics engine** in benchmark comparisons .

- Community **n8n** workflows for query result alerting and analytics pipeline automation.



**Frameworks for building custom systems**: Combine **Trino** for federated queries with **DuckDB** for single-node analytics, **Apache Doris** or **StarRocks** for real-time OLAP, and **Apache Calcite** for custom engine development—creating a comprehensive distributed SQL stack.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Distributed SQL query engines handling enterprise data must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls.

- **The "federated vs. warehouse" distinction matters.** **Trino, Presto, and Athena** query data where it lives—no ETL, no data movement . **Snowflake, BigQuery, Redshift, and Databricks SQL** are warehouses—they store and query data together, optimizing for their own storage format . **Choose federated engines when you have data sprawl; choose warehouses when you control the data lifecycle.**

- **The JVM performance gap is real for single-node workloads.** **Benchmarks show native/vectorized engines (DuckDB, ClickHouse, Velox-Presto) deliver up to an order of magnitude lower runtimes than JVM-only stacks (Trino, Spark SQL)** on single-node analytics . **But for distributed, federated queries across petabytes, Trino's breadth of connectors and maturity often outweigh raw speed.**

- **Trino's release cadence is relentless.** **Release 484 arrived in October 2026** with Parquet pushdown and connector improvements . **The trade-off**: you get rapid feature delivery, but **upgrades require attention**—check release notes for breaking changes.

- **Starburst Galaxy's free tier is genuinely usable.** **3 clusters free forever** with standard execution mode . **The 30-day trial with $500 in credits** lets you evaluate Enterprise features without commitment . **Compare against Athena's $5/TB scanned model**—for moderate workloads, Galaxy's credit model may be more predictable.

- Self-hosted open-source solutions require proper cluster management, connector configuration, and ongoing maintenance. **Query engines are infrastructure**—budget for tuning and monitoring regardless of platform choice.



---



**Made for data engineers, analysts, and organizations building transparent distributed SQL solutions.**  

Let's make Distributed SQL Query Engines more open, data-driven, and federated.
