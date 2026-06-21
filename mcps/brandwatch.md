# Brandwatch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brandwatch)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Access consumer research via Brandwatch — list projects, track queries, and retrieve social mentions directly from any AI agent.

## Description
Connect your **Brandwatch Consumer Research** account to any AI agent and orchestrate your social listening and data analysis workflows through natural conversation.

### What you can do

- **Project & Dashboard Navigation** — List and retrieve detailed metadata for all your active research projects and dashboards.
- **Query Management** — Access your configured search queries to monitor brand health and industry trends.
- **Mention Retrieval** — Query and inspect raw social mentions based on specific queries and date ranges.
- **Data Aggregation** — Retrieve volume aggregates to analyze mention trends and spikes over time.
- **Tag Coordination** — List and create categorization tags to organize your social data effectively.

### How it works

1. Subscribe to this server
2. Enter your Brandwatch API Username, Password, and Client ID
3. Start analyzing social data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly retrieve mention volumes and raw data without manual CSV exports.
- **Social Media Managers** — monitor query performance and brand sentiment straight from their workflow tools.
- **Market Researchers** — analyze trends and track customized tags using natural language.


## Available Tools
- **create_tag**: Create a new tag for categorizing mentions
- **get_mentions**: Retrieve mentions for a specific query
- **get_project**: Get details of a specific project
- **get_volume_aggregates**: Get mention volume aggregates for a query
- **list_dashboards**: List dashboards in a project
- **list_projects**: List all active projects
- **list_queries**: List configured queries in a project
- **list_tags**: List tags available in a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brandwatch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all queries configured in project proj_1."

**🤖 AI Agent:**
> I've retrieved the queries for project proj_1. You have 3 queries running: 'Brand Name Mentions' (ID: q_1), 'Competitor X' (ID: q_2), and 'Industry Trends' (ID: q_3).

---

**👤 You:**
> "Get volume aggregates for query q_1 from Jan 1st to Jan 31st."

**🤖 AI Agent:**
> Retrieving data... There were 15,200 mentions in total during January. The highest spike occurred on Jan 15th with 4,500 mentions.

---

**👤 You:**
> "Create a new tag called 'Urgent Review' in project proj_1."

**🤖 AI Agent:**
> The tag 'Urgent Review' has been successfully created in your project. You can now use it to categorize mentions.


## ❓ FAQ

**Q: Can I retrieve social mentions for a specific date range?**
Yes! Use the `get_mentions` tool with the Project ID, Query ID, and your ISO 8601 formatted start and end dates (e.g., 2024-01-01T00:00:00.000Z).

**Q: How do I see the volume trend of a query over time?**
Simply ask the agent to `get_volume_aggregates` and provide the relevant IDs and date range. It will return the aggregated data points showing mention spikes.

**Q: Does the integration allow creating new boolean queries?**
Currently, the toolset is focused on reading and retrieving data from existing setups. Creating complex boolean queries should be done via the Brandwatch web interface to utilize their query builder and syntax validation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brandwatch](https://vinkius.com/mcp/brandwatch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brandwatch** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `brandwatch` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brandwatch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brandwatch": {
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
