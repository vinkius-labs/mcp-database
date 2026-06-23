# Gipuzkoa Irekia MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gipuzkoa-irekia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access open data from Gipuzkoa (Spain) — search datasets, explore resources, and query organizations or thematic groups directly from any AI agent.

## Description
Connect to the **Gipuzkoa Irekia** open data portal and empower your AI agent to explore public sector information from the Gipuzkoa region through natural conversation.

### What you can do

- **Dataset Discovery** — Search for specific datasets (packages) using keywords or filter by organization and metadata
- **Resource Inspection** — Access detailed metadata for specific data files (resources), including formats and download links
- **Organizational Browsing** — List and inspect the various public departments and municipalities that publish data
- **Thematic Exploration** — Navigate data through thematic groups such as transport, environment, or economy
- **Advanced Querying** — Perform Solr-like searches to find precise information within the vast public catalog

### How it works

1. Subscribe to this server
2. Enter your Gipuzkoa Irekia API Key (optional for public data, recommended for higher limits)
3. Start querying public datasets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find and inspect public datasets for research and reporting without manual portal navigation
- **Developers** — retrieve resource IDs and metadata directly in the IDE to integrate public APIs into applications
- **Citizens & Researchers** — explore government transparency data and public records through simple natural language questions


## Available Tools (9)
- **list_groups**: List all group names
- **show_group**: Get details for a specific group
- **list_organizations**: List all organization names
- **show_organization**: Get details for a specific organization
- **list_packages**: List all dataset (package) names
- **search_packages**: Search for datasets
- **show_package**: Get metadata for a specific dataset
- **search_resources**: Search for resources
- **show_resource**: Get metadata for a specific resource


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gipuzkoa Irekia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the organizations that publish open data in Gipuzkoa."

**🤖 AI Agent:**
> I've retrieved the list of publishing organizations. There are several entities including 'Diputación Foral de Gipuzkoa', 'Ayuntamiento de Donostia', and various regional agencies. Would you like to see the details for a specific one?

---

**👤 You:**
> "Search for datasets related to 'environment' in the Gipuzkoa Irekia catalog."

**🤖 AI Agent:**
> Searching for 'environment'... I found several datasets, such as 'Air Quality Measurements' and 'Waste Management Statistics'. Which one would you like to explore further?

---

**👤 You:**
> "Show me the metadata for the dataset named 'presupuestos-municipales'."

**🤖 AI Agent:**
> Fetching metadata for 'presupuestos-municipales'... This dataset contains municipal budget information. It includes resources in CSV and XLS formats, last updated recently by the Finance Department. Do you want the specific resource IDs for downloading?


## ❓ FAQ

**Q: How can I search for datasets related to a specific topic like 'transport'?**
You can use the `search_packages` tool. Simply provide the search term in the `q` parameter (e.g., 'transport'), and the agent will return a list of matching datasets from the Gipuzkoa Irekia catalog.

**Q: Can I see which organizations are publishing data on this portal?**
Yes! Use the `list_organizations` tool to get a complete list of all departments, municipalities, and entities that contribute to the Gipuzkoa Irekia open data catalog.

**Q: How do I get the download links or format details for a specific data file?**
Use the `show_resource` tool with the specific Resource ID. It will provide detailed metadata, including the file format (CSV, JSON, etc.) and the direct URL to access the data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gipuzkoa-irekia](https://vinkius.com/mcp/gipuzkoa-irekia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gipuzkoa Irekia** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gipuzkoa-irekia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gipuzkoa Irekia** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gipuzkoa-irekia": {
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
