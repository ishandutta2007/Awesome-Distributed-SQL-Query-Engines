<p align="center">
  <img src="assets/banner.svg" alt="Awesome Distributed SQL Query Engines Banner" width="100%" />
</p>

# ⚡ Awesome-Distributed-SQL-Query-Engines

<p align="center">
  <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a>
  <a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Disoord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Distributed-SQL-Query-Engines/stargazers"><img src="https://img.shields.io/github/stars/ishandutta2007/Awesome-Distributed-SQL-Query-Engines?style=social" alt="GitHub_Stars" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Distributed-SQL-Query-Engines/network/members"><img src="https://img.shields.io/github/forks/ishandutta2007/Awesome-Distributed-SQL-Query-Engines?style=social" alt="GitHub forks" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Distributed-SQL-Query-Engines/blob/main/LICENSE"><img src="https://img.shields.io/github/license/ishandutta2007/Awesome-Distributed-SQL-Query-Engines" alt="License" /></a>
  <a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>
</p>

## 🚀 Top Distributed SQL Query Engines Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects** 🌐  
*Focused on Federated Queries, Lakehouse Analytics & Massive Parallel Processing (MPP)* 🔍  

**Last updated: October 2026** 📅

This repository tracks notable **SaaS platforms** and **open-source projects** for **Distributed SQL Query Engines**. These tools enable organizations to query massive datasets across data lakes, warehouses, and databases—from federated engines that read data where it lives to MPP warehouses that optimize storage and compute together. 📊

**Examples** include Trino, Presto, ClickHouse, DuckDB, Apache Spark, TiDB, CockroachDB, AWS Athena, Starburst Galaxy, Dremio Cloud, Snowflake, Google BigQuery, Amazon Redshift, Databricks SQL, and Teradata Vantage. 💡

**Open-source emphasis** 🛠️: This section is heavily expanded with major active projects for self-hosting, federated querying, and open lakehouse infrastructure—ideal for data engineers, analysts, and organizations seeking transparent, vendor-independent SQL analytics.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites. ✨

---

## 📑 Table of Contents

