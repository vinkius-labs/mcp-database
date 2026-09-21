# River Gauges MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/river-gauges)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

Live streamflow and river level from USGS gauges — how high the river is right now, whether it is rising or falling, and what the site is.

## Description
Connect any AI agent to **real river gauge readings** — the streamflow and gage-height data the USGS measures at thousands of surface-water sites, refreshed as often as every 5 to 15 minutes. No key required.

### What you can do

- **Ask what the river is doing right now** — the latest streamflow and gage height at a site, plus the last few readings so the trend shows, with water temperature, conductance, dissolved oxygen and pH available on request
- **Get the recent level curve** — the gage-height history over the last hours, by default 24, with the range and whether the river is rising or falling over the window
- **Look up a gauge site** — name, coordinates, drainage area, altitude and site type, which is what puts a flow number in context
- **List gauges by state** — every USGS surface-water site in a state, to find the id you need

### How it works

1. Subscribe to this server — no account, no key
2. Ask your agent: "How high is the Potomac at Little Falls right now?", "Is the river rising at site 01646500?", "List the gauges in Maryland"
3. The agent reads the live gauge and answers in plain language

### Good to know

Streamflow is the volume of water moving past the gauge — cubic feet per second in the US. Gage height is the water level against the gauge staff, not an altitude above sea level, so it is only meaningful against that site's own history. Recent readings are marked provisional: USGS checks and revises them, so a number from the last day or two can change. Coverage is the United States.

### Who is this for

- **Paddlers, anglers and boaters** — "is my run in?" answered by the gauge that sits on it
- **Flood watchers and emergency managers** — a rising curve under heavy rain is the flood signature
- **Water utilities and irrigators** — real flow at the intake, not yesterday's report
- **Anyone with a chat window** — "is the river up?" answered from measurements, not a guess


## Available Tools (4)
- **get_river_conditions**: Returns the latest reading for each parameter the gauge reports, plus the last few measurements so the trend shows. Site ids are digits, e.g. 01646500 for the Potomac at Little Falls. Discover an id with list_gauges_by_state or get_gauge_site. By default asks for streamflow (00060) and gage height (00065); pass parameter_codes to add water temperature (00010), specific conductance (00095), dissolved oxygen (00300) or pH (00400). Readings marked provisional are preliminary — USGS revises them later.

Get live streamflow and gage height at a USGS river gauge — what the river is doing right now
- **get_gauge_site**: Drainage area is in square miles; altitude in feet.

Get metadata for one USGS gauge site: name, coordinates, drainage area, altitude and type
- **get_river_stage_history**: Reports the day range, the latest level, and whether the river is rising or falling over the window. This is the tool for "is the river coming up?" — a rising curve under heavy rain is the flood signature. Gage height is relative to the gauge staff, not a sea-level altitude; compare it against the site metadata and any local flood stage you know.

Get the recent gage-height curve at a USGS gauge — the shape a flood watch or a paddler reads
- **list_gauges_by_state**: Give a two-letter state code — "NY", "CA", "TX" — and get back every active stream gauge there that has instantaneous data. Counts are in the hundreds per state, so results are paged with limit (default 50, max 500) and the list is cached for 6 hours. This covers the United States only; USGS has no gauges outside it.

List the active USGS stream gauges in a US state that report real-time data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **River Gauges** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the Potomac doing at gauge 01646500 right now? Give me the flow and level, and whether it's rising or falling."

**🤖 AI Agent:**
> The Potomac at Little Falls (01646500) is running at about 2,400 ft³/s with a gage height near 2.7 ft. Over the last 24 hours the level has fallen roughly 0.3 ft — the river is going down and no flooding is forecast at this site.

---

**👤 You:**
> "List the USGS river gauges in Maryland. I'm looking for one near the Patapsco."

**🤖 AI Agent:**
> Maryland has roughly 190 active USGS surface-water gauges. The ones nearest the Patapsco are listed below with their site numbers — the closest is Patapsco River at Hollofield (01582500). Tell me which one you want and I will read its live flow and level.

---

**👤 You:**
> "The Mississippi has been rising all week. Show me the stage history at St. Louis for the last seven days."

**🤖 AI Agent:**
> Gauge 07010000 — Mississippi River at St. Louis, MO (38.629, -90.180) — reads 6.42 m as of 01:00 local on 20 Sep 2026, up from 1.69 m on 13 Sep. That is a rise of about 4.7 m in seven days across 336 half-hourly samples, and the peak of the series is the most recent reading, so the river was still climbing at last report.


## ❓ FAQ

**Q: Does this need an API key?**
No. All endpoints used here are USGS public water services. Subscribe and ask away.

**Q: What is the difference between streamflow and gage height?**
Gage height is how deep the water is against that gauge's own reference staff — it is a local number. Streamflow is the volume of water moving past the gauge, in cubic feet per second in the US. Two sites at the same height can have very different flows because of channel shape, which is why the site metadata includes the drainage area.

**Q: Why are recent readings marked provisional?**
USGS publishes data as soon as the gauge sends it, then reviews and corrects it as the record is assembled. A reading from the last day or two can shift — usually only slightly, sometimes more after a storm or if the sensor was fouled. Data older than a few months has been approved.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/river-gauges](https://vinkius.com/en/ai-agent-connect/river-gauges)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **River Gauges** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `river-gauges` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **River Gauges** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "river-gauges": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
