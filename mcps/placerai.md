# Placer.ai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/placerai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Access foot traffic analytics — track visit trends, demographics, and trade areas directly from any AI agent.

## Description
Connect your AI agents to **Placer.ai**, the leading location intelligence platform. This MCP provides 10 tools to retrieve accurate foot traffic analytics, visitor demographics, and market rankings for millions of locations.

### What you can do

- **Visitation Metrics** — Retrieve estimated visits and trends for specific venues and brands with historical context
- **Demographic Profiles** — Understand visitor characteristics, including population estimates and trade area data
- **Competitive Benchmarking** — Access location rankings to compare performance against industry peers and category leaders
- **Trade Area Analysis** — Identify the True Trade Area (TTA) polygon for any point of interest to see where visitors come from

### How it works

1. Subscribe to this server
2. Request API access at [**placer.ai/placer-api**](https://www.placer.ai/placer-api)
3. Obtain your **API Key** from the Placer.ai developer portal
4. Identify the **POI IDs** for the locations you want to track
5. Connect your account to Vurb to start orchestrating location intelligence.

### Who is this for?

- **Retailers & Real Estate** — analyze store performance and identify expansion opportunities based on movement data
- **Market Researchers** — track physical consumer behavior and visitation trends at scale
- **Data Analysts** — integrate real-world traffic metrics into financial and operational models


## Available Tools (10)
- **get_same_store_visits**: Retrieve same-store foot traffic metrics
- **get_api_status**: Check Placer.ai API operational status
- **get_trade_area**: Get True Trade Area (TTA) coordinates
- **get_demographics**: Get visitor demographics estimates
- **get_poi_details**: Get complete details for a specific POI
- **get_rankings**: Get location performance rankings
- **get_trends**: Get visit trends over time
- **get_visits**: Retrieve foot traffic visit counts
- **list_properties**: ai account.

List properties associated with your account
- **search_poi**: Search for specific locations or brands


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Placer.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the foot traffic trends for POI ID 'poi_123' for the last month."

**🤖 AI Agent:**
> Retrieving location metrics... I've found the trends for 'Central Mall' (ID: poi_123). Visits are up 15% compared to last month, with the highest traffic occurring on Saturdays between 2 PM and 6 PM. Would you like a breakdown by day?

---

**👤 You:**
> "Search Placer.ai for 'Walmart' locations in Miami and show their IDs."

**🤖 AI Agent:**
> Searching the Placer.ai database... I found 3 Walmart locations in Miami: 1. Walmart Supercenter (ID: w_1), 2. Walmart Neighborhood Market (ID: w_2)... Which one would you like to analyze?

---

**👤 You:**
> "What is the demographic profile for the visitors of POI 'poi_abc'?"

**🤖 AI Agent:**
> Fetching population estimates for 'Oak Plaza' (ID: poi_abc)... The visitor base is primarily aged 25-44 (42%), with a median household income of $75,000. Most visitors reside within a 5-mile radius.


## ❓ FAQ

**Q: Can my AI automatically find the visit trends for a specific location just by its ID?**
Yes! Use the `get_trends` tool with the POI ID. Your agent will return day-over-day or week-over-week visit changes for that specific location.

**Q: How do I identify the POI ID for a specific store or venue?**
Use the `search_poi` tool with keywords like the brand name or address. Your agent will return a list of matching locations along with their unique Placer.ai POI IDs.

**Q: Does it support trade area analysis?**
Yes! The `get_trade_area` tool retrieves the True Trade Area (TTA) for any POI, providing the geographic boundaries of where the majority of visitors originate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/placerai](https://vinkius.com/mcp/placerai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Placer.ai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `placerai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Placer.ai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "placerai": {
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
