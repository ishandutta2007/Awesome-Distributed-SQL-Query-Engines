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

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)

- [SaaS/Hosted Platforms](#saashosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## Sector Overview & Market Dynamics

The global **data lake query engine market** is valued at approximately **$8.7 billion** and is projected to reach **$38.4 billion by 2034** at a CAGR of ~17.9%. The sector is **moderately concentrated** at the top — hyperscalers (Google BigQuery, AWS Athena/Redshift) and scaled pure-plays (Snowflake, Databricks) command the lion's share of revenue, but a healthy long tail of open-source engines (Trino, Presto, DuckDB) and specialized vendors (Starburst, Dremio, StarRocks) keeps competition vigorous and prevents a true winner-take-all dynamic.



## SaaS/Hosted Platforms

> Sorted by company scale (descending). Pricing reflects publicly listed starting-tier rates as of October 2026.

| Platform | Description | Pricing (Starting Tier) | Free Tier / Free Trial Limits | Company Scale | Best For |
|---|---|---|---|---|---|
| **Google BigQuery** | Serverless data warehouse with on-demand and flat-rate pricing | On-demand: **$6.25 per TiB** scanned; flat-rate editions available for predictable workloads | **Forever free**: 1 TiB queries/month + 10 GB storage/month per project (lifetime, no credit card) | Alphabet — **~$4.1 T market cap**; Google Cloud **$24.8 B quarterly rev** (Q2 2026) | Serverless analytics with a meaningful free tier |
| **AWS Athena** | Serverless interactive analytics for querying S3 data using SQL or Apache Spark | **$5.00 per TB** scanned (10 MB minimum per query); Spark billed per DPU-hour | **No perpetual free tier**; DDL statements & failed queries free; new AWS accounts can apply general sign-up credits | Amazon — **~$2.8 T market cap**; AWS **$42.2 B quarterly rev** (Q2 2026) | Ad-hoc queries on S3 without infrastructure mgmt |
| **Amazon Redshift** | Cloud data warehouse with provisioned and serverless options | Provisioned from **$0.543/hr**; Serverless from **$1.50/hr** (per-second billing, 60 s min) | **Trial only**: 2-month free trial with **$300 in credits** for provisioned clusters; no perpetual free tier | Amazon — **~$2.8 T market cap**; AWS **$42.2 B quarterly rev** (Q2 2026) | AWS-native teams wanting a mature MPP warehouse |
| **Databricks SQL** | Serverless and classic SQL warehouses on the lakehouse | SQL Pro: **$0.22/DBU** (+ instance costs); Classic: **$0.55/DBU**; Serverless: **$0.70/DBU** (instance incl.) | **Trial only**: 14-day trial with limited credits; **Community Edition** free forever but single-node, non-production only | Databricks — **$190 B valuation** (Aug 2026); **$7 B+ revenue run-rate** | Teams on Databricks wanting SQL analytics on Delta Lake |
| **Snowflake** | Cloud data warehouse with consumption-based pricing | Standard: **$2.00/credit**; Enterprise: **$3.00/credit**; Business Critical: **$4.00/credit** (AWS US East) | **Trial only**: 30-day trial with **$400 in credits** + Enterprise features; no perpetual free tier | Snowflake — **~$105—118 B market cap**; **$5.4 B TTM revenue** | Fully managed warehouse with broad ecosystem support |
| **Starburst Galaxy** | Fully managed Trino service for federated analytics | Pro: **$0.50/credit**; Enterprise: **$0.75/credit**; Mission-Critical: **$1.00/credit** | **Forever free**: 3 clusters with standard execution mode; **30-day trial** with **$500 in credits** for Enterprise | Starburst Data — **$3.35 B valuation** (Series D); **$100 M+ ARR** | Managed Trino with a generous free tier |
| **Teradata Vantage** | Enterprise MPP data warehouse | VantageCloud Lake Standard from **$4.80/hr** (~$1.50/TU); Lake+ from **$7.20/hr**; storage ~$23/TB/mo | **Trial only**: ClearScape Analytics Experience — free sandbox with 250+ guided demos, no credit card req'd; no production free tier | Teradata — **~$2.8 B market cap**; **$1.69 B TTM revenue** | Large enterprises with existing Teradata investments |
| **Dremio Cloud** | Fully managed SaaS lakehouse on AWS with Autonomous Reflections & Elastic Engines | **$0.20/DCU** pay-as-you-go; XS engine ~$6.40/hr, S ~$12.80/hr, M ~$25.60/hr | **Forever free**: Standard tier — ≤10 users, ≤200 tables, ≤1,000 views, engine capped at Small; **Enterprise trial**: $400 credits / 30 days | Dremio — acquired by **SAP** (May 2026); last private valuation **$2 B** | Managed Iceberg-native lakehouse |


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
