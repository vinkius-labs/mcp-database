# Comunidad de Madrid (Portal Regional) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/comunidad-de-madrid-portal-regional)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the official Open Data portal of the Community of Madrid. Search datasets, inspect public resources, and query the datastore for regional information.

## Description
Connect your AI agent to the **Comunidad de Madrid Open Data Portal** to access a wealth of public information directly through natural language. This MCP server provides a bridge to the regional CKAN-based repository, covering everything from transport and health to environment and economy.

### What you can do

- **Dataset Discovery** — Search for specific datasets using keywords like 'transporte', 'salud', or 'medio ambiente' to find relevant public records.
- **Metadata Inspection** — Retrieve full metadata for datasets, including tags, organizations, and update frequencies.
- **Resource Management** — List and inspect individual files (resources) within a dataset, such as CSVs, JSONs, or PDFs.
- **Direct Data Querying** — Use the DataStore integration to query the actual content of datasets directly, allowing for data analysis without manual downloads.
- **Portal Exploration** — List all available dataset identifiers to understand the scope of available regional data.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Comunidad de Madrid CKAN API Key for higher rate limits
3. Start querying regional data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly pull regional statistics and records into your workflow for analysis.
- **Developers** — integrate real-time public data from Madrid into applications without navigating complex API docs.
- **Researchers & Citizens** — find public information about air quality, transport schedules, or economic indicators through simple conversation.


## Available Tools
- **get_dataset**: Get full metadata for a specific dataset
- **get_resource**: Get metadata for a specific resource
- **list_datasets**: List all dataset identifiers in the portal
- **search_datasets**: g., transporte, salud).

Search for datasets matching specific criteria
- **search_datastore**: Query data directly from a resource in the DataStore


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Comunidad de Madrid (Portal Regional)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets related to air quality in Madrid."

**🤖 AI Agent:**
> I found several datasets. The most relevant is 'Calidad del aire: datos diarios' (ID: calidad_aire_datos_dia). Would you like to see its metadata or available resources?

---

**👤 You:**
> "List all dataset identifiers available in the portal."

**🤖 AI Agent:**
> Fetching the list of datasets... There are over 500 datasets available. Some examples include 'centros_salud', 'transporte_publico_lineas', and 'presupuestos_municipales'.

---

**👤 You:**
> "Get the metadata for the dataset 'calidad_aire_datos_dia'."

**🤖 AI Agent:**
> The dataset 'Calidad del aire: datos diarios' is managed by the Environment department. It contains 12 resources (CSV and Excel files) and is updated daily. Would you like the ID of the latest CSV resource?


## ❓ FAQ

**Q: How can I find datasets about a specific topic like 'transport'?**
Use the `search_datasets` tool with the query 'transporte'. The agent will return a list of matching datasets with their unique IDs and descriptions from the portal.

**Q: Can I see the actual content of a data file without downloading it?**
Yes. If the resource is stored in the CKAN DataStore, you can use the `search_datastore` tool with the Resource ID to query the rows and columns directly.

**Q: Is an API key mandatory to use this server?**
No, it is optional. However, providing a `CKAN_API_KEY` allows for higher rate limits and access to restricted datasets if your account has permissions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/comunidad-de-madrid-portal-regional](https://vinkius.com/mcp/comunidad-de-madrid-portal-regional)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Comunidad de Madrid (Portal Regional)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `comunidad-de-madrid-portal-regional` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Comunidad de Madrid (Portal Regional)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "comunidad-de-madrid-portal-regional": {
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
