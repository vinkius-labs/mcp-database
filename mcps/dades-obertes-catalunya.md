# Dades Obertes Catalunya MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dades-obertes-catalunya)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access Catalonia's Open Data portal — search catalogs and query datasets using SoQL to extract public information directly.

## Description
Unlock the power of **Dades Obertes Catalunya**, the official open data platform of the Government of Catalonia. This MCP server allows your AI agent to browse thousands of public datasets and perform complex queries through natural conversation.

### What you can do

- **Catalog Discovery** — Search for datasets by keywords, categories, or tags to find relevant public information using the `search_catalog` tool.
- **Advanced Querying** — Use SoQL (Socrata Query Language) via `query_dataset` to filter, select specific columns, and sort data from any dataset using its 4x4 identifier.
- **Data Analysis** — Group results and perform full-text searches across entire datasets to extract insights on health, transport, economy, and more.
- **Pagination & Limits** — Efficiently handle large datasets with built-in support for limits and offsets to browse records systematically.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Socrata App Token for higher rate limits
3. Start querying Catalan public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly pull public statistics into your workflow without manual CSV downloads
- **Researchers** — find and cross-reference government data on demographics, environment, or urban planning
- **Developers** — test data queries and explore API structures directly through natural language


## Available Tools (2)
- **query_dataset**: g., abcd-1234). Supports SoQL parameters like $select, $where, $limit.

Query a specific dataset using SoQL parameters
- **search_catalog**: Returns dataset identifiers needed for the query_dataset tool.

Search the Dades Obertes Catalunya catalog for datasets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dades Obertes Catalunya** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the catalog for datasets related to 'hospitals' in Catalonia."

**🤖 AI Agent:**
> I found several datasets. The most relevant is 'Centres sanitaris de Catalunya' with ID `8u93-v9az`. Would you like me to query its first few records?

---

**👤 You:**
> "Query dataset 'abcd-1234' and show me the top 5 results where population is over 10000."

**🤖 AI Agent:**
> Using `query_dataset` with `$where: "population > 10000"` and `$limit: 5`... Here are the results: 1. Barcelona (1.6M), 2. L'Hospitalet (264k), 3. Terrassa (223k)...

---

**👤 You:**
> "List the columns available in dataset 'xyz1-2345' using a full-text search for 'electric'."

**🤖 AI Agent:**
> I've queried `xyz1-2345` with `$q: "electric"`. I found records related to electric vehicle charging stations, including columns for 'location', 'power_kw', and 'status'.


## ❓ FAQ

**Q: How do I find the unique identifier for a specific dataset?**
Use the `search_catalog` tool with a descriptive query. The response will include the 4x4 alphanumeric ID (e.g., 'abcd-1234') which you can then use with the `query_dataset` tool.

**Q: Can I filter data by specific values like a city or a date range?**
Yes! When using `query_dataset`, use the `$where` parameter to apply SoQL filters. For example, `$where: "poblacio > 5000"` or `$where: "comarca = 'Barcelonès'"`.

**Q: Is a Socrata App Token mandatory to use this server?**
No, it is optional. However, providing a `DADES_APP_TOKEN` allows for higher rate limits and prevents throttling during intensive data exploration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dades-obertes-catalunya](https://vinkius.com/mcp/dades-obertes-catalunya)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dades Obertes Catalunya** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dades-obertes-catalunya` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dades Obertes Catalunya** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dades-obertes-catalunya": {
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
