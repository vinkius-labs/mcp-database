# Omni BI Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/omni-bi-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Interact with Omni BI dashboards, models, and data exports — run queries and track metrics directly from your AI agent.

## Description
Connect your **Omni BI** (omni.co) account to your AI agent and gain deep insights into your organization's data through natural conversation and programmatic query execution.

### What you can do

- **Dashboard Oversight** — List all available BI dashboards and retrieve detailed layout and component metadata.
- **Data Model Intelligence** — Access the semantic layer to list models and inspect specific field definitions and logic.
- **Programmatic Queries** — Execute custom queries against your data models directly from the chat and view results.
- **Resource Management** — Browse workspaces, folders, and projects to stay organized within your BI instance.
- **Connection Monitoring** — List all connected databases and data sources integrated with Omni.
- **Data Export** — Generate temporary export links for query results in CSV, JSON, or Excel formats.
- **Deep Inspection** — Fetch complete metadata for specific fields, dashboards, or data models using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Omni BI Instance URL and API Key (Bearer Token)
3. Start exploring your business intelligence from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts** — quickly check model field logic or run ad-hoc queries without opening the UI.
- **Business Leads** — monitor key dashboard metrics and organization workspaces through natural language.
- **Operations Teams** — automate the retrieval of data exports and model metadata for reporting.


## Available Tools (10)
- **export_query_results**: Export data to file
- **get_dashboard_details**: Get specific dashboard info
- **get_field_details**: Get specific field info
- **get_model_details**: Get data model metadata
- **list_data_connections**: List database connections
- **list_dashboards**: List BI dashboards
- **list_resource_folders**: List dashboard folders
- **list_data_models**: List Omni data models
- **list_bi_workspaces**: List organization workspaces
- **run_omni_query**: Run programmatic query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Omni BI Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our sales dashboards."

**🤖 AI Agent:**
> Retrieving dashboards... I found 5 related to sales, including 'Global Revenue Overview', 'Quarterly Performance', and 'Sales by Region'. Would you like the component details for the Revenue Overview?

---

**👤 You:**
> "Run a query on the 'Orders' model for fields 'total_price' and 'status'."

**🤖 AI Agent:**
> Executing query... I've retrieved the latest 100 records from the Orders model. The data includes prices ranging from $45 to $1,200 across 'shipped' and 'pending' statuses. Shall I generate a CSV export link for the full result set?

---

**👤 You:**
> "What are the field definitions for the 'Customer Retention' model?"

**🤖 AI Agent:**
> Fetching model details... The 'Customer Retention' model contains 12 fields including 'cohort_month', 'retention_rate' (measure), and 'active_user_count'. Would you like the specific calculation logic for the retention rate?


## ❓ FAQ

**Q: How do I get an Omni BI API Key?**
Log in to your Omni instance, navigate to user settings or organization settings, and look for the API Tokens section to generate a new token.

**Q: Can I run raw SQL queries?**
This implementation uses the `run_omni_query` tool which interacts with your defined data models (semantic layer). Raw SQL access depends on your specific model configuration in Omni.

**Q: What formats are supported for data export?**
The `export_query_results` tool supports CSV, JSON, and XLSX formats. You will receive a temporary URL to download the requested file.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/omni-bi-intelligence](https://vinkius.com/mcp/omni-bi-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Omni BI Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `omni-bi-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Omni BI Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "omni-bi-intelligence": {
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
