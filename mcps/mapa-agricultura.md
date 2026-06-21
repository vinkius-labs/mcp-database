# MAPA (Agricultura) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mapa-agricultura)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access official Brazilian agricultural open data — search datasets, inspect rural resources, and query Ministry of Agriculture (MAPA) records.

## Description
Connect your AI agent to the **Brazilian Ministry of Agriculture and Livestock (MAPA)** Open Data Portal. This server provides direct access to thousands of public datasets, enabling deep analysis of the Brazilian agribusiness sector.

### What you can do

- **Dataset Discovery** — List all available packages and search for specific topics like 'Agrofit', 'Rural Credit', or 'Livestock'
- **Metadata Inspection** — Fetch complete metadata for specific datasets to understand data provenance, update frequency, and coverage
- **Resource Access** — Retrieve direct download URLs and file formats for specific data resources (CSV, PDF, XLS)
- **Organizational Mapping** — List and inspect the various departments and organizations responsible for publishing agricultural data
- **Categorization** — Browse data by groups and tags to discover related information across different agricultural domains

### How it works

1. Subscribe to this server
2. (Optional) Enter your MAPA/CKAN API Key for higher rate limits
3. Start querying official Brazilian agricultural data from your MCP-compatible client

### Who is this for?

- **Data Scientists & Researchers** — quickly find and access official agricultural statistics for modeling and analysis
- **Agribusiness Analysts** — monitor regulatory data, pesticide registrations, and rural financing trends
- **Policy Makers** — retrieve official government records to support decision-making and reporting


## Available Tools
- **get_organization**: Get details for a specific organization
- **get_package**: Get metadata for a specific dataset (package)
- **get_resource**: Get metadata for a specific resource
- **list_groups**: List all groups
- **list_organizations**: List all organizations
- **list_packages**: List all dataset names (packages)
- **search_packages**: g., "agrofit" or "organization:mapa").

Search for datasets matching a query
- **list_tags**: List all tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MAPA (Agricultura)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets related to 'Agrofit' in the MAPA portal."

**🤖 AI Agent:**
> I found several datasets related to Agrofit. The main one is 'agrofit-sistema-de-agrotoxicos-fitossanitarios' (ID: 120593). Would you like to see the metadata or the available resources for this package?

---

**👤 You:**
> "List all organizations responsible for agricultural data."

**🤖 AI Agent:**
> I've retrieved the list of organizations. There are 12 entities, including 'Secretaria de Defesa Agropecuária (SDA)' and 'Secretaria de Política Agrícola (SPA)'. Which one would you like to explore?

---

**👤 You:**
> "Get the metadata for the dataset 'registro-de-agrotoxicos'."

**🤖 AI Agent:**
> Fetching metadata for 'registro-de-agrotoxicos'... This dataset is maintained by SDA and was last updated on 2023-10-15. It contains 3 resources (CSV, PDF, and XLS). Should I provide the download links?


## ❓ FAQ

**Q: How can I find datasets about a specific topic like 'coffee'?**
You can use the `search_packages` tool with the query 'café'. It will return all datasets that match the term in their title or description.

**Q: How do I get the actual download link for a data file?**
First, use `get_package` to find the resource IDs within a dataset. Then, call `get_resource` with the specific ID to retrieve the download URL and file format.

**Q: Can I see which government departments publish the data?**
Yes! Use the `list_organizations` tool to see all publishing entities. You can then use `get_organization` to see all datasets managed by a specific department.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mapa-agricultura](https://vinkius.com/mcp/mapa-agricultura)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MAPA (Agricultura)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mapa-agricultura` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MAPA (Agricultura)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mapa-agricultura": {
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
