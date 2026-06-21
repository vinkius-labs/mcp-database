# Acre Dados Abertos MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/acre-dados-abertos)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access open data from the State of Acre, Brazil — explore datasets, organizations, and thematic groups directly from your AI agent.

## Description
Connect to the **Acre Dados Abertos** portal to query public information from the State of Acre. This server allows AI agents to browse, search, and analyze government datasets, organizational structures, and thematic groups.

### What you can do

- **Dataset Discovery** — List and search for specific packages (datasets) like municipal GDP, environmental data, or demographic statistics.
- **Metadata Inspection** — Fetch detailed metadata for packages and individual resources (files) to understand data provenance and formats.
- **Thematic Exploration** — Browse data organized by thematic groups (e.g., economy, health, education) or by the specific government organizations that publish them.
- **Deep Data Querying** — Search and filter records directly within tabular resources (Datastore) like CSV files without downloading the entire dataset.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Acre API Key if you have one for higher rate limits
3. Start querying public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find and sample public datasets for research and reporting
- **Journalists** — verify government figures and find public records through natural language
- **Developers** — integrate real-time public data into applications using the Datastore search capabilities


## Available Tools
- **get_group**: Get details for a specific group
- **get_package**: Get detailed metadata for a specific dataset (package)
- **get_resource**: Get metadata for a specific resource
- **list_groups**: List all thematic groups
- **list_organizations**: List all organizations
- **list_packages**: List all dataset (package) names
- **search_datastore**: Search and filter records within a tabular resource (Datastore)
- **search_packages**: Search for datasets (packages)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Acre Dados Abertos** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets related to 'economia' in Acre."

**🤖 AI Agent:**
> I found several datasets. The most relevant are 'PIB Municipal' and 'Arrecadação Estadual'. Would you like to see the detailed metadata for 'PIB Municipal'?

---

**👤 You:**
> "List all thematic groups available in the Acre Open Data portal."

**🤖 AI Agent:**
> There are several thematic groups, including 'Saúde', 'Educação', 'Economia', and 'Segurança Pública'. Which group would you like to explore for specific datasets?

---

**👤 You:**
> "Query the datastore for resource ID 8f3e... filtering by municipio 'Rio Branco'."

**🤖 AI Agent:**
> I've retrieved the records from the datastore for Rio Branco. The data includes columns like 'ano', 'valor', and 'descricao'. Would you like me to summarize the results?


## ❓ FAQ

**Q: How can I search for datasets related to a specific topic like 'health'?**
Use the `search_packages` tool with the query 'saude'. The agent will return a list of datasets matching that theme from the Acre portal.

**Q: Can I filter data inside a CSV file without downloading it?**
Yes! If the resource is in the Datastore, use the `search_datastore` tool with the Resource ID. You can apply filters like `{"municipio": "Rio Branco"}` to get specific rows.

**Q: How do I find which government departments are publishing data?**
Use the `list_organizations` tool to see all contributing entities, or `list_groups` to see thematic categorizations like 'Environment' or 'Economy'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/acre-dados-abertos](https://vinkius.com/mcp/acre-dados-abertos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Acre Dados Abertos** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `acre-dados-abertos` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Acre Dados Abertos** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "acre-dados-abertos": {
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
