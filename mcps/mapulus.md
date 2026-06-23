# Mapulus MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mapulus)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Mapulus Location Intelligence for Australia — access boundaries, demographics, and spatial analytics.

## Description
Connect your **Mapulus** account to any AI agent and access deep Australian location intelligence through natural conversation.

### What you can do

- **Statistical Boundaries** — Search and list suburbs, postcodes, LGAs, and other Australian geographies
- **Demographic Data** — Retrieve ABS Census-derived insights on population, income, and housing
- **Spatial Analytics** — Generate isochrones (catchment areas) and query H3 hexagonal indices
- **Location Enrichment** — Enrich any lat/lon coordinate with detailed geographic and statistical context

### How it works

1. Subscribe to this server
2. Enter your Mapulus API Key
3. Start querying Australian geographic data from Claude, Cursor, or any MCP-compatible client


## Available Tools (9)
- **enrich_location**: Enrich a location with geographic context
- **get_boundary_details**: g., "poa:2000").

Get details for a specific boundary
- **get_demographics**: Get demographics for a boundary
- **get_h3_index**: Get H3 index for a location
- **get_isochrone**: Generate travel-time boundaries
- **get_postcode_data**: Get data for a specific postcode
- **list_data_topics**: List available data topics
- **search_boundaries**: Search for Australian statistical boundaries
- **search_suburbs**: Search specifically for Australian suburbs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mapulus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for boundaries matching 'Sydney'."

**🤖 AI Agent:**
> Fetching boundaries... I found several results including 'Sydney (LGA)', 'Sydney (Suburb)', and 'Sydney (Postcode)'.

---

**👤 You:**
> "Get demographics for postcode 2000."

**🤖 AI Agent:**
> Retrieving data... Postcode 2000 has a population of approximately 27,000 with a median age of 32.

---

**👤 You:**
> "Show available data topics."

**🤖 AI Agent:**
> Here are the available topics: 'population', 'income', 'housing', 'education', 'employment'.


## ❓ FAQ

**Q: How do I find my Mapulus API Key?**
Log in to Mapulus, go to Profile > API Keys, and you can generate your key there.

**Q: What regions are covered by Mapulus?**
Mapulus specializes in Australian geographic and statistical data (ABS Census boundaries).

**Q: Is my API Key secure?**
Absolutely. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mapulus](https://vinkius.com/mcp/mapulus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mapulus** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mapulus` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mapulus** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mapulus": {
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
