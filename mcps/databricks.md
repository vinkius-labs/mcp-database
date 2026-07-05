# Databricks MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/databricks)
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


## Available Tools (8)
- **list_schemas**: List schemas in catalog from Databricks
- **get_me**: Get current user from Databricks
- **list_warehouses**: List SQL warehouses from Databricks
- **list_catalogs**: List Unity Catalog catalogs from Databricks
- **list_clusters**: List all clusters from Databricks
- **get_cluster**: Get cluster details from Databricks
- **list_jobs**: List all jobs from Databricks
- **list_job_runs**: List job runs from Databricks


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


## ❓ FAQ

**Q: Can my agent check the status of a specific Databricks job run?**
Yes. Provide the 'job_id' to the 'list_job_runs' tool. The agent will retrieve the chronological history of executions, allowing you to identify successful completions or precise points of failure in your workflows.

**Q: How do I explore schemas within a specific Unity Catalog via chat?**
Use the 'list_schemas' tool and provide the catalog name. Your agent will pull the detailed databases and schemas registered inside that Unity Catalog, giving you immediate visibility into your data hierarchy.

**Q: Can I monitor the health of my Databricks clusters through the agent?**
Absolutely. The 'list_clusters' and 'get_cluster' tools allow your agent to retrieve detailed node information and operational statuses, helping you audit cluster health and capacity across your workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/databricks](https://vinkius.com/mcp/databricks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Databricks** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `databricks` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Databricks** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "databricks": {
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
