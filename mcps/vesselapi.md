# VesselAPI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vesselapi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Track maritime vessels — audit schedules and positions via AI.

## Description
Empower your AI agent to orchestrate your entire maritime research and vessel auditing workflow with **VesselAPI**, the comprehensive source for global shipping data. By connecting VesselAPI to your agent, you transform complex logistics searches into a natural conversation. Your agent can instantly track vessels by IMO number, audit upcoming port schedules, and retrieve real-time AIS positions without you ever touching a maritime dashboard. Whether you are conducting supply chain research or monitoring global trade flow, your agent acts as a real-time maritime consultant, ensuring your data is always precise and up-to-the-minute.

### What you can do

- **Vessel Auditing** — Retrieve high-resolution details for any vessel by IMO number, including flag, type, and build metadata.
- **Schedule Oversight** — Audit upcoming port calls and historical schedules to maintain a clear view of maritime logistics.
- **Position Intelligence** — Query real-time AIS positions to understand the current geographic distribution of vessels instantly.
- **Port Discovery** — List global maritime ports and retrieve localized metadata to assist in geographic planning.
- **Logistics Monitoring** — Check API status and monitor your data usage to maintain strict control over your research volume.

### How it works

1. Subscribe to this server
2. Enter your VesselAPI Key
3. Start managing your maritime intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Supply Chain Analysts** — monitor vessel movements and retrieve logistics metadata straight from your workflow.
- **Trade Researchers** — verify port calls and audit global shipping patterns without manual searching.
- **Logistics Managers** — perform rapid audits of vessel positions and identify potential delays through natural language.
- **Operations Leads** — automate maritime data querying to orchestrate cross-functional logistics teams smoothly.


## Available Tools (6)
- **check_api_status**: Check if the VesselAPI is operational
- **get_vessel_position**: Get the latest AIS position for a vessel
- **get_vessel_schedules**: Get upcoming port calls and schedules for a vessel
- **get_vessel_details**: Get comprehensive details for a vessel by IMO number
- **list_maritime_ports**: List global maritime ports supported by VesselAPI
- **search_vessels**: Search for vessels by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VesselAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get details for vessel with IMO 9411159 using VesselAPI."

**🤖 AI Agent:**
> I've retrieved the details for IMO 9411159! It is a Container Ship named 'Emma Maersk', sailing under the flag of Denmark. Would you like the latest position or upcoming port schedules?

---

**👤 You:**
> "Where is vessel 'MSC OSCAR' located right now?"

**🤖 AI Agent:**
> I've identified 'MSC OSCAR' and retrieved its latest AIS position. It is currently in the Suez Canal, heading North. I can provide the exact latitude and longitude metadata if you'd like.

---

**👤 You:**
> "Show upcoming schedules for IMO 9243394."

**🤖 AI Agent:**
> I've retrieved the schedule for that vessel. Its next port of call is Rotterdam, expected on 2024-05-15. I can provide the full list of planned stops and durations if you'd like.


## ❓ FAQ

**Q: How do I find my VesselAPI Key?**
Log in to your [**VesselAPI dashboard**](https://vesselapi.com/account), and you will find your API Key under the settings page. Copy and paste it below.

**Q: Does it support real-time AIS data?**
Yes. The `get_vessel_position` tool provides the latest AIS position received for the specified vessel IMO number.

**Q: Can the agent show port schedules?**
Yes. Use the `get_vessel_schedules` tool to retrieve upcoming port calls and arrival/departure metadata for any vessel.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vesselapi](https://vinkius.com/mcp/vesselapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VesselAPI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vesselapi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VesselAPI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vesselapi": {
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
