# Tinybird Data Platform MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tinybird-data-platform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Analyze real-time data via Tinybird — manage Data Sources, inspect Pipes, and query endpoints directly.

## Description
Connect your AI agent to **Tinybird**, the real-time data platform for developers. This integration allows you to oversee your analytical infrastructure, manage ingestion storage (Data Sources), and interact with transformation logic (Pipes) through natural conversation.

### What you can do

- **Infrastructure Oversight** — List and inspect all your Data Sources and Pipes in real-time
- **Transformation Analysis** — Retrieve SQL logic and nodes for any Pipe to understand how data is being processed
- **Live Querying** — Execute published Pipes or run arbitrary SQL queries (ClickHouse dialect) to explore your data directly via the agent
- **Operational Metrics** — Check ingestion stats, row counts, and storage sizes for your analytical units
- **Access Control** — List and audit authentication tokens and workspace configurations

### How it works

1. Subscribe to this server
2. Enter your **Tinybird Admin Token** (found in your Tinybird workspace settings)
3. Start analyzing and managing your real-time data flows via chat

### Who is this for?

- **Data Engineers** — quickly audit pipe logic and data source states during development
- **Product Analysts** — run quick SQL queries or check pipe outputs without opening the dashboard
- **DevOps Teams** — monitor ingestion performance and token scopes via AI assistance


## Available Tools (10)
- **execute_sql_query**: Execute an arbitrary SQL query against the Tinybird workspace
- **get_datasource_details**: Get comprehensive information for a specific Data Source
- **get_pipe_details**: Get detailed information for a specific Pipe
- **get_datasource_stats**: Retrieve ingestion and usage statistics for a Data Source
- **list_datasources**: Retrieve a list of all Data Sources in the current workspace
- **list_pipe_nodes**: List all SQL nodes within a specific Pipe
- **list_pipes**: Retrieve a list of all Pipes in the current workspace
- **list_auth_tokens**: Retrieve a list of all authentication tokens in the workspace
- **list_workspaces**: Retrieve a list of available workspaces
- **query_pipe_data**: Execute a Pipe and retrieve the results as JSON


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tinybird Data Platform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all data sources in my Tinybird workspace."

**🤖 AI Agent:**
> Fetching data sources... I found 3 sources: 'events_log' (1.2M rows), 'users_data' (50k rows), and 'api_analytics' (800k rows). Which one would you like to inspect?

---

**👤 You:**
> "Run the pipe 'monthly_revenue_summary' with limit 5."

**🤖 AI Agent:**
> Executing pipe... Here are the top 5 records from 'monthly_revenue_summary': 1. Jan ($12k), 2. Feb ($15k), 3. Mar ($11k)...


## ❓ FAQ

**Q: Where do I find my Tinybird Admin Token?**
Log in to your [**Tinybird Dashboard**](https://app.tinybird.co/), select a workspace, and go to the 'Auth Tokens' section. You can use the Admin Token or create a custom one with the necessary scopes.

**Q: Which SQL dialect does Tinybird use?**
Tinybird is powered by ClickHouse, so it uses the ClickHouse SQL dialect, which includes powerful functions for high-performance analytical processing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tinybird-data-platform](https://vinkius.com/mcp/tinybird-data-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tinybird Data Platform** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tinybird-data-platform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tinybird Data Platform** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tinybird-data-platform": {
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
