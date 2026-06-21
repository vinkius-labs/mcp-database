# Maranhão Open Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/maranhao-open-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access public datasets from Maranhão, Brazil — search packages, inspect resources, and query the datastore via SQL.

## Description
Connect to the **Maranhão Open Data Portal** to explore government transparency data directly through your AI agent. This server interfaces with the state's CKAN-based infrastructure to provide real-time access to public information.

### What you can do

- **Dataset Discovery** — List all available packages or search for specific topics like education, health, or finance using `list_packages` and `search_packages`.
- **Metadata Inspection** — Retrieve detailed metadata for datasets and specific resources (CSV, PDF, API endpoints) with `get_package` and `get_resource`.
- **Data Exploration** — Search within specific resource rows using `search_datastore` or execute complex SQL queries against the DataStore for deep analysis with `search_datastore_sql`.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Maranhão API Key for higher rate limits
3. Start querying public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Journalists** — quickly find and analyze government spending, social indicators, and public contracts.
- **Developers** — integrate public data into applications without manually browsing the portal.
- **Data Analysts** — run SQL queries directly on government datasets to generate insights and reports.


## Available Tools (6)
- **get_package**: Retrieve dataset metadata
- **get_resource**: g., a CSV file or API endpoint within a dataset).

Retrieve resource metadata
- **list_packages**: List all datasets (packages) on the portal
- **search_datastore_sql**: Execute SQL query against the DataStore
- **search_datastore**: Search within a resource in the DataStore
- **search_packages**: Search for datasets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Maranhão Open Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available datasets on the Maranhão Open Data portal."

**🤖 AI Agent:**
> I've retrieved the list of datasets. There are several packages available, including 'Receitas Estaduais', 'Despesas por Órgão', and 'Contratos Públicos'. Which one would you like to explore?

---

**👤 You:**
> "Search for datasets related to 'saúde' (health)."

**🤖 AI Agent:**
> Searching for 'saúde'... I found datasets such as 'Leitos Hospitalares' and 'Vacinação COVID-19'. Do you want the metadata for any of these?

---

**👤 You:**
> "Run a SQL query to select the first 5 rows from the resource 'd3b0c...'."

**🤖 AI Agent:**
> Executing SQL query... Here are the first 5 records from the requested resource, showing columns for Date, Value, and Description.


## ❓ FAQ

**Q: How do I find datasets about a specific topic like 'education'?**
You can use the `search_packages` tool with a query string. For example, searching for 'educação' will return all related datasets available on the portal.

**Q: Can I query the actual content of a CSV file without downloading it?**
Yes! If the resource is in the DataStore, use `search_datastore` with the Resource ID to search through the rows directly.

**Q: Is it possible to perform complex filtering using SQL?**
Absolutely. Use the `search_datastore_sql` tool to execute standard SQL queries against any resource stored in the portal's DataStore.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/maranhao-open-data](https://vinkius.com/mcp/maranhao-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Maranhão Open Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `maranhao-open-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Maranhão Open Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "maranhao-open-data": {
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
