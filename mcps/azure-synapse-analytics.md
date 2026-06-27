# Azure Synapse Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/azure-synapse-analytics)
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


## Available Tools (7)
- **list_datasets**: List all Azure Synapse explicit datasets targets
- **list_pipelines**: List all Azure Synapse Analytics data integration pipelines
- **get_pipeline**: Get precise definition of a specific Azure Synapse pipeline
- **list_notebooks**: List all Azure Synapse Spark notebooks
- **list_spark_pools**: List pre-provisioned Apache Spark Analytics pools
- **list_sql_pools**: List dedicated and serverless SQL Analytics pools in Synapse
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


## ❓ FAQ

**Q: Can I audit completely isolated Spark clusters running heavy tasks?**
Yes. Ask the agent to pull your active or paused `list_spark_pools`. It exposes pre-provisioned engine nodes along with boundaries explicitly defining core-node dimensions for analytic scaling operations.

**Q: Can my AI pinpoint the exact failing task inside an ETL pipeline?**
Using the specific `get_pipeline` action equipped with the exact target name, the agent unfolds the raw underlying JSON orchestration topology. You can trace its target execution mappings, identifying incorrectly bounded inputs right on your prompt window.

**Q: Is it possible to diagnose broken connectivity to external Azure services?**
Yes! The agent can invoke the built-in Linked Services inspector. This extracts all distinct dependencies attached to your current scope, such as mapping paths to a lost Key Vault or orphaned CosmosDB. Finding blind spots has never been faster.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/azure-synapse-analytics](https://vinkius.com/mcp/azure-synapse-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Azure Synapse Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `azure-synapse-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Azure Synapse Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "azure-synapse-analytics": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
