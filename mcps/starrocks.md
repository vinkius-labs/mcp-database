# StarRocks MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/starrocks)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

High-performance analytical database — manage clusters, tables, and query data via AI.

## Description
Empower your AI agent to orchestrate your high-performance OLAP infrastructure with **StarRocks**, the leading distributed analytical database. By connecting StarRocks to your agent, you transform complex cluster auditing, schema management, and data querying into a natural conversation. Your agent can instantly list databases, retrieve table schemas, monitor backend nodes, and even execute complex SQL queries without you ever needing to open a SQL terminal or the StarRocks Manager. Whether you are conducting a data audit or monitoring real-time ingestion jobs, your agent acts as a real-time data reliability assistant, keeping your analytical platform accurate and your insights moving.

### What you can do

- **Database Orchestration** — List all databases and retrieve detailed table schemas and structures.
- **Analytical Querying** — Execute arbitrary SQL queries directly through the agent to retrieve real-time insights.
- **Cluster Monitoring** — Browse status and metadata for Frontend (FE) and Backend (BE) nodes to audit health.
- **Ingestion Control** — Monitor data load jobs and historical ingestion performance for your analytical pipelines.
- **Storage Insights** — Retrieve disk usage and data size statistics across the entire distributed cluster.

### How it works

1. Subscribe to this server
2. Enter your StarRocks FE Host, Port, User, and Password
3. Start managing your OLAP infrastructure through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — automate schema auditing and monitor ingestion pipelines through natural language queries.
- **Analytics Leads** — coordinate data access and audit materialized views directly from your AI-powered workspace.
- **Infrastructure SREs** — monitor cluster node health and storage usage via a unified AI interface.
- **StarRocks Power Users** — integrate your existing analytical workflows into your AI-driven daily routines.


## Available Tools (10)
- **execute_query**: Execute arbitrary SQL query
- **get_cluster_info**: Get frontend nodes info
- **get_storage_usage**: Get data storage statistics
- **get_table_schema**: Get table structure
- **list_databases**: List all databases
- **list_jobs**: List data load jobs
- **list_mvs**: List materialized views
- **list_nodes**: List backend nodes
- **list_tables**: List tables in a database
- **list_views**: List database views


## 💬 Prompt Examples

Here are some examples of how you can interact with the **StarRocks** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all databases in my StarRocks cluster."

**🤖 AI Agent:**
> I've retrieved your StarRocks databases. You have 5 databases, including 'sales_analytics', 'user_behavior', and 'logs_archive'. Which one would you like to see the tables for?

---

**👤 You:**
> "Show me the average order value from the 'sales' table."

**🤖 AI Agent:**
> I've executed the query. The average order value across the 'sales' table is $142.50. Would you like a breakdown of this metric by region or product category?

---

**👤 You:**
> "Check for any offline backend nodes."

**🤖 AI Agent:**
> I've checked the backend nodes. All 10 Backend (BE) nodes are currently online and healthy. CPU and memory usage across the cluster is within normal limits.


## ❓ FAQ

**Q: How do I find my StarRocks FE Host and Port?**
The FE Host is the IP address or domain of your StarRocks Frontend node. The default HTTP port is 8030. You can verify these in your deployment configuration or by contacting your administrator.

**Q: Can I execute DELETE or UPDATE queries through this server?**
Yes. Use the `execute_query` tool. As long as your authenticated user has the necessary permissions in StarRocks, you can execute any valid SQL statement, including DDL and DML operations.

**Q: Is it possible to monitor cluster health through the agent?**
Yes! Use the `get_cluster_info` and `list_nodes` tools to retrieve real-time status for all Frontend and Backend nodes, helping you identify offline or overloaded nodes instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/starrocks](https://vinkius.com/mcp/starrocks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **StarRocks** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `starrocks` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **StarRocks** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "starrocks": {
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
