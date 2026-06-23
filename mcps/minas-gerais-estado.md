# Minas Gerais (Estado) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/minas-gerais-estado)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access the official Open Data Portal of the State of Minas Gerais, Brazil. Query datasets, organizations, and public resources directly.

## Description
Connect to the **Minas Gerais State Open Data Portal** to explore a vast repository of public information. This server allows AI agents to programmatically browse, search, and retrieve metadata from one of Brazil's most comprehensive transparency portals.

### What you can do

- **Dataset Discovery** — List all available packages or search for specific datasets related to health, education, or finance using `list_packages` and `search_packages`.
- **Organizational Insights** — Explore the structure of the state government by listing departments and viewing their specific datasets via `list_organizations` and `get_organization`.
- **Resource Access** — Identify specific files (CSV, PDF, XLS) within datasets and retrieve their metadata using `get_resource` and `search_resources`.
- **Categorized Browsing** — Navigate data through thematic groups (categories) or tags to find exactly what you need with `list_groups` and `list_tags`.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Minas Gerais Portal API Key for higher rate limits
3. Start querying public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find and inspect public datasets for research and reporting
- **Journalists** — automate the discovery of government transparency data and organizational structures
- **Developers** — integrate official state data into applications without manual portal navigation


## Available Tools (10)
- **list_groups**: List all groups (categories)
- **get_group**: Get details and datasets of a group
- **list_organizations**: List all organizations
- **get_organization**: Get details and datasets of an organization
- **list_packages**: List all dataset names in the portal
- **search_packages**: Search for datasets matching specific criteria
- **get_package**: Get full metadata of a specific dataset
- **search_resources**: Search for resources matching a query
- **get_resource**: Get metadata of a specific resource (file)
- **list_tags**: List all tags used in the portal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Minas Gerais (Estado)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets related to 'educação' in the Minas Gerais portal."

**🤖 AI Agent:**
> I found several datasets related to education, including 'Indicadores da Educação Básica' and 'Matrículas na Rede Estadual'. Which one would you like to explore in detail?

---

**👤 You:**
> "List all organizations available in the portal."

**🤖 AI Agent:**
> I've retrieved the list of organizations. There are over 50 entities, including 'Controladoria-Geral do Estado (CGE)' and 'Secretaria de Estado de Fazenda (SEF)'.

---

**👤 You:**
> "Get the metadata for the dataset 'planejamento-e-monitoramento'."

**🤖 AI Agent:**
> The dataset 'Planejamento e Monitoramento' contains 12 resources, including CSV files for budget execution and PDF reports. It is maintained by the SEPLAG organization.


## ❓ FAQ

**Q: How can I find datasets related to a specific topic like 'health'?**
You can use the `search_packages` tool with the query 'saude' or use `get_group` with the ID 'saude' to list all datasets categorized under that theme.

**Q: Can I see the actual download links for the data files?**
Yes. By using `get_package` with a dataset ID, the AI will retrieve the metadata for all associated resources, which typically includes the URL, format (CSV, PDF), and description of each file.

**Q: How do I list all government agencies that publish data on the portal?**
Use the `list_organizations` tool. It will return a list of all government bodies (like CGE, SEF, etc.) that have active datasets in the Minas Gerais portal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/minas-gerais-estado](https://vinkius.com/mcp/minas-gerais-estado)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Minas Gerais (Estado)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `minas-gerais-estado` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Minas Gerais (Estado)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "minas-gerais-estado": {
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
