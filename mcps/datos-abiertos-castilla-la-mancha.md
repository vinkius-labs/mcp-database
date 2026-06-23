# Datos Abiertos Castilla-La Mancha MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datos-abiertos-castilla-la-mancha)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the official Open Data portal of Castilla-La Mancha. Explore datasets, resources, and query tabular data directly through your AI agent.

## Description
Connect to the **Castilla-La Mancha Open Data** portal and explore a wealth of public information from the Spanish region directly through your AI agent. This server allows you to navigate the official CKAN-based repository to find datasets related to economy, environment, health, and more.

### What you can do

- **Dataset Discovery** — List all available datasets and browse through the portal's catalog using tags and identifiers.
- **Metadata Inspection** — Fetch detailed information about specific datasets, including descriptions, update frequency, and maintainers.
- **Resource Access** — Identify specific files (CSV, JSON, PDF) within a dataset and retrieve their direct access metadata.
- **Data Querying** — Search and filter records directly within tabular resources (CSV/Datastore) without downloading the entire file.
- **Tag Navigation** — Explore the organizational structure of the portal by listing all active tags and categories.

### How it works

1. Subscribe to this server
2. Enter your API Key from the portal (optional for public data but recommended for higher limits)
3. Start querying regional data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find and sample regional statistics for research or reporting.
- **Developers** — integrate public data sources into applications by testing queries through the AI.
- **Citizens & Researchers** — navigate complex public records using natural language instead of manual portal searches.


## Available Tools (5)
- **get_dataset**: Get details for a specific dataset
- **get_resource**: Get details for a specific resource
- **list_datasets**: List all datasets in the portal
- **list_tags**: List all tags in the portal
- **search_datastore**: Search records within a datastore resource


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Datos Abiertos Castilla-La Mancha** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available datasets from the Castilla-La Mancha Open Data portal."

**🤖 AI Agent:**
> I have retrieved the list of datasets. There are numerous entries including 'Presupuesto 2024', 'Calidad del Aire', and 'Centros Educativos'. Which one would you like to explore in detail?

---

**👤 You:**
> "Search for the first 5 records in the datastore resource 'd4e5f6a7-b8c9'."

**🤖 AI Agent:**
> Querying the datastore... I found the first 5 rows for resource 'd4e5f6a7-b8c9'. The data includes fields such as 'Municipio', 'Población', and 'Año'. Would you like me to summarize these records?

---

**👤 You:**
> "Get the metadata and resources for the dataset 'centros-sanitarios'."

**🤖 AI Agent:**
> Fetching details for 'centros-sanitarios'... This dataset contains information about health centers in the region. It has 3 resources available: a CSV file (ID: res-123), an Excel file, and a GeoJSON map. Do you want to search inside the CSV data?


## ❓ FAQ

**Q: Can I search for specific records inside a CSV file without downloading it?**
Yes! Use the `search_datastore` tool with the Resource ID. You can apply filters and limits to query the data rows directly from the portal's internal database.

**Q: How do I find all available datasets in the portal?**
Simply run the `list_datasets` tool. It will return a comprehensive list of dataset identifiers that you can then inspect further using `get_dataset`.

**Q: Can I see the categories or tags used to organize the data?**
Yes, use the `list_tags` tool to retrieve all the keywords and categories used by the Castilla-La Mancha portal to classify their information.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datos-abiertos-castilla-la-mancha](https://vinkius.com/mcp/datos-abiertos-castilla-la-mancha)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Datos Abiertos Castilla-La Mancha** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `datos-abiertos-castilla-la-mancha` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Datos Abiertos Castilla-La Mancha** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "datos-abiertos-castilla-la-mancha": {
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
