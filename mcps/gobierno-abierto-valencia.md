# Gobierno Abierto Valencia MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gobierno-abierto-valencia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access Valencia's Open Data portal to query datasets, resources, and public records directly from your AI agent.

## Description
Connect to the **Valencia Open Data portal (Gobierno Abierto)** to explore public datasets, groups, and specific resource data through natural conversation.

### What you can do

- **Datasets & Packages** — List all available public datasets and fetch detailed metadata for specific ones using their name or ID.
- **Resource Inspection** — Access specific file metadata, formats, and descriptions within a dataset to understand the available data structures.
- **Data Search** — Query actual records inside a resource's datastore with powerful filtering, search queries, and pagination.
- **Categories & Groups** — Browse datasets by organizational groups or thematic categories to find relevant information faster.

### How it works

1. Subscribe to this server
2. Enter your Valencia Open Data API Key (if required for specific datasets)
3. Start querying public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find and inspect public datasets without manual browsing
- **Developers** — integrate real-time city data into applications by testing queries via AI
- **Citizens & Researchers** — explore municipal transparency data and public records through simple questions


## Available Tools
- **search_datastore**: Search for data within a specific resource
- **list_groups**: List dataset groups (categories)
- **show_package**: Get metadata for a specific dataset
- **list_packages**: List all dataset names
- **show_resource**: Get metadata for a specific resource


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gobierno Abierto Valencia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available datasets in the Valencia portal."

**🤖 AI Agent:**
> I've retrieved the list of datasets. There are several available, including 'Tráfico', 'EMT Valencia', and 'Presupuestos Municipales'. Which one would you like to explore?

---

**👤 You:**
> "Search for 'bicis' records in resource ID 456."

**🤖 AI Agent:**
> Searching the datastore... I found 10 records matching 'bicis'. These include real-time station availability and location data. Would you like to see the specific coordinates?

---

**👤 You:**
> "Show me the details for the dataset 'EMT Valencia'."

**🤖 AI Agent:**
> Fetching metadata for 'EMT Valencia'... This dataset contains real-time bus information, routes, and schedules. It includes 5 resources (CSV, JSON, and GeoJSON formats).


## ❓ FAQ

**Q: How do I search for specific records within a data file?**
Use the `search_datastore` tool with the specific Resource ID. You can provide a search string `q` to filter the records and use `limit` or `offset` for pagination.

**Q: How can I see the metadata for a specific dataset?**
Simply use the `show_package` tool and provide the name or ID of the dataset. The agent will return full metadata including descriptions, maintainers, and associated resources.

**Q: Can I list all the data categories available in the portal?**
Yes! The `list_groups` tool returns all dataset groups or categories available in the Valencia Open Data portal, helping you browse by topic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gobierno-abierto-valencia](https://vinkius.com/mcp/gobierno-abierto-valencia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gobierno Abierto Valencia** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gobierno-abierto-valencia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gobierno Abierto Valencia** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gobierno-abierto-valencia": {
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
