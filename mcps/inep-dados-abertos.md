# Inep Dados Abertos MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/inep-dados-abertos)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access official Brazilian educational data from INEP — query Censo Escolar, ENEM, and higher education statistics directly.

## Description
Connect to the **Inep Open Data Portal** (Instituto Nacional de Estudos e Pesquisas Educacionais Anísio Teixeira) and explore the most comprehensive educational datasets in Brazil through natural language.

### What you can do

- **Dataset Discovery** — List and search through hundreds of educational packages including ENEM, IDEB, and Censo Escolar.
- **Deep Data Querying** — Use SQL-like queries to filter and extract specific rows from massive datasets without downloading huge files.
- **Resource Inspection** — Access metadata, download links, and structural information for CSVs, PDFs, and microdata.
- **Organizational Mapping** — Explore data grouped by specific departments and thematic groups within the Brazilian Ministry of Education.
- **Granular Search** — Find specific resources or tags to pinpoint the exact statistical series needed for research or reporting.

### How it works

1. Subscribe to this server
2. (Optional) Provide your Inep API Key if you have specific access requirements, or use public access
3. Start querying Brazilian educational statistics from Claude, Cursor, or any MCP client

### Who is this for?

- **Researchers & Academics** — quickly find specific microdata years and variables for educational studies.
- **Data Journalists** — extract live statistics on exam performance or school infrastructure for reporting.
- **Public Policy Analysts** — monitor educational indicators and IDEB results across different regions of Brazil.


## Available Tools (12)
- **get_group**: Get group details
- **get_organization**: Get organization details
- **get_package**: Get dataset details
- **get_resource**: Get resource details
- **list_groups**: List groups
- **list_organizations**: g., different departments within Inep).

List organizations
- **list_packages**: List all dataset (package) names
- **list_tags**: List tags
- **search_datastore_sql**: Query data using SQL (DataStore)
- **search_datastore**: Search data within a resource (DataStore)
- **search_packages**: Search datasets
- **search_resources**: Search resources


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Inep Dados Abertos** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all available datasets related to 'Censo Escolar'."

**🤖 AI Agent:**
> I found several datasets for 'Censo Escolar', including annual microdata from 2010 to 2023. Would you like to see the details for the most recent one?

---

**👤 You:**
> "List the resources and download URLs for the 'ENEM 2022' package."

**🤖 AI Agent:**
> The 'ENEM 2022' dataset contains 4 resources, including the main microdata CSV and the documentation PDF. Here are the direct download links...

---

**👤 You:**
> "Run a SQL query to get the first 10 records from resource 'd9e8f7a6-...' where the state is 'SP'."

**🤖 AI Agent:**
> Querying the DataStore... I've retrieved 10 records for the state of São Paulo. The data includes school codes, names, and administrative categories.


## ❓ FAQ

**Q: Can I query specific data inside a resource without downloading the whole file?**
Yes! You can use the `search_datastore_sql` tool to run SQL queries directly against the Inep database for resources that support the DataStore API.

**Q: How do I find datasets related to a specific topic like 'ENEM'?**
Use the `search_packages` tool with the query 'ENEM'. It will return all matching datasets, which you can then inspect using `get_package`.

**Q: Is it possible to list all organizations that publish data on the portal?**
Yes, the `list_organizations` tool retrieves all departments and entities within Inep that maintain open data resources.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inep-dados-abertos](https://vinkius.com/mcp/inep-dados-abertos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Inep Dados Abertos** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `inep-dados-abertos` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Inep Dados Abertos** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "inep-dados-abertos": {
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
