# US Airport Weather Sentinel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/us-airport-weather-sentinel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Know what's happening at your airport before you roll: latest METAR conditions plus every active NWS weather alert for the airport's zone, with since-based deltas so the agent re-checks and reports only what changed — keyless, stateless.

## Description
US Airport Weather Sentinel wraps the public National Weather Service API so your agent can answer the two questions travelers actually ask: "is anything happening at my airport right now?" and "what's changed since my last check?"

### What you can do

- **One snapshot of the whole airport** — latest METAR observation (temperature, wind/gusts, visibility, conditions) joined with every active NWS alert in the airport's forecast zone
- **Re-check, not re-read** — delta tools take the timestamp of your previous check and return only what changed: new weather text, gusts above 39 km/h, visibility under 1.5 km, or newly issued alerts
- **Watch one alert type** — follow only FloodWarnings, WinterStormWarnings, TornadoWarnings or any NWS event type for an airport
- **Batch up to 3 airports** — a single call gives temperature, weather and active alert counts for SFO, JFK, ORD (or any mix of major US airports)

### How it works

1. Subscribe to this server (no credential, no account — the NWS API is public)
2. Ask "is there anything going on at SFO?" — one call returns conditions + active alerts
3. Keep the `as_of` timestamp in context; on the next check, pass it as `since` and the agent reports only the delta

### Who is this for?

- **People who fly** — commuters and travelers who want to know about delays, IFR conditions and active warnings without opening five tabs
- **Agents & automations** — a scheduled "airport pulse" that flags gusts, icing and new alerts, computed server-side
- **Planners & dispatchers** — multi-airport watchlists with per-airport error isolation


## Available Tools (6)
- **airport_status**: Use it as the first check before travel, and re-run it to detect new alerts between calls. conditions may be null if the station feed is momentarily empty (see station_note).

Current conditions and active weather alerts for one US airport (its NWS forecast zone)
- **alert_watch**: g. FloodWarning, HighWindAdvisory, SevereThunderstormWarning, WinterStormWarning, TornadoWarning, HurricaneWarning). With no event, returns every active alert and the list of commonly watched event types. Zero results is a meaningful answer: no such alert is active in the zone right now.

Active NWS alerts for an airport's zone, optionally filtered by one event type
- **alerts_delta**: Pass since as the ISO-8601 timestamp of your previous check (from alerts_delta.active_now or airport_status). The NWS feed keeps only the most recent alerts, so a very old baseline may miss alerts older than the window — the note says so. Test messages are removed automatically.

New and recently expired NWS alerts for an airport's zone since your last check
- **conditions_delta**: 5 km), changed_weather, max_gust_kmh, min_visibility_km, temp_range_c. Pass since as an ISO-8601 timestamp — the as_of value from your previous airport_status call. The station posts roughly every 5-15 minutes; the feed is capped at 50 observations, so if your baseline is older than that window the result says how far back it reaches (changed=false with a note).

What changed in observed weather conditions since your last check, for one airport
- **find_airports**: Use it to discover the exact IATA code before calling the other tools, or when the user named an airport in words. If no airport matches, the error lists the supported codes so you can pick one.

Find supported US airports by IATA code, ICAO code, city, or name fragment
- **watch_status**: Keep it to 3 — more trips the anonymous NWS rate limit and the whole call fails. Per-airport errors are reported in that row without failing the others.

Compact current status for up to 3 US airports in one call


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Airport Weather Sentinel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is there anything going on at SFO right now that would affect my flight?"

**🤖 AI Agent:**
> Runs airport_status on SFO and reports conditions + any active NWS alerts in the zone.

---

**👤 You:**
> "Last check at JFK was at 14:00 UTC — what changed since then?"

**🤖 AI Agent:**
> Runs conditions_delta/alerts_delta on JFK with since=that timestamp and reports only the delta.

---

**👤 You:**
> "Watch ORD for flood and winter alerts."

**🤖 AI Agent:**
> Runs alert_watch on ORD for FloodWarning/WinterStormWarning and reports the active ones.


## ❓ FAQ

**Q: Do I need credentials?**
No. The National Weather Service API is public and requires no key, no account, no signup. Anonymous access is rate-limited to roughly 30 requests per minute, which is why batched calls are capped at 3 airports and the tools keep their fetch count low.

**Q: How do the "since" delta tools work?**
The server is stateless. Call airport_status (or any delta tool), keep the as_of timestamp in the agent's context, and on the next check pass it as since. The tool fetches the recent observations/alerts and returns only what is newer than that timestamp — e.g. new alerts, gusts above 39 km/h, visibility drops. The station feed keeps ~50 most recent observations, so a baseline older than that window comes back as "no observations since X" with a note.

**Q: Which airports are supported?**
The major US commercial airports (roughly 45): JFK, LGA, EWR, BOS, IAD, ATL, ORD, DFW, AUS, DEN, SEA, SFO, LAX, SNA, PHX, LAS, SLC, MCO, MIA, FLL, TPA, MSY, STL, DTW, BNA, MEM, CHS, CLT, RDU, GSP, OAK, PDX, GEG, RNO, ONT, SAN, HNL and more. find_airports lists the exact supported codes; the airport code resolves to its NWS forecast zone and METAR station automatically.

**Q: Why can't I filter alerts by state or time?**
The NWS API's 2026 revision dropped the state/sent/since query parameters — the server resolves your airport to its NWS forecast zone and filters time deltas client-side from the timestamps each alert carries. So you always filter by the airport (zone) and by `since`, which is what a traveler cares about anyway.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/us-airport-weather-sentinel](https://vinkius.com/en/ai-agent-connect/us-airport-weather-sentinel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Airport Weather Sentinel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-airport-weather-sentinel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Airport Weather Sentinel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-airport-weather-sentinel": {
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
