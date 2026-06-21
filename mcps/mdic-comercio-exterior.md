# MDIC (Comércio Exterior) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mdic-comercio-exterior)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access Brazilian foreign trade data from MDIC — list datasets, search for trade packages, and query the datastore for export/import statistics.

## Description
Connect to the **MDIC (Ministry of Development, Industry, Trade and Services)** open data portal to analyze Brazilian foreign trade metrics directly through your AI agent.

### What you can do

- **Dataset Discovery** — List and search through all available trade packages (datasets) like 'comex-stat' or 'exportacao-municipios'
- **Metadata Inspection** — Get detailed descriptions, tags, and resource lists for specific trade datasets
- **Direct Data Querying** — Use the Datastore search to filter and retrieve specific rows from CSV resources using SQL-like parameters
- **Resource Management** — Access individual file metadata and download links for trade statistics

### How it works

1. Subscribe to this server
2. (Optional) Provide an API key if required by your specific endpoint for higher rate limits
3. Start querying Brazilian trade data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly fetch trade volumes and export trends without manual downloads
- **Economists** — analyze official government trade data using natural language queries
- **Business Intelligence Leads** — integrate official Brazilian trade statistics into automated reports and dashboards


## Available Tools
- **get_package**: Get detailed metadata for a specific dataset (package)
- **get_resource**: Get metadata for a specific resource (data file)
- **list_packages**: List all datasets (packages) available in the MDIC portal
- **search_datastore**: Query data directly from a resource stored in the Datastore
- **search_packages**: g., "comex", "exportação").

Search for datasets matching a specific query string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MDIC (Comércio Exterior)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for MDIC datasets related to 'exportação'."

**🤖 AI Agent:**
> I found several datasets. The most relevant are 'exportacao-municipios-detalhada' and 'comex-stat-exportacao'. Which one would you like to inspect for metadata?

---

**👤 You:**
> "List the resources available in the 'comex-stat' package."

**🤖 AI Agent:**
> The 'comex-stat' package contains 12 resources, including 'Exportações Mensais (CSV)' and 'Importações Mensais (CSV)'. I have the resource IDs ready if you want to query the data.

---

**👤 You:**
> "Query the first 5 rows from resource ID d3b0c1... with a limit of 5."

**🤖 AI Agent:**
> Retrieved 5 rows from the datastore. The data includes columns for 'Year', 'Month', 'Product_Code', and 'Value_FOB'. Would you like me to summarize these results?


## ❓ FAQ

**Q: Can I search for specific trade terms like 'soybean' or 'iron ore'?**
Yes! Use the `search_packages` tool with your query string. It will return all datasets matching those terms within the MDIC portal.

**Q: How do I access the actual data rows inside a CSV resource?**
Use the `search_datastore` tool by providing the `resource_id`. You can also apply filters and limits to retrieve exactly the data points you need.

**Q: Is it possible to see the file format and download URL for a dataset?**
Yes. The `get_package` tool returns a list of resources, and `get_resource` provides specific metadata including the format (CSV, XLSX, etc.) and the direct download URL.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mdic-comercio-exterior](https://vinkius.com/mcp/mdic-comercio-exterior)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MDIC (Comércio Exterior)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mdic-comercio-exterior` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MDIC (Comércio Exterior)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mdic-comercio-exterior": {
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
