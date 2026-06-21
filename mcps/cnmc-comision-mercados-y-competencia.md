# CNMC (Comisión Mercados y Competencia) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cnmc-comision-mercados-y-competencia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access Spanish market and competition data — search datasets and retrieve records from the CNMC open data portal.

## Description
Connect to the official Open Data portal of the **CNMC (Comisión Nacional de los Mercados y la Competencia)**. This server allows AI agents to explore and extract public data regarding telecommunications, energy, transport, and postal sectors in Spain.

### What you can do

- **Catalog Discovery** — Use `package_search` to find datasets, resources, and metadata using keywords or specific queries.
- **Data Extraction** — Use `datastore_search` to pull actual records and rows from specific resources using their unique IDs.
- **Granular Filtering** — Apply JSON filters to narrow down results to specific dates, regions, or categories within a dataset.
- **Resource Inspection** — Identify update frequencies, license types, and resource formats before processing data.

### How it works

1. Subscribe to this server
2. Enter your CNMC API Key (if required for higher rate limits)
3. Start querying Spanish market data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly fetch market statistics without manual CSV downloads
- **Legal & Compliance Teams** — monitor regulatory data and competition records
- **Policy Researchers** — access public sector information for economic modeling and reporting


## Available Tools
- **datastore_search**: g., a CSV file within a dataset). Requires a resource_id obtained via package_search.

Retrieve actual records from a specific CNMC resource
- **package_search**: Use this to find the resource_id needed for datastore_search.

Search for datasets and resources in the CNMC catalog


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CNMC (Comisión Mercados y Competencia)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets related to 'energía eléctrica' in the CNMC catalog."

**🤖 AI Agent:**
> I found several datasets. The most relevant one is 'Estadística mensual de energía eléctrica' with resource ID 'e123-abc'. Would you like me to fetch the latest records from it?

---

**👤 You:**
> "Get the first 5 records from the CNMC resource '06935639-5561-4608-9580-59367208479e'."

**🤖 AI Agent:**
> I've retrieved the first 5 records for that resource. They include data on market shares for telecommunications operators in Q1 2023. [Data table displayed...]

---

**👤 You:**
> "Search for 'gas natural' datasets and filter the results for the year 2022."

**🤖 AI Agent:**
> I've identified the 'Consumo de gas natural' dataset. Applying the filter for 2022... I found 12 monthly records. Would you like a summary of the total consumption?


## ❓ FAQ

**Q: How do I find the resource_id needed for data retrieval?**
Use the `package_search` tool with a query related to your topic. The response will include a list of resources, each with a unique `id` (the resource_id) that you can then use in `datastore_search`.

**Q: Can I limit the number of records returned to avoid large payloads?**
Yes! The `datastore_search` tool includes an optional `limit` parameter. You can specify exactly how many rows you want to retrieve (e.g., 10 or 100) to keep the response concise.

**Q: Is it possible to filter data by a specific field, like a year or a city?**
Absolutely. Use the `filters` parameter in `datastore_search`. It accepts a JSON string (e.g., `{"Year": "2023"}`) to return only the records that match your criteria.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cnmc-comision-mercados-y-competencia](https://vinkius.com/mcp/cnmc-comision-mercados-y-competencia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CNMC (Comisión Mercados y Competencia)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cnmc-comision-mercados-y-competencia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CNMC (Comisión Mercados y Competencia)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cnmc-comision-mercados-y-competencia": {
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
