# Junta de Andalucía (Portal) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/junta-de-andalucia-portal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the official Open Data Portal of the Junta de Andalucía. Explore datasets, resources, and public records directly from your AI agent.

## Description
Connect to the **Junta de Andalucía Open Data Portal** to query and analyze public information from the Andalusian government through natural language.

### What you can do

- **Dataset Discovery** — List all available packages and datasets published in the portal to find relevant public information.
- **Metadata Inspection** — Retrieve detailed metadata for specific datasets and resources, including descriptions, formats, and update frequencies.
- **Deep Data Search** — Use the Datastore search capabilities to query content within specific resources using full-text search and filters.
- **Organizational Mapping** — List all publishing organizations and groups (categories) to understand the structure of public data in the region.
- **Resource Analysis** — Inspect individual files (resources) within datasets to get direct access links and technical specifications.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Portal API Key for higher rate limits
3. Start querying Andalusian public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts & Researchers** — quickly find and inspect public datasets for socio-economic or environmental studies.
- **Developers** — retrieve resource IDs and metadata to integrate public data into applications without manual browsing.
- **Citizens & Journalists** — explore government transparency records and public statistics through simple conversation.


## Available Tools (6)
- **search_datastore**: Search for data within a specific resource
- **list_organizations**: List all publishing organizations
- **get_package**: Get metadata for a specific dataset
- **list_packages**: List all dataset names in the portal
- **get_resource**: Get metadata for a specific resource (file)
- **list_groups**: List all groups (categories)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Junta de Andalucía (Portal)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available datasets in the Junta de Andalucía portal."

**🤖 AI Agent:**
> I've retrieved the list of datasets. There are numerous packages available, including 'Presupuestos de la Comunidad', 'Centros Educativos', and 'Calidad del Aire'. Which category or specific dataset would you like to explore?

---

**👤 You:**
> "Search for 'turismo' in the resource with ID 550e8400-e29b-41d4-a716-446655440000."

**🤖 AI Agent:**
> Searching the datastore... I found 12 entries matching 'turismo' in that resource. The results include data on hotel occupancy and local attractions. Would you like me to summarize the top results?

---

**👤 You:**
> "Show me the metadata for the dataset 'centros-sanitarios'."

**🤖 AI Agent:**
> Fetching metadata for 'centros-sanitarios'... This dataset contains information about all health centers in Andalusia, updated monthly. It includes 3 resources in CSV and JSON formats. Would you like the IDs of these resources?


## ❓ FAQ

**Q: How can I search for specific information inside a dataset's file?**
Use the `search_datastore` tool with the specific `resource_id`. You can provide a query string `q` to filter the rows and find exactly what you need within the data table.

**Q: Can I see which government department published a specific dataset?**
Yes. You can use `list_organizations` to see all publishers or use `get_package` with the dataset ID to see the specific organization responsible for that data.

**Q: Is an API key mandatory to use this server?**
No, the API key is optional. Most data on the Junta de Andalucía portal is public. However, providing a key via the `JUNTA_API_KEY` credential may help avoid rate limits during intensive usage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/junta-de-andalucia-portal](https://vinkius.com/mcp/junta-de-andalucia-portal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Junta de Andalucía (Portal)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `junta-de-andalucia-portal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Junta de Andalucía (Portal)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "junta-de-andalucia-portal": {
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
