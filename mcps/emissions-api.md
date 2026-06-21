# Emissions API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emissions-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage your environmental research — audit air quality and gas emissions via AI.

## Description
Empower your AI agent to orchestrate your entire environmental research workflow with **Emissions API**, the open source platform for satellite-based emission data. By connecting Emissions API to your agent, you transform complex gas monitoring into a natural conversation. Your agent can instantly query carbon monoxide, methane, and ozone levels for any country without you ever touching a technical portal. Whether you are conducting climate research or monitoring industrial impact, your agent acts as a real-time environmental analyst, ensuring your data is always grounded in precise, satellite-derived measurements.

### What you can do

- **Gas Auditing** — Query real-time and historical levels of Carbon Monoxide, Methane, and Ozone to maintain a clear view of atmospheric composition.
- **Regional Oversight** — Retrieve emission data for specific countries or geographic coordinates to understand local environmental trends.
- **Temporal Intelligence** — Query data across specific date ranges to monitor changes in gas concentrations over time.
- **Spatial Discovery** — Retrieve emission measurements in GeoJSON format to maintain strict control over geographic data distribution.
- **Product Discovery** — List all available gas products in the catalog to identify relevant markers for your research.

### How it works

1. Subscribe to this server
2. No API Key required (Emissions API is a public and free service)
3. Start managing your environmental intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Environmental Scientists** — monitor global gas concentrations and retrieve satellite metadata straight from your workflow.
- **Policy Makers** — verify regional emission levels and audit atmospheric trends without manual data exports.
- **Sustainability Leads** — perform rapid audits of local air quality and discover environmental insights through natural language.
- **Operations Leads** — automate atmospheric data querying to orchestrate cross-functional climate teams smoothly.


## Available Tools (6)
- **get_carbon_monoxide**: Get carbon monoxide emission data
- **get_geojson_emissions**: Get emission data in GeoJSON format
- **get_methane**: Get methane emission data
- **get_nitrogen_dioxide**: Get nitrogen dioxide emission data
- **get_ozone**: Get ozone emission data
- **get_available_products**: List all available gas products in the database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emissions API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the latest carbon monoxide level in Germany (DE)?"

**🤖 AI Agent:**
> I've retrieved the measurement for Germany. The latest value is approximately 0.03 mol/m². The timestamp associated with this satellite reading is from yesterday. Would you like the data for other regions?

---

**👤 You:**
> "List all available gas products in the Emissions API."

**🤖 AI Agent:**
> I've scanned the catalog. Available products include carbonmonoxide, methane, ozone, and nitrogendioxide. I can retrieve emission data for any of these markers.

---

**👤 You:**
> "Show methane emission trends for the last 30 days in the US."

**🤖 AI Agent:**
> I've retrieved the methane levels for the US over the requested period. The values range from 1800 to 1900 ppb. I can provide a summary of the peak days if you'd like.


## ❓ FAQ

**Q: Is an API Key required for Emissions API?**
No. Emissions API is a free and open service. This server works out of the box without any static credentials required.

**Q: What gases can be audited via the agent?**
You can query Carbon Monoxide (`carbonmonoxide`), Methane (`methane`), Ozone (`ozone`), and Nitrogen Dioxide (`nitrogendioxide`) using specialized tools.

**Q: Is the data historical or real-time?**
The API provides historical measurement data collected by the Sentinel-5P satellite, typically updated daily with a short processing lag.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emissions-api](https://vinkius.com/mcp/emissions-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emissions API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emissions-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emissions API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emissions-api": {
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
