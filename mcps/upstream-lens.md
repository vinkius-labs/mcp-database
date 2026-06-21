# Upstream Lens MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/upstream-lens)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Monitor upstream oil and gas operations with production data analytics, well performance tracking, and field reporting tools.

## Description
Connect your **Upstream Tech Lens** account to any AI agent and simplify how you monitor conservation projects, analyze satellite imagery, and track environmental changes through natural conversation.

### What you can do

- **Project & Portfolio Oversight** — List all environmental projects and portfolios to manage your conservation assets.
- **Imagery Analysis** — Query available satellite imagery layers (Sentinel, Landsat, etc.) for specific property features.
- **Geospatial Insights** — Fetch detailed metadata and field observations for properties to track ground-truth data.
- **Environmental Monitoring** — List project notes and observations to keep a record of changes over time.
- **Organization Management** — Retrieve Lens organization profiles and verify account configurations.
- **Operational Status** — Check API health and connectivity to ensure your monitoring engine is always active.

### How it works

1. Subscribe to this server
2. Enter your Upstream Tech Lens API Key (found in your account dashboard)
3. Start monitoring your environmental assets from Claude, Cursor, or any MCP client

### Who is this for?

- **Conservation Managers** — quickly retrieve field notes and check satellite imagery availability via simple AI queries.
- **Environmental Analysts** — monitor changes in property features and verify geospatial metadata directly from the workspace.
- **Sustainability Teams** — track project observations and maintain an organized portfolio of environmental monitoring sites.


## Available Tools
- **get_property_details**: Get details for a specific property feature
- **get_organization_info**: Get organization metadata
- **check_api_health**: Check Lens API health
- **list_property_imagery**: ) for a specific property.

List available imagery layers for a property
- **list_project_notes**: Can be filtered by update date.

List observations and notes for a project
- **list_project_observations**: List detailed project observations
- **list_portfolios**: List all portfolios
- **list_projects**: List all environmental projects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Upstream Lens** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active environmental projects in my Lens account."

**🤖 AI Agent:**
> I've retrieved your projects. You have access to: 'Amazon Rainforest Restoration', 'Coral Reef Protection', and 'Midwest Soil Health'. Which one would you like to inspect?

---

**👤 You:**
> "Show me the latest field notes for the 'Amazon Restoration' project."

**🤖 AI Agent:**
> I've fetched the project notes. There are 2 recent observations: 'Tree growth rate 15% higher than Q3' and 'New sensor installed at station B'. Shall I retrieve the previous history?

---

**👤 You:**
> "List available satellite imagery layers for property 'feat_10293'."

**🤖 AI Agent:**
> I found 3 available imagery layers for property feat_10293: 'Sentinel-2 (True Color)', 'Sentinel-2 (NDVI)', and 'Landsat 8'. The most recent capture was yesterday. Shall I retrieve the download metadata?


## ❓ FAQ

**Q: Can I see if new satellite images are available for my project?**
Yes! Use the `list_property_imagery` tool and provide the Property ID. Your agent will retrieve all available imagery layers (Sentinel, Landsat, etc.) with their respective capture dates.

**Q: How do I retrieve field notes for a specific conservation project?**
Run the `list_project_notes` query with your Project ID. You can also provide an optional timestamp to filter only notes updated after a specific date.

**Q: Is it possible to see the geospatial metadata for a property feature?**
Absolutely. Use the `get_property_details` tool with the Feature ID to retrieve detailed geospatial data and metadata for any monitored property.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/upstream-lens](https://vinkius.com/mcp/upstream-lens)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Upstream Lens** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `upstream-lens` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Upstream Lens** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "upstream-lens": {
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
