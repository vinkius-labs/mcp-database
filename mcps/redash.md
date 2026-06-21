# Redash MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/redash)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Connect to Redash to manage SQL queries, execute data visualizations, and monitor dashboards directly from your AI agent.

## Description
Connect your **Redash** instance to any AI agent to interact with your data through natural language. This server allows you to bridge the gap between raw data and actionable insights.

### What you can do

- **Query Management** — List, create, and update SQL queries. Archive old queries to keep your workspace clean.
- **Data Execution** — Execute queries on-demand, handle parameters, and fetch fresh or cached results.
- **Dashboard Access** — Browse and retrieve dashboard configurations and visualizations.
- **Data Source Inspection** — Check the status and configuration of your connected data sources.
- **Job Tracking** — Monitor the progress of long-running query executions (jobs).

### How it works

1. Subscribe to this server
2. Provide your Redash Base URL and API Key
3. Start asking your AI to run reports or fetch data metrics

### Who is this for?

- **Data Analysts** — Quickly iterate on SQL queries and check results without switching tabs.
- **Business Intelligence Leads** — Monitor dashboard statuses and share insights via chat.
- **Engineers** — Test data source connections and manage query objects programmatically through the agent.


## Available Tools (17)
- **archive_dashboard**: Archive the specified dashboard
- **archive_query**: Archive the specified query
- **create_dashboard**: Create a new dashboard object
- **create_query**: Create a new query object
- **execute_query**: Parameters must be provided for parameterized queries.

Initiates a new query execution or returns a cached result
- **get_cached_query_result**: Get a cached result for a query ID (non-parameterized only)
- **get_dashboard**: Returns an individual dashboard object
- **get_data_source**: Get data source details
- **get_job**: SUCCESS includes query_result_id.

Returns the status of a query task (job)
- **get_query_result**: Returns a query result by its result ID
- **get_query**: Get an individual query object
- **list_dashboards**: Returns a paginated array of dashboard objects
- **list_queries**: List Redash queries
- **test_data_source**: Test connection for a data source
- **update_dashboard**: Edit an existing dashboard object
- **update_data_source**: Configure a data source (e.g., SSH tunnel)
- **update_query**: Edit an existing query object


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Redash** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Redash queries."

**🤖 AI Agent:**
> I've retrieved your queries. You have 12 active queries, including 'Monthly Revenue' (ID: 45) and 'User Growth' (ID: 82). Would you like to see the details of a specific one?

---

**👤 You:**
> "Execute query ID 45 and show me the fresh results."

**🤖 AI Agent:**
> Starting execution for query 45... The job is finished. Here are the results: Total Revenue for October was $124,500 across 1,200 transactions.

---

**👤 You:**
> "Show me the 'Sales Overview' dashboard details."

**🤖 AI Agent:**
> I've fetched the 'Sales Overview' dashboard (slug: sales-overview). It contains 4 widgets: Revenue Chart, Regional Breakdown, Top Sales Reps, and Monthly Target Progress.


## ❓ FAQ

**Q: How do I run a query and get the results?**
Use the `execute_query` tool. If the query takes time, it returns a `job_id`. You can then use `get_job` to check the status, and once successful, use `get_query_result` with the provided ID to fetch the data.

**Q: Can I update the SQL of an existing query through the agent?**
Yes! Use the `update_query` tool by providing the Query ID and the new SQL string in the `query` parameter. You can also update the name or data source ID.

**Q: How do I find a specific dashboard and its widgets?**
First, use `list_dashboards` to find the slug of the dashboard you need. Then, use the `get_dashboard` tool with that slug to retrieve all its configuration details and widgets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/redash](https://vinkius.com/mcp/redash)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Redash** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `redash` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Redash** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "redash": {
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
