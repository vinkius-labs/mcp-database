# Azure Synapse Analytics MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/azure-synapse-analytics)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/azure-synapse-analytics-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/azure-synapse-analytics-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Azure Synapse data pipelines seamlessly — audit Spark pools, SQL pools, datasets, and integration pipelines via your AI agent.

## Description
Connect your **Azure Synapse** workspace to any AI agent and take full control of your enterprise analytics workflows and data integration limits through natural conversation.

### What you can do

- **Compute Pools** — Monitor currently provisioned infrastructure, ranging from Serverless/Dedicated SQL Pools to your active Apache Spark analytic clusters
- **Integration Pipelines** — Dissect data movement workflows (ETL/ELT), viewing precise activity target parameters and logical steps for a single tracked job
- **Notebooks** — Explore global Apache Spark analytics notebooks stored in the workspace mapped limits
- **Datasets & Schemas** — Audit specifically defined storage mappings shaping static or dynamic structures natively inside the limits
- **Linked Services** — Safely extract dependencies indicating external mappings referencing Key Vaults, Blob Storages, or other crucial endpoints

### How it works

1. Subscribe to this server
2. Provide your Azure Synapse Workspace URL and an active Access Token
3. Start dispatching complex analytics queries or debugging pipeline health from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — trace failed pipelines and dissect linked service misconfigurations seamlessly without bouncing back to the Azure portal
- **Data Scientists** — survey available Spark Notebooks and retrieve dataset bounds quickly to evaluate variables right in the AI IDE
- **Cloud Ops** — remotely inspect compute scale thresholds (SQL/Spark pools) answering billing and scaling architecture queries on-demand


## Available Tools
- **list_pipelines**: List all Azure Synapse Analytics data integration pipelines
- **get_pipeline**: Get precise definition of a specific Azure Synapse pipeline
- **list_notebooks**: List all Azure Synapse Spark notebooks
- **list_spark_pools**: List pre-provisioned Apache Spark Analytics pools
- **list_sql_pools**: List dedicated and serverless SQL Analytics pools in Synapse
- **list_datasets**: List all Azure Synapse explicit datasets targets
- **list_linked_services**: List explicit Azure Synapse Linked Services


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Azure Synapse Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the full integration topology for 'NightlyCustomerSync'."

**🤖 AI Agent:**
> I fetched 'NightlyCustomerSync' configurations recursively. It contains 3 connected flow steps. An initial lookup against an external datastore proceeds towards a massive iterative mapping sequence. Would you like me to inspect the target payload for the iteration loop?

---

**👤 You:**
> "List all Spark Notebooks currently stored in this analytic root."

**🤖 AI Agent:**
> You have 12 Apache Spark Notebooks saved. Three are flagged primarily for Marketing ML analysis utilizing the basic 8-core compute provision. The others govern deep ETL mapping routines. Shall we retrieve the metadata code mapping one of them?

---

**👤 You:**
> "Check and audit our externally mapping Linked Services health statuses."

**🤖 AI Agent:**
> I discovered 4 linked services mapped to this workspace constraint natively. 'DataLakeStorageV2' and 'SQLDedicated' indicate active, properly anchored keys. The last one, 'StagingKeyVault', is issuing a deprecation notice for an aging secret token mapping.


## Installation & Usage

To install and use the **Azure Synapse Analytics** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/azure-synapse-analytics](https://vinkius.com/mcp/azure-synapse-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
