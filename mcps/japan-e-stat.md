# Japan e-Stat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/japan-e-stat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Query official Japanese government statistics — population, GDP, industry, trade, employment, and more — from the e-Stat national database.

## Description
The **Japan e-Stat MCP Server** connects your AI agent to the official Portal of Government Statistics of Japan — the most comprehensive public data repository for the world's third-largest economy.

### Core Capabilities

- **Table Search** — Discover statistical tables across all Japanese government ministries by keyword. Covers census data, national accounts, industrial production, foreign trade, labor force surveys, and more.
- **Data Retrieval** — Pull raw numerical data from any table, fully classified by category, geographic area, and time period.
- **English Support** — The API supports `lang=E` for English-translated table names and categories where available.

Free API key required (instant registration at e-stat.go.jp). Japan publishes some of the most detailed and reliable economic statistics in the world, making this an essential resource for global macro analysis, trade research, and market intelligence.


## Available Tools
- **get_japan_stats_data**: Use search_japan_statistics first to find the correct table ID. Returns category-classified data with time periods, areas, and values.

Retrieve statistical data from a specific Japanese Government e-Stat table
- **search_japan_statistics**: Returns table IDs, organization names, titles, and survey dates. Use the returned table ID with get_japan_stats_data to retrieve actual numbers. Keywords work in both English and Japanese. Common topics: population, GDP, industry, trade, employment, tourism, education, health.

Search for statistical tables in the Japanese Government e-Stat database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Japan e-Stat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find Japanese population statistics by prefecture."

**🤖 AI Agent:**
> I've searched e-Stat for population data by prefecture. Found 15 relevant tables from the Statistics Bureau. The most recent census table (ID: 0003448237) shows Tokyo at 14.0 million, Kanagawa at 9.2 million, and Osaka at 8.8 million. Japan's total population stands at approximately 125.5 million.

---

**👤 You:**
> "Fetch the latest Consumer Price Index (CPI) data for Tokyo."

**🤖 AI Agent:**
> I retrieved the latest CPI data for the Ku-area of Tokyo. The all-items index currently stands at 106.5 (2020=100), representing a 2.4% year-over-year increase, driven primarily by rising food and energy costs.

---

**👤 You:**
> "Show me the industrial production index for the automotive sector."

**🤖 AI Agent:**
> According to the latest METI data from e-Stat, the Indices of Industrial Production (IIP) for the motor vehicles, parts, and accessories sector rests at 98.2, showing a slight month-over-month decrease of 1.1%.


## ❓ FAQ

**Q: How do I get an e-Stat API key?**
Register for a free account at e-stat.go.jp, then visit your My Page to generate an Application ID (appId). Approval is instant.

**Q: Is the data available in English?**
Many tables support English translations for table titles and category names. The API uses lang=E by default. Some specialized datasets may only be available in Japanese.

**Q: What types of statistics are covered?**
The database covers national census data, labor force surveys, consumer price indices (CPI), trade statistics, industrial production, health, and education metrics published by all Japanese government ministries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/japan-e-stat](https://vinkius.com/mcp/japan-e-stat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Japan e-Stat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `japan-e-stat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Japan e-Stat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "japan-e-stat": {
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
