# Región de Murcia Datos Abiertos MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/region-de-murcia-datos-abiertos)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access the official open data portal of the Region of Murcia (Spain) to query datasets, organizations, and public statistics.

## Description
Connect your AI agent to the **Región de Murcia Datos Abiertos** portal. This MCP server provides direct access to the CKAN-based catalog of the regional government of Murcia, Spain, allowing you to explore a wealth of public information.

### What you can do

- **Dataset Discovery** — Search through thousands of public datasets using keywords or list all available identifiers in the catalog.
- **Detailed Metadata** — Retrieve complete metadata for specific datasets, including descriptions, formats, and resource links.
- **Organizational Insights** — List and explore the various government organizations and groups that publish data on the portal.
- **Trend Tracking** — Instantly fetch the most recently updated or the most viewed datasets to stay informed on regional trends.
- **Public Transparency** — Access data regarding economy, environment, demographics, and infrastructure directly through natural language.

### How it works

1. Subscribe to this server
2. Enter your Murcia API Key (optional for public data, but recommended for higher rate limits)
3. Start querying Spanish regional data from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts** — quickly find and inspect regional statistics without manual portal navigation
- **Researchers & Students** — gather public data for academic or social studies via simple conversation
- **Developers** — integrate real-time public data sources into applications using AI-assisted discovery


## Available Tools (7)
- **get_most_recent_datasets**: Get the most recently added datasets
- **get_most_viewed_datasets**: Get the most viewed datasets
- **list_organizations**: List all organizations in the catalog
- **get_dataset**: Get details for a specific dataset
- **list_datasets**: List all datasets in the catalog
- **list_groups**: List all groups in the catalog
- **search_datasets**: Search for datasets in the catalog


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Región de Murcia Datos Abiertos** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets about 'medio ambiente' in the Murcia portal."

**🤖 AI Agent:**
> I found several datasets related to the environment. Notable ones include 'Calidad del aire' and 'Espacios naturales protegidos'. Would you like the details for any of these?

---

**👤 You:**
> "Show me the 10 most viewed datasets in Murcia."

**🤖 AI Agent:**
> The most viewed datasets include the 'Directorio de Centros Educativos', 'Presupuestos Municipales', and 'Evolución de la población'. I can fetch the full metadata for any of these if you provide the name.

---

**👤 You:**
> "List all organizations that publish data on the portal."

**🤖 AI Agent:**
> I've retrieved the list of organizations. There are many contributors, including 'Consejería de Salud', 'Ayuntamiento de Murcia', and 'Servicio Murciano de Salud'. Which organization's data are you interested in?


## ❓ FAQ

**Q: How can I find datasets related to a specific topic like 'transport'?**
You can use the `search_datasets` tool. Just provide a query string like 'transporte' and the agent will return all matching packages from the Murcia portal.

**Q: Can I see which public data is currently trending or most popular?**
Yes! Use the `get_most_viewed_datasets` tool to retrieve the ten most visited datasets in the portal, or `get_most_recent_datasets` for the latest additions.

**Q: How do I get the full details and download links for a specific dataset?**
Use the `get_dataset` tool with the dataset's ID or name. It will provide complete metadata, including descriptions of the resources and their access URLs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/region-de-murcia-datos-abiertos](https://vinkius.com/mcp/region-de-murcia-datos-abiertos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Región de Murcia Datos Abiertos** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `region-de-murcia-datos-abiertos` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Región de Murcia Datos Abiertos** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "region-de-murcia-datos-abiertos": {
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