- [📈 Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [☁️ SaaS/Hosted Platforms](#️-saashosted-platforms)
- [🔓 Open-Source GitHub Projects](#-open-source-github-projects)
- [🤝 How to Contribute](#-how-to-contribute)
- [💖 Support](#-support)
- [📊 Star History](#-star-history)
- [⚠️ Disclaimer](#️-disclaimer)

---

## 📈 Sector Overview & Market Dynamics

The global **data lake query engine market** is valued at approximately **$8.7 billion** and is projected to reach **$38.4 billion by 2034** at a CAGR of ~17.9%. The sector is **moderately concentrated** at the top — hyperscalers (Google BigQuery, AWS Athena/Redshift) and scaled pure-plays (Snowflake, Databricks) command the lion's share of revenue, but a healthy long tail of open-source engines (Trino, Presto, DuckDB, ClickHouse) and specialized vendors (Starburst, Dremio, StarRocks) keeps competition vigorous and prevents a true winner-take-all dynamic. 🌐

---

## ☁️ SaaS/Hosted Platforms

> 📌 *Sorted by company scale (descending). Pricing reflects publicly listed starting-tier rates as of October 2026.*

| Platform | Description | Pricing (Starting Tier) | Free Tier / Free Trial Limits | Company Scale | Best For |
|---|---|---|---|---|---|
| **Google BigQuery** | Serverless data warehouse with on-demand and flat-rate pricing | On-demand: **$6.25 per TiB** scanned; flat-rate editions available for predictable workloads | **Forever free**: 1 TiB queries/month + 10 GB storage/month per project (lifetime, no credit card) | Alphabet — **~$4.1 T market cap**; Google Cloud **$24.8 B quarterly rev** (Q2 2026) | Serverless analytics with a meaningful free tier |
| **AWS Athena** | Serverless interactive analytics for querying S3 data using SQL or Apache Spark | **$5.00 per TB** scanned (10 MB minimum per query); Spark billed per DPU-hour | **No perpetual free tier**; DDL statements & failed queries free; new AWS accounts can apply general sign-up credits | Amazon — **~$2.8 T market cap**; AWS **$42.2 B quarterly rev** (Q2 2026) | Ad-hoc queries on S3 without infrastructure mgmt |
| **Amazon Redshift** | Cloud data warehouse with provisioned and serverless options | Provisioned from **$0.543/hr**; Serverless from **$1.50/hr** (per-second billing, 60 s min) | **Trial only**: 2-month free trial with **$300 in credits** for provisioned clusters; no perpetual free tier | Amazon — **~$2.8 T market cap**; AWS **$42.2 B quarterly rev** (Q2 2026) | AWS-native teams wanting a mature MPP warehouse |
| **Databricks SQL** | Serverless and classic SQL warehouses on the lakehouse | SQL Pro: **$0.22/DBU** (+ instance costs); Classic: **$0.55/DBU**; Serverless: **$0.70/DBU** (instance incl.) | **Trial only**: 14-day trial with limited credits; **Community Edition** free forever but single-node, non-production only | Databricks — **$190 B valuation** (Aug 2026); **$7 B+ revenue run-rate** | Teams on Databricks wanting SQL analytics on Delta Lake |
| **Snowflake** | Cloud data warehouse with consumption-based pricing | Standard: **$2.00/credit**; Enterprise: **$3.00/credit**; Business Critical: **$4.00/credit** (AWS US East) | **Trial only**: 30-day trial with **$400 in credits** + Enterprise features; no perpetual free tier | Snowflake — **~$105–118 B market cap**; **$5.4 B TTM revenue** | Fully managed warehouse with broad ecosystem support |
| **Starburst Galaxy** | Fully managed Trino service for federated analytics | Pro: **$0.50/credit**; Enterprise: **$0.75/credit**; Mission-Critical: **$1.00/credit** | **Forever free**: 3 clusters with standard execution mode; **30-day trial** with **$500 in credits** for Enterprise | Starburst Data — **$3.35 B valuation** (Series D); **$100 M+ ARR** | Managed Trino with a generous free tier |
| **Teradata Vantage** | Enterprise MPP data warehouse | VantageCloud Lake Standard from **$4.80/hr** (~$1.50/TU); Lake+ from **$7.20/hr**; storage ~$23/TB/mo | **Trial only**: ClearScape Analytics Experience — free sandbox with 250+ guided demos, no credit card req'd; no production free tier | Teradata — **~$2.8 B market cap**; **$1.69 B TTM revenue** | Large enterprises with existing Teradata investments |
| **Dremio Cloud** | Fully managed SaaS lakehouse on AWS with Autonomous Reflections & Elastic Engines | **$0.20/DCU** pay-as-you-go; XS engine ~$6.40/hr, S ~$12.80/hr, M ~$25.60/hr | **Forever free**: Standard tier — ≤10 users, ≤200 tables, ≤1,000 views, engine capped at Small; **Enterprise trial**: $400 credits / 30 days | Dremio — acquired by **SAP** (May 2026); last private valuation **$2 B** | Managed Iceberg-native lakehouse |

---

## 🔓 Open-Source GitHub Projects

> 📌 *Sorted by GitHub_Stars_Count (descending). Each badge links directly to that repository's stargazers page.*

- **ClickHouse** [![Stars](https://img.shields.io/github/stars/ClickHouse/ClickHouse?style=social&color=white)](https://github.com/ClickHouse/ClickHouse/stargazers) ⚡  
  **Column-oriented DBMS for real-time analytical reporting** (Apache-2.0). The fastest open-source single-node and distributed analytics engine in benchmark comparisons, delivering sub-second query performance over billions of rows. **Best for**: real-time analytics, telemetry, event logs, and high-concurrency dashboards.

- **Apache Spark** [![Stars](https://img.shields.io/github/stars/apache/spark?style=social&color=white)](https://github.com/apache/spark/stargazers) 🔥  
  **Unified analytics engine for large-scale data processing** (Apache-2.0). Provides distributed SQL via Spark SQL, DataFrame APIs, and structured streaming across clusters with extensive catalyst optimizer pushdown. **Best for**: massive-scale batch transformations, complex distributed data pipelines, and machine learning at petabyte scale.

- **DuckDB** [![Stars](https://img.shields.io/github/stars/duckdb/duckdb?style=social&color=white)](https://github.com/duckdb/duckdb/stargazers) 🦆  
  **In-process SQL OLAP database management system** (MIT). Benchmarks show native vectorized execution delivers blazing fast runtimes on columnar formats like Parquet and Iceberg without requiring external cluster coordination. **Best for**: local analytics, embedded analytical engines, fast Python/R data pipelines, and serverless compute nodes.

- **TiDB** [![Stars](https://img.shields.io/github/stars/pingcap/tidb?style=social&color=white)](https://github.com/pingcap/tidb/stargazers) 🗄️  
  **Open-source distributed Hybrid Transactional and Analytical Processing (HTAP) database** (Apache-2.0). MySQL compatible, horizontal elasticity, strong consistency with Raft consensus, and real-time analytical queries using TiFlash columnar store. **Best for**: modern HTAP workloads needing zero-ETL transaction processing combined with distributed SQL analytics.

- **CockroachDB** [![Stars](https://img.shields.io/github/stars/cockroachdb/cockroach?style=social&color=white)](https://github.com/cockroachdb/cockroach/stargazers) 🪳  
  **Distributed SQL database built on transactional and strongly consistent key-value store** (BSL/Open Source core). Provides standard PostgreSQL dialect, multi-region horizontal scaling, and surviving host failures transparently. **Best for**: globally distributed operational applications demanding strong consistency and distributed SQL.

- **Apache Arrow** [![Stars](https://img.shields.io/github/stars/apache/arrow?style=social&color=white)](https://github.com/apache/arrow/stargazers) 🏹  
  **Multi-language development platform for in-memory columnar data** (Apache-2.0). The global data exchange and in-memory execution standard underlying modern query execution engines including DuckDB, Velox, and DataFusion. **Best for**: zero-copy data exchange and high-performance columnar compute.

- **Presto (PrestoDB)** [![Stars](https://img.shields.io/github/stars/prestodb/presto?style=social&color=white)](https://github.com/prestodb/presto/stargazers) 🦅  
  **Distributed SQL query engine for big data** (Apache-2.0) — **the original Presto implementation** developed at Facebook and maintained by the Presto Foundation. Modern deployments leverage Velox for C++ vectorized native acceleration. **Best for**: large-scale interactive SQL analytics on open data lakes.

- **Apache Doris** [![Stars](https://img.shields.io/github/stars/apache/doris?style=social&color=white)](https://github.com/apache/doris/stargazers) 🐬  
  **Real-time analytical database** (Apache-2.0) — **the MySQL-compatible OLAP engine**. Provides sub-second queries on large datasets with lakehouse federation, inverted indexes, and real-time streaming ingestion. **Best for**: real-time user-facing dashboards, ad-hoc OLAP analysis, and reporting.

- **Trino** [![Stars](https://img.shields.io/github/stars/trinodb/trino?style=social&color=white)](https://github.com/trinodb/trino/stargazers) 🗡️  
  **Distributed SQL query engine for big data** (Apache-2.0) — **the federated query standard**. Connects to 40+ heterogeneous data sources (Hive, Iceberg, Delta Lake, PostgreSQL, MySQL, Kafka, Elasticsearch) without data movement. **Best for**: querying heterogeneous data sources without ETL and federated analytics across multi-cloud lakes.

- **StarRocks** [![Stars](https://img.shields.io/github/stars/StarRocks/starrocks?style=social&color=white)](https://github.com/StarRocks/starrocks/stargazers) 🌟  
  **Next-generation high-performance sub-second OLAP database** (Apache-2.0). Designed for full lakehouse analytics with vectorized C++ execution, cost-based optimizer (CBO), and intelligent materialized views directly on Iceberg/Delta/Hudi formats. **Best for**: low-latency lakehouse queries, real-time analytics, and high-concurrency BI.

- **Apache DataFusion** [![Stars](https://img.shields.io/github/stars/apache/datafusion?style=social&color=white)](https://github.com/apache/datafusion/stargazers) 🦀  
  **Extensible query execution engine written in Rust** (Apache-2.0). Features an Apache Arrow-native in-memory format, vectorized query execution, SQL parser, and modular planner/optimizer. **Best for**: building custom high-performance distributed query engines, in-process analytical tools, and lakehouse query engines.

- **Apache Iceberg** [![Stars](https://img.shields.io/github/stars/apache/iceberg?style=social&color=white)](https://github.com/apache/iceberg/stargazers) 🧊  
  **Open table format for huge analytic datasets** (Apache-2.0). Enables multiple distributed SQL engines (Trino, Presto, Spark, ClickHouse, StarRocks, Dremio) to safely query and write to the same tables concurrently with ACID guarantees, schema evolution, and hidden partitioning. **Best for**: standardized lakehouse table representation across diverse SQL query engines.

- **Apache Calcite** [![Stars](https://img.shields.io/github/stars/apache/calcite?style=social&color=white)](https://github.com/apache/calcite/stargazers) 📐  
  **Dynamic data management framework** (Apache-2.0) — **the SQL parser, validator, and relational algebra cost optimizer**. Used beneath dozens of distributed query engines including Trino, Drill, Dremio, and Apache Hive. **Best for**: engineers and developers building custom distributed query execution engines.

- **Velox** [![Stars](https://img.shields.io/github/stars/facebookincubator/velox?style=social&color=white)](https://github.com/facebookincubator/velox/stargazers) 🏎️  
  **C++ vectorized database acceleration library** (Apache-2.0). Originated at Meta, Velox acts as a modular execution engine backend accelerating Presto, Spark (via Gluten), and custom distributed computing engines with substantial speedups over pure JVM runtimes. **Best for**: engine builders accelerating distributed execution layers.

- **Apache Ballista** [![Stars](https://img.shields.io/github/stars/apache/datafusion-ballista?style=social&color=white)](https://github.com/apache/datafusion-ballista/stargazers) 🏹  
  **Distributed compute platform powered by Apache Arrow and DataFusion** (Apache-2.0). Written in Rust, it provides a lightweight, highly efficient distributed query execution engine that scales horizontally across clusters. **Best for**: cloud-native, memory-efficient distributed SQL execution without JVM overhead.

- **Dremio OSS** [![Stars](https://img.shields.io/github/stars/dremio/dremio-oss?style=social&color=white)](https://github.com/dremio/dremio-oss/stargazers) 🌊  
  **Open-source data lakehouse platform and SQL engine** (Apache-2.0). Built on Apache Arrow, providing semantic layering, federated queries, data reflections acceleration, and direct query execution over data lakes. **Best for**: self-hosted open data lakehouse architectures and semantic layer management.

---

## 🤝 How to Contribute

1. 🍴 Fork the repository.
2. ✍️ Add or edit entries in `README.md` following the existing format.
3. 📝 Include: name, links, badges, factual description, and category (SaaS or Open-Source).
4. 🚀 Submit a Pull Request with a clear explanation of changes.

⭐ Star the repo if you find it helpful!

---

## 💖 Support

Thank you for exploring and using **Awesome-Distributed-SQL-Query-Engines**! 🙌

If this repository has saved you time or aided your data infrastructure decisions, please consider supporting the project:

- ⭐ **Star** this repository on GitHub to help others discover it!
- 🍴 **Fork** and share it with your fellow data engineers and architects!
- 📣 **Spread the word** across your networks and communities!
- ☕ **Buy me a coffee**: Support ongoing maintenance and curated updates directly via the [GitHub Sponsors Dashboard](https://github.com/sponsors/ishandutta2007).

Your encouragement and support keep this project accurate, fresh, and continuously updated! 🚀

---

## 📊 Star History

[![Star History Chart](https://star-history.dera.page/svg?repos=ishandutta2007/Awesome-Distributed-SQL-Query-Engines&type=date&legend=top-left)](https://star-history.dera.page/#ishandutta2007/Awesome-Distributed-SQL-Query-Engines&type=date&legend=top-left)

---

## ⚠️ Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement. 📋
- Distributed SQL query engines handling enterprise data must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls. 🔒
- **The "federated vs. warehouse" distinction matters**: **Trino, Presto, and Athena** query data where it lives without ETL data movement. **Snowflake, BigQuery, Redshift, and Databricks SQL** store and query data together, optimizing for their own internal columnar formats. Choose federated engines when dealing with heterogeneous data sprawl; choose warehouses when you manage the end-to-end data lifecycle. ⚖️
- **The native/vectorized performance advantage**: Benchmarks demonstrate native/vectorized engines (ClickHouse, DuckDB, Velox-Presto, DataFusion) achieve up to an order of magnitude lower runtimes than JVM-only engines for compute-bound queries. However, for massive-scale petabyte queries across disparate enterprise connectors, mature federated distributed engines like Trino remain industry benchmarks. ⚙️
- Self-hosted open-source query engines require dedicated cluster sizing, memory configuration, and operational monitoring. Budget for proper tuning regardless of engine selection. 💡

---

**Made with ❤️ for data engineers, analysts, and organizations building high-performance distributed SQL query solutions.**  
*Let's make Distributed SQL Query Engines more open, performant, and federated!* 🌐
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



- **[AWS Athena](https://aws.amazon.com/athena/)**

  **Serverless interactive analytics service** for querying data in S3 using SQL or Apache Spark. **Pricing**: **$5 per TB scanned** for SQL queries (minimum 10MB per query) . **Free tier**: No perpetual free tier—$5/TB applies from the first byte; AWS Free Tier does not cover Athena query costs. **Best for**: ad-hoc queries on S3 data without infrastructure management.



- **[Starburst Galaxy](https://www.starburst.io/)**

  **Fully managed Trino service** for federated analytics. **Pricing**: **Pro at $0.50/credit**; **Enterprise at $0.75/credit**; **Mission-Critical at $1.00/credit** . **Free tier**: **Free forever with 3 clusters** and standard execution mode for ad-hoc queries . **Free trial**: **30-day trial** with **$500 in compute credits** and Enterprise-tier features . **Best for**: teams wanting managed Trino with a genuinely usable free tier.



- **[Dremio Cloud](https://www.dremio.com/)**

  **Fully managed SaaS lakehouse on AWS** with consumption-based pricing (DCUs). Features **Autonomous Reflections**, **Elastic Engines that scale to zero**, and a **hosted MCP server**. **Free trial**: **$400 in credits** with all enterprise features included, no credit card required, account preserved 30 days after trial . **Best for**: teams wanting a managed Iceberg-native lakehouse.



- **[Snowflake](https://www.snowflake.com/)**

  **Cloud data warehouse with consumption-based pricing**. **Pricing**: **Standard at $2.00/credit** (AWS US East), **Enterprise at $3.00/credit**, **Business Critical at $4.00/credit** . **Free tier**: **30-day trial** with **$400 in credits**; no perpetual free tier. **Best for**: enterprises wanting a fully managed warehouse with broad ecosystem support.



- **[Google BigQuery](https://cloud.google.com/bigquery)**

  **Serverless data warehouse with on-demand and flat-rate pricing**. **Pricing**: **On-demand at $6.25 per TiB scanned**; **flat-rate editions** for predictable workloads. **Free tier**: **1 TiB of queries per month** and **10 GB of storage per month** for the lifetime of the project . **Best for**: teams wanting serverless analytics with a meaningful perpetual free tier.



- **[Amazon Redshift](https://aws.amazon.com/redshift/)**

  **Cloud data warehouse with provisioned and serverless options**. **Pricing**: **Provisioned starts at $0.543/hour**; **Redshift Serverless starts at $0.375 per RPU-hour** (60-second minimum), roughly **$1.50/hour at the 4-RPU base** . **Free tier**: **2-month free trial** with **$300 in credits** for provisioned clusters; Serverless has no perpetual free tier. **Best for**: AWS-native teams wanting a mature MPP warehouse.



- **[Databricks SQL](https://www.databricks.com/)**

  **Serverless and classic SQL warehouses on the lakehouse**. **Pricing**: **Serverless SQL at $0.70/DBU** (includes cloud instance cost) ; **Classic SQL** and **SQL Pro** tiers available at lower DBU rates with separate instance billing. **Free tier**: **14-day trial** with limited credits; **Community Edition** is free but limited to non-production use. **Best for**: teams already on Databricks wanting SQL analytics on Delta Lake.



- **[Teradata Vantage](https://www.teradata.com/)**

  **Enterprise MPP data warehouse**. **Pricing**: **Quote-only** via Teradata or Azure Marketplace; overage billed at **$0.01/unit** beyond contractual amount. **Free tier**: **Teradata Vantage Express** is a free, fully functional VM image for local testing and development ; **ClearScape Analytics Experience** provides a free hosted instance for testing . **Best for**: large enterprises with existing Teradata investments.



## Open-Source GitHub Projects



- **[Trino](https://github.com/trinodb/trino)**

  **Distributed SQL query engine for big data** (Apache-2.0) — **the federated query standard**. **13,217 GitHub stars** . **Connects to 40+ data sources** including Hive, Iceberg, Delta Lake, PostgreSQL, MySQL, Kafka, and Elasticsearch—**query data where it lives without moving it**. **Release 484** (October 2026) adds **Parquet selected-positions pushdown** for selective filters, **S3 checksum configuration**, and **DuckDB/Elasticsearch connector improvements**. **The reference implementation for federated SQL**—**choose when you need to query across heterogeneous sources without ETL**.



- **[Presto (PrestoDB)](https://github.com/prestodb/presto)**

  **Distributed SQL query engine for big data** (Apache-2.0) — **the original Presto implementation**. **16,700+ GitHub stars** . **Created at Facebook** and now maintained by the Presto Foundation. **The trade-off**: **JVM-only stacks (including both Trino and Presto) are an order of magnitude slower than native engines like DuckDB and ClickHouse** for single-node analytics. **Best for**: teams already committed to the Presto ecosystem or needing Facebook-scale heritage.



- **[Apache Calcite](https://github.com/apache/calcite)**

  **Dynamic data management framework** (Apache-2.0) — **the SQL parser and optimizer beneath many engines**. Provides **SQL parsing, validation, and query optimization** for Trino, Dremio, and others. **Best for**: developers building custom query engines.



- **[Apache Doris](https://github.com/apache/doris)**

  **Real-time analytical database** (Apache-2.0) — **the MySQL-compatible OLAP choice**. **15,046 GitHub stars** . **Sub-second queries** on large datasets with lakehouse federation. **Best for**: real-time dashboards and interactive analytics.



- **[DuckDB](https://github.com/duckdb/duckdb)**

  **In-process analytical database** (MIT) — **the single-node benchmark leader**. **36,510 GitHub stars** . **Benchmarks show native/vectorized engines like DuckDB achieve substantially lower runtimes than JVM-only stacks** on single-node workloads. **Best for**: local analytics and embedded query workloads.



- **[Velox](https://github.com/facebookincubator/velox)**

  **C++ vectorized database acceleration library** (Apache-2.0) — **the engine behind Velox-accelerated Presto**. **4,200 GitHub stars** . Delivers order-of-magnitude speedups over JVM stacks. **Best for**: teams building or accelerating query engines.



### Additional Strong Open-Source Options



- **[StarRocks](https://github.com/StarRocks/starrocks)** — **High-performance OLAP database** (Apache-2.0). **Sub-second queries on data lake and warehouse** with materialized views and CBO optimizer. **Best for**: teams wanting fast queries directly on Iceberg/Delta/Hudi.

- **[Apache Arrow](https://github.com/apache/arrow)** — **Columnar in-memory format** (Apache-2.0). **The data exchange standard** beneath DuckDB, Velox, and modern engines.

- **[ClickHouse](https://github.com/ClickHouse/ClickHouse)** — **Column-oriented OLAP database** (Apache-2.0). **The fastest single-node analytics engine** in benchmark comparisons.

- Community **n8n** workflows for query result alerting and analytics pipeline automation.



**Frameworks for building custom systems**: Combine **Trino** for federated queries with **DuckDB** for single-node analytics, **Apache Doris** for real-time OLAP, and **Apache Calcite** for custom engine development—creating a comprehensive distributed SQL stack.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Distributed SQL query engines handling enterprise data must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls.

- **The "federated vs. warehouse" distinction matters.** **Trino, Presto, and Athena** query data where it lives—no ETL, no data movement. **Snowflake, BigQuery, Redshift, and Databricks SQL** are warehouses—they store and query data together, optimizing for their own storage format. **Choose federated engines when you have data sprawl; choose warehouses when you control the data lifecycle.**

- **The JVM performance gap is real for single-node workloads.** **Benchmarks show native/vectorized engines (DuckDB, ClickHouse, Velox-Presto) deliver up to an order of magnitude lower runtimes than JVM-only stacks (Trino, Spark SQL)** on single-node analytics. **But for distributed, federated queries across petabytes, Trino's breadth of connectors and maturity often outweigh raw speed.**

- **Starburst Galaxy's free tier is genuinely usable.** **3 clusters free forever** with standard execution mode . **The 30-day trial with $500 in credits** lets you evaluate Enterprise features without commitment. **Compare against Athena's $5/TB scanned model**—for moderate workloads, Galaxy's credit model may be more predictable.

- **BigQuery's perpetual free tier is the most generous among warehouses.** **1 TiB of queries and 10 GB storage per month, forever** . **Redshift's 2-month trial with $300 credits** is time-bound. **Snowflake and Databricks offer trials only**—no perpetual free tier.

- Self-hosted open-source solutions require proper cluster management, connector configuration, and ongoing maintenance. **Query engines are infrastructure**—budget for tuning and monitoring regardless of platform choice.



---



**Made for data engineers, analysts, and organizations building transparent distributed SQL solutions.**  

Let's make Distributed SQL Query Engines more open, data-driven, and federated.
