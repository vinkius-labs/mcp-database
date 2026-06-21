# NCREIF Custom Query MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ncreif-custom-query)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Institutional real estate data — execute custom SQL-like queries on NPI and other indices via NCREIF.

## Description
Empower your AI agents with institutional real estate intelligence. This server provides programmatic access to the **NCREIF Query Tool API**, allowing for deep analysis of the NCREIF Property Index (NPI), Fund Index (ODCE), and specialized timberland/farmland data.

### What you can do

- **Custom Analytics** — Execute SQL-like queries to calculate income returns, appreciation, and total returns
- **Index Monitoring** — Access historical and real-time performance data for major US real estate indices
- **Predefined KPIs** — Quickly retrieve key metrics like Cap Rates and Occupancy percentages
- **Granular Filtering** — Filter by property type, region, CBSA, and more using powerful where clauses

### How it works

1. Subscribe to this server
2. Enter your **NCREIF Username** and **Password** (Member/Subscriber credentials)
3. Start querying institutional data directly from Claude, Cursor, or any MCP client


## Available Tools
- **execute_query**: Execute a custom NCREIF query
- **get_historical_npi**: Get historical NPI returns
- **get_predefined_kpi**: Get predefined KPI data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NCREIF Custom Query** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show NPI total returns for the last 4 quarters."

**🤖 AI Agent:**
> Executing NPI query... The total return for Q4 2025 was 1.2%, following 0.8% in Q3. Here is the historical breakdown...


## ❓ FAQ

**Q: Who can access this API?**
Access is limited to NCREIF Data Contributor Members and paid Data Subscribers. You must use your website login credentials.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ncreif-custom-query](https://vinkius.com/mcp/ncreif-custom-query)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NCREIF Custom Query** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ncreif-custom-query` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NCREIF Custom Query** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ncreif-custom-query": {
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
