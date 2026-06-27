# USITC DataWeb (International Trade Commission) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/usitc-dataweb-international-trade-commission)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access US international trade statistics directly. Query imports, exports, and trade balances using HS, SITC, or NAICS classifications.

## Description
Connect to the **USITC DataWeb** to retrieve official US international trade data. This server allows AI agents to perform complex queries on trade statistics, including imports, exports, and trade balances across various classification systems like HS, SITC, and NAICS.

### What you can do

- **Trade Data Queries** — Fetch detailed statistics by commodity, country, and time period using the `query_trade_data` tool.
- **Metadata Exploration** — List available data tables, fields, and valid values (like country codes or commodity levels) to build precise queries.
- **Classification Support** — Work with Harmonized Tariff Schedule (HS), SITC, or NAICS codes at various digit levels.
- **Time-Series Analysis** — Retrieve annual or monthly data to analyze trade trends over time.

### How it works

1. Subscribe to this server
2. Enter your USITC DataWeb API Key
3. Start analyzing global trade patterns from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Economists & Analysts** — instantly retrieve trade volumes and values for specific sectors without manual CSV downloads.
- **Supply Chain Managers** — monitor international trade flows and commodity trends directly from your workspace.
- **Policy Researchers** — audit trade balances and historical data using official government sources.


## Available Tools (4)
- **list_metadata_values**: g., a list of all valid country codes).

List valid values for a specific field within a table
- **list_metadata_fields**: List fields available for a specific table
- **query_trade_data**: Uses POST to support large filter sets.

Query USITC trade statistics
- **list_metadata_tables**: List available data tables


## 💬 Prompt Examples

Here are some examples of how you can interact with the **USITC DataWeb (International Trade Commission)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available metadata tables from USITC DataWeb."

**🤖 AI Agent:**
> I've retrieved the available tables. You can query data from tables such as 'imports', 'exports', and 'balance'. Which one would you like to explore?

---

**👤 You:**
> "Show me the fields available for the 'imports' table."

**🤖 AI Agent:**
> For the 'imports' table, you can use fields such as 'commodity', 'country', 'year', 'month', and 'customs_value'. Would you like to see valid values for any of these?

---

**👤 You:**
> "Query trade data for HS code '01' from Canada (1220) for the year 2022."

**🤖 AI Agent:**
> I've processed the query for HS code '01' (Live Animals) from Canada in 2022. The total import value was $X million. Would you like a breakdown by month?


## ❓ FAQ

**Q: How do I find the correct country code for a trade query?**
You can use the `list_metadata_values` tool. Provide the table ID (e.g., 'imports') and the field ID for countries to see a full list of valid USITC country codes.

**Q: What classification systems are supported for commodity queries?**
The server supports 'hs' (Harmonized System), 'sitc' (Standard International Trade Classification), and 'naics' (North American Industry Classification System) via the `query_trade_data` tool.

**Q: Can I see what data tables are available before querying?**
Yes, use the `list_metadata_tables` tool to retrieve a list of all available data tables and their identifiers from the USITC DataWeb API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usitc-dataweb-international-trade-commission](https://vinkius.com/mcp/usitc-dataweb-international-trade-commission)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **USITC DataWeb (International Trade Commission)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `usitc-dataweb-international-trade-commission` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **USITC DataWeb (International Trade Commission)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "usitc-dataweb-international-trade-commission": {
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
