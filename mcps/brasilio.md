# Brasil.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brasilio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access structured Brazilian public data — query COVID-19 stats, company records, and socio-economic datasets directly from your AI agent.

## Description
Connect to **Brasil.io**, the leading platform for accessible Brazilian public data, and empower your AI agent to analyze real-world datasets through natural conversation.

### What you can do

- **Dataset Discovery** — List all available public datasets hosted on the platform, from health data to judicial salaries.
- **Metadata Inspection** — Fetch detailed schemas and metadata for specific tables to understand available columns and data types.
- **Advanced Querying** — Retrieve actual data records with powerful filtering capabilities (by state, city, date, etc.) using simple JSON filters.
- **Pagination Support** — Navigate through large datasets efficiently using built-in pagination controls.

### How it works

1. Subscribe to this server
2. Enter your Brasil.io API Token
3. Start querying Brazilian public intelligence from Claude, Cursor, or any MCP client

No more manual CSV downloads or wrestling with government transparency portals. Your AI acts as a data scientist specialized in Brazilian public records.

### Who is this for?

- **Data Analysts & Journalists** — quickly extract facts and figures for reports without writing complex scrapers.
- **Researchers** — access historical and current socio-economic data for academic or market studies.
- **Developers** — integrate real Brazilian administrative data into your workflows or applications via your IDE.


## Available Tools (3)
- **list_datasets**: io platform. Supports pagination.

List available datasets on Brasil.io
- **query_table_data**: You can pass arbitrary filters as a JSON string to filter by column names (e.g., {"state": "PR"}).

Query data records from a specific table
- **get_table_metadata**: Get metadata for a specific table in a dataset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brasil.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available datasets on Brasil.io."

**🤖 AI Agent:**
> I've retrieved the available datasets. You can access data on 'covid19', 'salarios-magistrados', 'socios-brasil', and more. Which one would you like to explore?

---

**👤 You:**
> "Show me the metadata for the 'caso' table in the 'covid19' dataset."

**🤖 AI Agent:**
> The 'caso' table in the 'covid19' dataset contains fields such as 'date', 'state', 'city', 'confirmed', 'deaths', and 'is_last'. It tracks daily COVID-19 reports by municipality.

---

**👤 You:**
> "Query the 'caso' table in 'covid19' for the state of 'PR' and city 'Curitiba'."

**🤖 AI Agent:**
> I found the latest records for Curitiba, PR. On 2023-03-20, there were X confirmed cases and Y deaths. Would you like to see previous dates?


## ❓ FAQ

**Q: How can I filter data for a specific state or city?**
Use the `query_table_data` tool and provide a JSON string in the `filters` parameter, such as `{"state": "SP", "city": "São Paulo"}`. The agent will apply these filters to the Brasil.io API request.

**Q: How do I find out what columns are available in a dataset?**
First, use `list_datasets` to find the slug of the dataset. Then, use `get_table_metadata` with the dataset and table slugs to see the full list of available fields and their descriptions.

**Q: Can I navigate through large amounts of data?**
Yes. Both `list_datasets` and `query_table_data` support `page` and `page_size` parameters, allowing you to iterate through results without overloading the response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brasilio](https://vinkius.com/mcp/brasilio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brasil.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `brasilio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brasil.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brasilio": {
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
