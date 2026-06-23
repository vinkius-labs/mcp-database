# Datalastic Maritime MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datalastic-maritime)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Universal maritime intelligence — search vessels, track positions, and find ports via AI.

## Description
Equip your AI agent with real-time global maritime intelligence through the **Datalastic** MCP server. This integration provides instant access to detailed information on thousands of vessels and ports worldwide. Your agent can search for ships by name, retrieve exhaustive metadata (including MMSI, status, and flag), and track real-time positions and ETAs for specific vessels. It also allows searching for maritime ports by country to find official UN/LOCODEs. Whether you are managing global logistics, auditing supply chains, or researching maritime traffic, your agent acts as a dedicated port captain and logistics analyst through natural conversation.

### What you can do

- **Vessel Search & Specs** — Find commercial ships by name and retrieve robust technical dimensions and tonnages.
- **Navigation Intelligence** — Retrieve real-time positions, ETAs, and historical AIS tracking paths for specific vessels.
- **Geofence Discovery** — Find all active vessels and cargo tankers located within a specific circular radius instantly.
- **Port Insights** — Discover maritime ports by country or name and retrieve exact geolocations and UN/LOCODEs.

### How it works

1. Subscribe to this server
2. Enter your Datalastic API Key (get it at datalastic.com)
3. Start querying global maritime data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Supply Chain Managers** — track cargo vessels and monitor delivery schedules in real-time.
- **Maritime Researchers** — analyze global shipping patterns and vessel distributions.
- **Trade Compliance Officers** — verify vessel details and flag information for international shipments.
- **Port Operations Teams** — quickly find port codes and technical data for global terminals.


## Available Tools (8)
- **get_port_details**: Get specific details and coordinates for a maritime port
- **get_vessel_history**: Get historical AIS track and location data for a vessel
- **get_vessel_pro_specs**: Get advanced technical specifications for a vessel
- **get_vessel_status**: Get real-time location and status for a specific vessel
- **find_vessels_in_radius**: Find all vessels currently located within a specific circular radius
- **search_ports_by_name**: Search for maritime ports by text name
- **search_ports_by_country**: Search for maritime ports in a specific country
- **search_maritime_vessels**: Search for vessels by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Datalastic Maritime** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for a vessel named 'Ever Given'."

**🤖 AI Agent:**
> Searching the Datalastic database... I've identified the 'Ever Given' cargo vessel with MMSI '353136000'. I can now retrieve its current position and destination if you'd like.

---

**👤 You:**
> "What is the current status and ETA for vessel MMSI '235114578'?"

**🤖 AI Agent:**
> Retrieving vessel details... The ship is currently 'Underway using Engine' and is heading to the Port of Southampton. The estimated time of arrival (ETA) is October 15th at 14:30 UTC.

---

**👤 You:**
> "List all major ports in 'Brazil'."

**🤖 AI Agent:**
> Retrieving port data for Brazil (BR)... I've found a list of terminals including Santos (BRSSZ), Paranaguá (BRPNG), and Itajaí (BRITJ). I can provide the exact coordinates or technical details for any of these ports.


## ❓ FAQ

**Q: Can I track a ship using its name?**
Yes! Use the `search_maritime_vessels` tool with the vessel's name. It will return a list of matching ships with their MMSI numbers, which you can then use for real-time tracking.

**Q: What is an MMSI number?**
MMSI stands for Maritime Mobile Service Identity. It is a unique 9-digit number used to identify a vessel's radio equipment and is the primary identifier for AIS tracking.

**Q: How can I find the official code for a port?**
Use the `search_ports_by_country` tool with the 2-letter ISO country code. The response will list ports in that country along with their official UN/LOCODEs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datalastic-maritime](https://vinkius.com/mcp/datalastic-maritime)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Datalastic Maritime** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `datalastic-maritime` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Datalastic Maritime** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "datalastic-maritime": {
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
