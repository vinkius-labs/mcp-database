# Matillion (Cloud Data Integration & ELT) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/matillion-cloud-data-integration-elt)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/matillion-cloud-data-integration-elt-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/matillion-cloud-data-integration-elt-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Manage data pipelines via Matillion — audit ETL workflows, track execution statuses, and monitor cloud environments.

## Description
Connect your **Matillion Data Productivity Cloud** account to any AI agent and take full control of your enterprise ELT orchestration and data integration lifecycle through natural conversation.

### What you can do

- **Pipeline Orchestration** — List all managed ETL pipelines and retrieve detailed structural components of your data transformation logic directly from your agent
- **Execution Audit** — Monitor recent pipeline executions to track failed or successful deployment statuses and identify operational bottlenecks in real-time
- **Infrastructure Visibility** — Enumerate active Matillion runtime agents and Hybrid SaaS components physically resolving operations across your local network
- **Environment Audit** — List configured destination environments attached to cloud data warehouses like Snowflake, Redshift, or BigQuery to ensure data mapping accuracy
- **Project Management** — Extract and navigate broad project containers that bind your pipelines and environments together within the Matillion Hub
- **Metadata Inspection** — Deep-dive into specific pipeline IDs to retrieve the underlying orchestration definitions and schema mappings securely

### How it works

1. Subscribe to this server
2. Enter your Matillion API URL, Client ID, and Client Secret
3. Start managing your data productivity cloud from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — verify pipeline designs and audit execution logs through natural conversation without manual hub navigation
- **Analytics Leads** — monitor project health and data warehouse environment statuses directly from your workspace terminal
- **BI Operations Teams** — track active runtime agents and ensure high availability of critical ELT processes efficiently


## Available Tools
- **list_pipelines**: List all Matillion ETL pipelines
- **get_pipeline**: Get specific pipeline details
- **list_executions**: List recent pipeline executions
- **list_environments**: List all environment configurations
- **list_agents**: List all Matillion runtime agents
- **list_projects**: List all projects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Matillion (Cloud Data Integration & ELT)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Matillion ETL pipelines in my account"

**🤖 AI Agent:**
> I've retrieved your ETL pipelines from the Data Productivity Cloud. Highlights include 'Sales-Data-Sync' (ID: pipe-123), 'Customer-360-View' (ID: pipe-456), and 'Finance-Consolidation' (ID: pipe-789). Would you like to see the structural components for the sales sync?

---

**👤 You:**
> "Show me the last 5 pipeline executions and their status"

**🤖 AI Agent:**
> Retrieving recent executions… I've identified the 5 latest runs: 3 succeeded (including 'Inventory-Load'), 1 is currently 'Running' ('Marketing-Attribution'), and 1 'Failed' ('Web-Log-Ingestion'). Would you like me to investigate the error for the failed run?

---

**👤 You:**
> "What cloud environments are configured in my Matillion instance?"

**🤖 AI Agent:**
> I've identified 3 destination environments: 'Snowflake-Prod' (Targeting: SF_WH_01), 'Redshift-Staging' (Targeting: AWS_NODE_ALPHA), and 'BigQuery-Analytics' (Targeting: GCP_DATASET_V1). I can provide the project mappings for these environments if you'd like.


## Installation & Usage

To install and use the **Matillion (Cloud Data Integration & ELT)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/matillion-cloud-data-integration-elt](https://vinkius.com/mcp/matillion-cloud-data-integration-elt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
