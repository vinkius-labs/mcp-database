# Databricks MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/databricks)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/databricks-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/databricks-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage lakehouse via Databricks — monitor compute clusters, track job executions, audit SQL warehouses, and explore Unity Catalog directly from any AI agent.

## Description
Connect your **Databricks** workspace to any AI agent and take full control of your data intelligence platform and lakehouse orchestration through natural conversation.

### What you can do

- **Cluster Monitoring** — List all compute nodes and retrieve detailed information for specific clusters to audit health and capacity limits
- **Job Orchestration** — List all configured workflows and jobs, and monitor recent executions to verify data pipeline statuses
- **SQL Warehouse Management** — Enumerate explicitly configured SQL Serverless warehouses and track their active operational boundaries
- **Unity Catalog Exploration** — List root catalogs and detailed schemas/databases to identify exactly where your structured data resides
- **Identity Oversight** — Fetch profile information for the authenticated user or service principal to verify active workspace permissions
- **Run Auditing** — Retrieve chronological logs of job runs to identify precise points of failure in your complex data workflows

### How it works

1. Subscribe to this server
2. Enter your Databricks Host URL and Personal Access Token (PAT)
3. Start managing your lakehouse from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — monitor job runs and cluster health without leaving the development environment
- **Analytics Engineers** — explore Unity Catalog schemas and verify SQL warehouse availability in real-time
- **Data Platform Teams** — audit workspace resources and monitor active service principal identities
- **MLOps Engineers** — track model training jobs and verify compute cluster configurations through natural language


## Available Tools
- **list_clusters**: List all clusters from Databricks
- **get_cluster**: Get cluster details from Databricks
- **list_jobs**: List all jobs from Databricks
- **list_job_runs**: List job runs from Databricks
- **list_warehouses**: List SQL warehouses from Databricks
- **list_catalogs**: List Unity Catalog catalogs from Databricks
- **list_schemas**: List schemas in catalog from Databricks
- **get_me**: Get current user from Databricks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Databricks** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all compute clusters in my workspace"

**🤖 AI Agent:**
> I found 3 clusters: 'Standard-ETL-Cluster' (Running), 'ML-Training-Node' (Terminated), and 'Shared-Dev-Pool' (Running). Would you like to see the detailed specs for any of these?

---

**👤 You:**
> "Show me the last 5 runs for job 'Daily-Sales-ETL'"

**🤖 AI Agent:**
> Retrieving runs for 'Daily-Sales-ETL'... The most recent (ID: 987) finished successfully at 6:00 AM. Run 985 failed due to a cluster timeout. I can pull the detailed error logs if you'd like.

---

**👤 You:**
> "List all catalogs in Unity Catalog"

**🤖 AI Agent:**
> I found 4 root catalogs: 'main', 'development', 'samples', and 'system'. Which one would you like to explore for databases and schemas?


## Installation & Usage

To install and use the **Databricks** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/databricks](https://vinkius.com/mcp/databricks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
