# Mato Grosso do Sul Open Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mato-grosso-do-sul-open-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access public datasets from the state of Mato Grosso do Sul (Brazil) — list packages, search datastores, and query public records via SQL.

## Description
Connect to the **Mato Grosso do Sul (MS) Open Data Portal** to explore and analyze public information from the Brazilian state. This server allows AI agents to programmatically access datasets, organizations, and specific resource records.

### What you can do

- **Datasets & Packages** — List all available public data packages and retrieve detailed metadata using `list_packages` and `get_package`.
- **Resource Inspection** — Drill down into specific files or links within datasets to understand their structure with `get_resource`.
- **DataStore Search** — Filter and search through actual records in CSVs or spreadsheets directly using `datastore_search`.
- **SQL Queries** — Execute complex SQL statements on DataStore resources for advanced data analysis with `datastore_search_sql`.
- **Organizational Context** — List the government organizations and groups responsible for the data via `list_organizations` and `list_groups`.

### How it works

1. Subscribe to this server
2. Enter your Mato Grosso do Sul Data Portal API Key
3. Start querying public state data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — instantly retrieve and filter state records without manual downloads
- **Researchers** — automate the collection of public metadata and resource links
- **Developers** — integrate real-time public data into applications using SQL queries


## Available Tools (7)
- **get_package**: Get details of a specific dataset package
- **get_resource**: Get details of a specific resource
- **list_groups**: List all groups
- **list_organizations**: List all organizations
- **list_packages**: List all dataset packages
- **datastore_search_sql**: Execute a SQL query on DataStore resources
- **datastore_search**: Search data in a DataStore resource


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mato Grosso do Sul Open Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the public data packages available in Mato Grosso do Sul."

**🤖 AI Agent:**
> I've retrieved the list of available packages. There are several datasets including 'frota-de-veiculos', 'receita-corrente-liquida', and 'gastos-com-pessoal'. Which one would you like to explore?

---

**👤 You:**
> "Search for records containing 'Campo Grande' in the resource ID 550e8400-e29b-41d4-a716-446655440000."

**🤖 AI Agent:**
> Searching the DataStore... I found 15 records matching 'Campo Grande' in that resource. Most relate to urban infrastructure projects. Should I list the specific values for you?

---

**👤 You:**
> "Run a SQL query to select all columns from resource 'receita-2023' where the value is greater than 1000000."

**🤖 AI Agent:**
> Executing SQL query on the DataStore... The query returned 8 high-value entries. The largest entry is for 'Transferências Constitucionais' with a value of 5,400,000. Would you like the full breakdown?


## ❓ FAQ

**Q: How do I find specific datasets about health or education?**
Use the `list_packages` tool to see all available dataset names, then use `get_package` with a specific ID to see the resources and descriptions related to that topic.

**Q: Can I perform complex filtering on the data records?**
Yes! Use the `datastore_search_sql` tool to execute standard SQL queries (e.g., SELECT, WHERE, GROUP BY) directly against the DataStore resources for precise analysis.

**Q: How do I see which government departments provide the data?**
Use the `list_organizations` action. It will return a list of all state entities and departments that have published data on the portal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mato-grosso-do-sul-open-data](https://vinkius.com/mcp/mato-grosso-do-sul-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mato Grosso do Sul Open Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mato-grosso-do-sul-open-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mato Grosso do Sul Open Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mato-grosso-do-sul-open-data": {
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
