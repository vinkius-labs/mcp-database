# Aragón Open Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aragon-open-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access public data from the Government of Aragón — query datasets, preview views, and explore the CKAN catalog directly from your AI agent.

## Description
Connect to the **Aragón Open Data** portal and unlock a wealth of public information from the Government of Aragón. This MCP server allows your AI agent to browse, search, and analyze regional datasets, statistical views, and organizational metadata through natural language.

### What you can do

- **Data Exploration** — List all available views and datasets from the GA_OD_Core and CKAN catalogs.
- **Deep Data Preview** — Fetch and preview actual records from specific views or resources with support for filtering and pagination.
- **Schema Inspection** — Understand the structure of data by retrieving column names and data types for any specific view.
- **Advanced Search** — Use Solr-powered queries to find specific datasets, tags, or organizations within the public catalog.
- **Publisher Insights** — Retrieve detailed information about the organizations and themes (groups) that publish data in the region.

### How it works

1. Subscribe to this server
2. Enter your Aragón Open Data API Key (optional for public endpoints)
3. Start querying public records from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find and preview regional statistics without manual CSV downloads
- **Developers** — inspect API schemas and data structures directly from the code editor
- **Researchers & Journalists** — search for public records and government transparency data through conversation


## Available Tools (15)
- **count_datasets**: Get total dataset count
- **get_organization**: Get publisher/organization details
- **get_dataset**: Get dataset details
- **get_tag**: Get tag details
- **list_groups**: List all themes/groups
- **list_organizations**: List all publishers/organizations
- **list_datasets**: List all datasets (packages)
- **list_tags**: List all tags
- **list_views**: List all available views in Aragón Open Data
- **most_downloaded_datasets**: Get most downloaded datasets
- **newest_datasets**: Get newest datasets
- **preview_data**: By default, it returns the first 1000 records.

Preview data from a view or resource
- **query_sparql**: Supports ontologies like EI2A, Aragopedia, ELI, and DataCube.

Execute a SPARQL query
- **search_datasets**: Search for datasets
- **show_columns**: Get information about columns for a specific view


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aragón Open Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available data views in Aragón Open Data."

**🤖 AI Agent:**
> I've retrieved the list of available views. There are several registered views including 'Censo de Viviendas', 'Presupuestos Municipales', and 'Calidad del Aire'. Which one would you like to explore?

---

**👤 You:**
> "Search for datasets related to 'turismo' in the catalog."

**🤖 AI Agent:**
> Searching the CKAN catalog... I found several datasets related to tourism, such as 'Ocupación Turística' and 'Red de Oficinas de Turismo'. Would you like the details for a specific one?

---

**👤 You:**
> "Show me the first 5 records from the view with ID '702'."

**🤖 AI Agent:**
> Fetching data preview for view 702... Here are the first 5 records containing fields like 'Municipio', 'Año', and 'Valor'. The data shows a breakdown of local demographics for the selected period.


## ❓ FAQ

**Q: Can I filter the data preview to see only specific records?**
Yes! Use the `preview_data` tool and provide a JSON string in the `filters` parameter (e.g., `{"entidad": "ARANDA"}`). This allows you to restrict the results to exactly what you need.

**Q: How do I find the structure and data types of a specific view?**
You can use the `show_columns` tool by providing the `view_id`. It will return a detailed list of all columns, their descriptions, and their technical data types.

**Q: Is it possible to search for datasets by keywords or topics?**
Absolutely. Use the `search_datasets` tool with the `q` parameter to perform a Solr search across the entire CKAN catalog for relevant datasets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aragon-open-data](https://vinkius.com/mcp/aragon-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aragón Open Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aragon-open-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aragón Open Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aragon-open-data": {
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
