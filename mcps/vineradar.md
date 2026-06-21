# VineRadar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vineradar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search wine and vineyards — audit varietals and vintages via AI.

## Description
Empower your AI agent to orchestrate your entire wine research and vineyard auditing workflow with **VineRadar**, the comprehensive platform for global wine data. By connecting VineRadar to your agent, you transform complex varietal searches into a natural conversation. Your agent can instantly search for specific wines, audit vineyard locations, and retrieve detailed vintage metadata without you ever touching a wine app. Whether you are building a personal cellar or conducting market research on varietals, your agent acts as a real-time sommelier, ensuring your data is always detailed and well-categorized.

### What you can do

- **Wine Auditing** — Search for thousands of wines by name or keyword and retrieve detailed metadata, including ratings and vintages.
- **Vineyard Oversight** — Browse vineyard profiles by location to maintain a clear view of regional wine production.
- **Varietal Discovery** — Query wine varietals to understand the technological and regional distribution of specific grape types instantly.
- **Vintage Intelligence** — Retrieve full details for specific wine IDs to assist in deep-dive collection audits.
- **Market Monitoring** — List all supported varietals in the VineRadar catalog to identify trending wine themes in real-time.

### How it works

1. Subscribe to this server
2. Enter your VineRadar API Key
3. Start managing your wine intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sommeliers & Collectors** — monitor wine ratings and retrieve vineyard metadata straight from your workflow.
- **Wine Merchants** — verify varietal availability and audit regional distributions for your catalog.
- **Enthusiasts** — perform rapid audits of wine vintages and discover new labels through natural language.
- **Operations Leads** — automate wine data querying to orchestrate cross-functional hospitality teams smoothly.


## Available Tools
- **check_api_status**: Check if the VineRadar API is operational
- **get_vineyard_details**: Get full details for a specific vineyard by ID
- **get_wine_details**: Get full details for a specific wine by ID
- **list_wine_varietals**: List all wine varietals supported by VineRadar
- **search_vineyards**: Search for vineyards by location
- **search_wines**: Search for wines by name or keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VineRadar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Cabernet Sauvignon' wines using VineRadar."

**🤖 AI Agent:**
> I've retrieved 10 Cabernet Sauvignon wines. Notable labels include high-rated bottles from Napa Valley and Bordeaux. Would you like the full details for the top matches?

---

**👤 You:**
> "Find vineyards in 'Napa Valley'."

**🤖 AI Agent:**
> I've identified 5 premium vineyards in Napa Valley. Notable locations include 'Silver Oak' and 'Stag's Leap'. I can provide the specific IDs for these vineyards if you'd like.

---

**👤 You:**
> "What are the details for wine ID 12345?"

**🤖 AI Agent:**
> I've identified wine ID 12345 as a 2018 Reserve Merlot. It has a rating of 4.5 stars and is noted for its smooth finish. Would you like to see the vineyard metadata or similar varietals?


## ❓ FAQ

**Q: How do I find my VineRadar API Key?**
Log in to your [**VineRadar dashboard**](https://vineradar.com/account), and you will find your API Key under the 'Integrations' or 'Developer' section. Copy and paste it below.

**Q: Can the agent search for vineyards by region?**
Yes. Use the `search_vineyards` tool providing the location name (e.g., 'Napa Valley' or 'Bordeaux'). Your agent will return matching vineyards instantly.

**Q: Is vintage information included?**
Yes. The wine records retrieved by your agent include the vintage year and specific characteristics associated with that production cycle.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vineradar](https://vinkius.com/mcp/vineradar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VineRadar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `vineradar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VineRadar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vineradar": {
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
