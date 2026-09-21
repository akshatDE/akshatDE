<div align="center">

# Akshat Sharma

### Data Engineer × AI Engineer

Boston, MA

<a href="https://akshat-sharma-portfolio-psi.vercel.app/">
  <img src="https://img.shields.io/badge/Portfolio-Know_More-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio" />
</a>
<a href="https://linkedin.com/in/akshat-sharma-35a514222">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge" alt="LinkedIn" />
</a>
<a href="mailto:sharmaakshat0001@gmail.com">
  <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
</a>

</div>

---

I build data platforms, ETL/ELT pipelines, and AI systems, with an emphasis on reliable architecture and production engineering.

Three years of production data engineering taught me the unglamorous parts — reconciliation, quality gates, failure triage, the schema conversation you have six months before anyone notices you were right. AI is the layer I'm building on top of that: RAG, local LLMs, Text-to-SQL, tool-calling agents.

> ### → [**Know more:** projects, case studies and architecture diagrams](https://akshat-sharma-portfolio-psi.vercel.app/)

---

## Selected Work

### [SoftCart](https://github.com/akshatDE/softcart-ecom-data_platform) · E-commerce Data Platform + Text-to-SQL

![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-4A4A4A?style=flat-square&logo=ollama&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

MySQL and MongoDB through a PostgreSQL staging layer into a DuckDB Kimball star schema — 2 fact tables at order-item grain, 7 conformed dimensions with surrogate keys. Two blocking Airflow quality gates fail the run on violation.

The Text-to-SQL layer's safety is enforced by **code, not by the model**: parsed SELECT-only validation, table allowlist, injected LIMIT, read-only connection, and a pytest suite of injection attempts.

### [YT Trending Pipeline](https://github.com/akshatDE/YT-Trending-Data-Pipeline) · Serverless Medallion on AWS

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

Ingests YouTube Data API v3 trending data across 10 regions into a Bronze–Silver–Gold medallion on Snappy Parquet, provisioned with Boto3. Glue PySpark unifies JSON and CSV schemas; Step Functions orchestrates on a 6-hour EventBridge schedule with exponential-backoff retries.

Quality gates at two boundaries — row-count floors, null thresholds, schema conformance, 48-hour freshness — **halt Gold promotion rather than publishing bad data**. QuickSight reads four Athena SPICE datasets.

### [Agentic AI Learning](https://github.com/akshatDE/AgenticAILearning) · Agent Loop From First Principles

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-4A4A4A?style=flat-square&logo=ollama&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat-square)

A tool-calling agent written without LangChain, LangGraph, CrewAI or AutoGen — the loop written by hand to understand what the frameworks abstract away. JSON tool schemas, a bounded turn budget, and validation errors fed back to the model instead of raised. Runs against local models via Ollama or hosted ones via Groq.

---

## Open Source

[![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)](https://github.com/langchain-ai/langchain)
[![Merged](https://img.shields.io/badge/PR_%2339924-Merged-8957E5?style=flat-square&logo=github&logoColor=white)](https://github.com/langchain-ai/langchain/pull/39924)

Diagnosed a sync/async streaming inconsistency in LangChain's Perplexity integration that corrupted response metadata across streamed chunks. The diagnosis and fix were credited in merged [**PR #39924**](https://github.com/langchain-ai/langchain/pull/39924).

---

## Tech

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**Data Engineering & Orchestration**

![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)

<sub>ETL/ELT · Kimball dimensional modelling · Medallion architecture · Data quality gates · Data governance</sub>

**Warehouses & Databases**

![BigQuery](https://img.shields.io/badge/BigQuery-669DF6?style=flat-square&logo=googlebigquery&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)

**Cloud**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white)

<sub>S3 · Glue · Lambda · Athena · Step Functions · EventBridge · SNS · CloudWatch</sub>

**AI / LLM Engineering**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langgraph&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-4A4A4A?style=flat-square&logo=ollama&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square)

<sub>RAG · Text-to-SQL · Tool-calling agents · MCP · Local inference · Prompt & context engineering</sub>

**Backend & DevOps**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

---

<div align="center">

**Open to Data Engineering and AI-integrated data roles.**

<a href="https://akshat-sharma-portfolio-psi.vercel.app/">
  <img src="https://img.shields.io/badge/See_the_full_portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio" />
</a>

</div>
