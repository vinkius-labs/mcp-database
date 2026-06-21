# STF Dados Abertos MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stf-dados-abertos)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access open data from the Brazilian Supreme Federal Court (STF) — explore datasets, resources, and institutional organizations via AI.

## Description
Connect your AI agent to the **STF Dados Abertos** portal and explore the transparency data of the Brazilian Supreme Federal Court through natural language.

### What you can do

- **Dataset Discovery** — List all available datasets (packages) and search for specific legal or administrative topics using keywords.
- **Resource Inspection** — Fetch detailed metadata for specific files, data links, and resources within a dataset to understand their structure.
- **DataStore Querying** — Perform SQL-like queries directly on DataStore-enabled resources to extract specific information without downloading large files.
- **Institutional Browsing** — Explore the organizations and groups that categorize and maintain the court's open data.
- **Metadata Analysis** — Access comprehensive metadata for packages, organizations, and groups to understand data provenance and update frequency.

### How it works

1. Subscribe to this server
2. (Optional) Enter your STF API Key for higher access limits
3. Start querying Brazilian judicial data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Researchers** — quickly find and analyze court datasets without manual portal navigation
- **Data Journalists** — automate the discovery of transparency data and resource updates for reporting
- **Developers & Analysts** — integrate official STF data into applications using structured metadata and DataStore queries


## Available Tools
- **get_group**: Get group details
- **get_organization**: Get organization details
- **get_package**: Get dataset details
- **get_resource**: Get resource details
- **list_groups**: List groups
- **list_organizations**: List organizations
- **list_packages**: List all datasets (packages) in STF Dados Abertos
- **search_datastore**: Query DataStore
- **search_packages**: Search datasets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **STF Dados Abertos** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available datasets in the STF Dados Abertos portal."

**🤖 AI Agent:**
> I've retrieved the list of datasets. Notable packages include 'Processos Eletrônicos', 'Gastos com Pessoal', and 'Decisões'. Which one would you like to explore further?

---

**👤 You:**
> "Search for datasets related to 'votações'."

**🤖 AI Agent:**
> Searching... I found 3 datasets matching 'votações'. The most relevant is 'Votações em Plenário'. Would you like to see the available resources for this package?

---

**👤 You:**
> "Get the details and resources for the dataset 'folha-de-pagamento'."

**🤖 AI Agent:**
> Fetching details for 'folha-de-pagamento'... This dataset contains 12 resources (CSV and JSON formats) and is maintained by the 'Secretaria de Gestão Estratégica'. Do you want to inspect a specific resource ID?


## ❓ FAQ

**Q: Can I perform SQL-like queries on the court's data files?**
Yes! If a resource is integrated into the DataStore, you can use the `search_datastore` tool with the Resource ID to query the data within the file directly.

**Q: How do I find datasets related to a specific legal topic?**
Use the `search_packages` tool. Simply provide a search term (e.g., 'processos' or 'votação') and the agent will return all matching datasets from the portal.

**Q: Is it possible to list all organizations that publish data on the STF portal?**
Absolutely. Use the `list_organizations` tool to see all departments and entities, or `get_organization` to see details and datasets owned by a specific one.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stf-dados-abertos](https://vinkius.com/mcp/stf-dados-abertos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **STF Dados Abertos** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `stf-dados-abertos` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **STF Dados Abertos** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stf-dados-abertos": {
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
