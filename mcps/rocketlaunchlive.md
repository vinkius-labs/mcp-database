# RocketLaunch.Live MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rocketlaunchlive)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Track rocket launches worldwide — search upcoming launches, vehicles, companies, locations and missions.

## Description
Connect to **RocketLaunch.Live** and explore the world's curated rocket launch database through natural conversation — no API key needed for basic access.

### What you can do

- **Upcoming Launches** — Get the next upcoming rocket launches with vehicle, provider and mission details
- **Launch Search** — Search launches by date range, location, provider, vehicle or free-text query
- **Launch Details** — Get complete info on a specific launch including webcast links and status
- **Companies** — Browse launch providers and manufacturers (SpaceX, NASA, Roscosmos, etc.)
- **Locations** — Explore launch sites and facilities worldwide
- **Launch Pads** — Find specific launch pads (LC-39A, SLC-40, etc.)
- **Vehicles** — Search rockets and launch vehicles (Falcon 9, Starship, SLS, etc.)
- **Missions** — Browse missions and payloads (Starlink, Artemis, CRS, etc.)
- **Tags** — Filter launches by category (crew, satellite, ISS, etc.)

### How it works

1. Subscribe to this server
2. No API key needed for basic access (5 upcoming launches)
3. Start tracking rocket launches from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Space Enthusiasts** — track upcoming launches, explore vehicles and follow space missions
- **Educators** — demonstrate real-world rocket launches, providers and space industry to students
- **Researchers** — analyze launch frequency, provider market share and launch site utilization


## Available Tools (9)
- **get_tags**: Returns tag text and IDs for filtering launches.

Search launch tags
- **get_vehicles**: Returns vehicle names, descriptions, families and manufacturers.

Search launch vehicles (rockets)
- **get_companies**: Returns company names, countries, logos and active status. Filter by name or country code.

Search launch providers and manufacturers
- **get_launch**: Returns vehicle, provider, location, pad, mission, launch time, status and webcast links.

Get a specific launch by ID
- **get_locations**: Returns location names, country codes and associated launch pads.

Search launch locations
- **get_missions**: Returns mission names, descriptions and objectives.

Search launch missions
- **get_next_launches**: Free tier supports up to 5 launches without API key. Premium key unlocks full access.

Get the next upcoming rocket launches
- **get_pads**: Returns pad names, locations, maps and associated launch facilities.

Search launch pads
- **search_launches**: Live database for rocket launches. Supports free-text search, date range filtering, and filtering by location, provider, vehicle and tag. Returns launches with vehicle info, provider, launch site, mission details and status.

Search rocket launches


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RocketLaunch.Live** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What rocket launches are coming up next?"

**🤖 AI Agent:**
> Next 5 launches: 1. SpaceX Falcon 9 — Starlink Group (LC-39A, KSC) — Tomorrow 06:45 UTC. 2. Rocket Lab Electron — Capella Space (Launch Complex 1, NZ) — In 2 days. 3. ULA Atlas V — USSF mission (SLC-41, CCSFS) — In 4 days. 4. SpaceX Starship — IFT-7 (Starbase, TX) — In 5 days.

---

**👤 You:**
> "Show me all SpaceX launches this month."

**🤖 AI Agent:**
> Found 8 SpaceX launches this month: 5x Falcon 9 (Starlink missions from FL and CA), 2x Falcon Heavy (USSF and commercial), 1x Starship test flight. All launches include webcast links and detailed mission info.

---

**👤 You:**
> "What launch vehicles does Rocket Lab use?"

**🤖 AI Agent:**
> Rocket Lab operates the Electron rocket (small-lift, ~300kg to LEO) and is developing Neutron (medium-lift, reusable). Electron launches from Launch Complex 1 in New Zealand and Launch Complex 2 in Virginia.


## ❓ FAQ

**Q: Do I need an API key?**
No! Basic access works without authentication for the next 5 upcoming launches. For full search access and unlimited queries, a premium API key is available from rocketlaunch.live.

**Q: How far in advance are launches listed?**
Launches are typically listed weeks or months in advance based on official schedules from providers. Dates may change due to weather, technical issues or scheduling conflicts.

**Q: Can I filter launches by specific rockets?**
Yes! Use get_vehicles to find vehicle IDs, then use search_launches with the vehicle_id parameter to filter by specific rockets like Falcon 9, Starship or Atlas V.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rocketlaunchlive](https://vinkius.com/mcp/rocketlaunchlive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RocketLaunch.Live** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rocketlaunchlive` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RocketLaunch.Live** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rocketlaunchlive": {
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
