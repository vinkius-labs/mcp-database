# QWeather Ocean/Tide API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qweather-oceantide-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Monitor ocean tides — audit water levels and peaks via AI.

## Description
Empower your AI agent to orchestrate your entire maritime research and oceanographic auditing workflow with the **QWeather Ocean/Tide API**, the specialized source for global tide data. By connecting QWeather's ocean intelligence to your agent, you transform complex water level searches into a natural conversation. Your agent can instantly retrieve real-time tide tables, audit high and low water peaks, and query specific location metadata without you ever touching a technical portal. Whether you are planning coastal logistics or conducting marine research, your agent acts as a real-time oceanographic consultant, ensuring your data is always verified and precise.

### What you can do

- **Tide Auditing** — Retrieve high-resolution tide tables for global locations and maintain a clear view of water level changes.
- **Peak Oversight** — Audit high and low water times and heights to understand the temporal distribution of maritime scale instantly.
- **Geographic Discovery** — Query tide data by location ID or coordinates to maintain strict organizational control over regional data.
- **Ocean Intelligence** — Retrieve detailed oceanographic metadata to assist in deep-dive coastal classification.
- **Operational Monitoring** — Check API status to ensure your maritime research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your QWeather API Key
3. Start managing your oceanographic intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Mariners & Harbor Masters** — monitor tide levels and retrieve water metadata straight from your workflow.
- **Marine Researchers** — verify tide patterns and audit oceanographic markers without manual searching.
- **Coastal Planners** — perform rapid audits of water peaks and identify relevant maritime markers through natural language.
- **Operations Leads** — automate oceanographic data querying to orchestrate cross-functional maritime teams smoothly.


## Available Tools (2)
- **check_api_status**: Check if the QWeather Ocean service is operational
- **get_ocean_tide_data**: Get real-time tide data for a specific location and date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QWeather Ocean/Tide API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get tide data for location '101010100' (Shanghai) for '20240510' using QWeather."

**🤖 AI Agent:**
> I've retrieved the tide table for Shanghai! Notable peaks include a High Tide at 11:30 AM (3.5m) and a Low Tide at 5:45 PM (0.8m). Would you like the hourly water level metadata for this location?

---

**👤 You:**
> "What is the tide forecast for latitude 22.3193 and longitude 114.1694 (Hong Kong)?"

**🤖 AI Agent:**
> I've retrieved the real-time tide data for those coordinates! Multiple water level peaks are identified for today. I can provide the exact height and peak type metadata to assist in your maritime audit.

---

**👤 You:**
> "Show the full tide table for today."

**🤖 AI Agent:**
> I've retrieved the complete tide table for your selected location! It includes timestamped entries for all water level changes throughout the day. I can assist you with an audit of the most significant peaks if you'd like.


## ❓ FAQ

**Q: How do I find my QWeather API Key?**
Log in to your [**QWeather Developer portal**](https://dev.qweather.com/), create a project, and you will find your API Key in your dashboard. Copy and paste it below.

**Q: Does it support coordinate search?**
Yes. You can provide location coordinates (lat,lon) to the `get_ocean_tide_data` tool to retrieve precise regional tide metadata.

**Q: What data format is returned for tide tables?**
The API returns detailed hourly or daily tide tables, including timestamped water height and peak type metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qweather-oceantide-api](https://vinkius.com/mcp/qweather-oceantide-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **QWeather Ocean/Tide API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `qweather-oceantide-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **QWeather Ocean/Tide API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qweather-oceantide-api": {
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
