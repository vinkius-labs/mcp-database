# Cube.dev MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cubedev)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Access your Cube semantic layer — execute queries, inspect generated SQL, manage pre-aggregations, and explore data metadata directly.

## Description
Connect your **Cube.dev** instance to any AI agent to bridge the gap between natural language and your data warehouse. This server allows your agent to interact with Cube's semantic layer, ensuring consistent metrics and high-performance data retrieval.

### What you can do

- **Data Querying** — Execute complex REST API queries using `load_query` to fetch aggregated data with measures, dimensions, and filters.
- **SQL Inspection** — Use `get_sql` and `execute_cube_sql` to debug or run raw queries against the SQL API for deep data investigation.
- **Metadata Exploration** — Retrieve cube definitions, views, and segments via `get_meta` to understand your data model without leaving the chat.
- **Performance Management** — Trigger and monitor background pre-aggregation builds with `trigger_pre_aggregation_job` to ensure your dashboards stay fast.
- **Cloud Management** — List deployments and environments if using Cube Cloud to manage your infrastructure context.

### How it works

1. Subscribe to this server
2. Provide your Cube API URL and Secret Token
3. Start asking questions about your data metrics and model structure

### Who is this for?

- **Data Engineers** — quickly verify data models and trigger cache refreshes via CLI or AI interface.
- **Analytics Engineers** — debug generated SQL and inspect metadata to ensure metric consistency.
- **Product Managers** — get instant answers to data questions by letting the AI query the semantic layer directly.


## Available Tools (15)
- **check_live**: Check if Cube deployment is live
- **check_ready**: Check if Cube deployment is ready
- **convert_query**: Convert a SQL query to a REST API query format
- **execute_cube_sql**: Execute a raw SQL query against the SQL API
- **generate_meta_token**: Requires CUBE_CLOUD_API_KEY.

Generate a JWT for the Metadata API
- **get_entity**: Get detailed metadata for a specific entity
- **get_meta**: Get metadata for cubes and views
- **get_pre_aggregation_job_status**: Get status of pre-aggregation jobs
- **get_sql**: Useful for debugging.

Get generated SQL for a Cube query
- **list_data_sources**: List configured data sources
- **list_deployments**: Requires CUBE_CLOUD_API_KEY.

List all Cube Cloud deployments
- **list_entities**: List all cubes and views
- **list_environments**: Requires CUBE_CLOUD_API_KEY.

List environments for a deployment
- **load_query**: Use this to get aggregated data.

Execute a Cube query and return results
- **trigger_pre_aggregation_job**: Trigger a pre-aggregation build job


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cube.dev** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the metadata for all available cubes and views."

**🤖 AI Agent:**
> I've retrieved the metadata. You have cubes for 'Orders', 'Users', and 'Products'. The 'Orders' cube includes measures like 'count' and 'totalAmount', and dimensions like 'status' and 'createdAt'.

---

**👤 You:**
> "Run a query to get the total count of orders grouped by status for the last 30 days."

**🤖 AI Agent:**
> Executing `load_query`... The results show 150 'completed' orders, 20 'pending', and 5 'cancelled' for the requested period.

---

**👤 You:**
> "Trigger a pre-aggregation build for the 'Sales' cube."

**🤖 AI Agent:**
> I've triggered the pre-aggregation job for the 'Sales' cube using `trigger_pre_aggregation_job`. You can check the status using the job token provided.


## ❓ FAQ

**Q: Can I see the exact SQL that Cube generates for a specific query?**
Yes. You can use the `get_sql` tool. By providing the query JSON, the agent will return the generated SQL string, which is perfect for debugging or verifying your data logic.

**Q: How do I refresh the data cache or pre-aggregations using the AI?**
You can use the `trigger_pre_aggregation_job` tool. You can specify which cubes or data sources to target, and the agent will initiate the background build process for you.

**Q: Is it possible to explore the available measures and dimensions?**
Absolutely. Use the `get_meta` tool to fetch all metadata. This allows the AI to understand what data is available to be queried, including views and segments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cubedev](https://vinkius.com/mcp/cubedev)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cube.dev** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cubedev` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cube.dev** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cubedev": {
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
