# Marine Conditions MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/marine-conditions)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [weather-climate](../categories/weather-climate.md)

The marine go/no-go for any coastal point — official NWS marine warnings in effect for those waters, wave and swell forecasts, and the latest station observation, in one answer.

## Description
Connects an AI agent to the National Weather Service's marine programme — the same forecasts and warnings a harbourmaster or a coast-guard station reads.

### What you can do

- **The go/no-go** — give a latitude and longitude and get every active marine warning for those waters alongside the wave and swell forecast, in one answer
- **Read a warning** — the full text of the Small Craft Advisories, Gale Warnings, Storm Warnings and Beach Hazards in effect for one zone, with severity, timing and the action the agency recommends
- **Forecast the sea** — significant wave height, wave period, primary and secondary swell, wind waves, wind speed and gusts, hour by hour, up to a week
- **Read a station** — the latest measured wind, pressure, visibility, temperature and humidity from the observing station covering the point
- **Find a zone** — the catalogue of 699 coastal and offshore marine zones, filterable by forecast office or name

### Why it matters

Marine warnings are issued against zones, not points, and zones lie over water — so a point query alone cannot surface the warning that governs the stretch you are heading to. This server does the join the agency's own workflow uses: the point resolves to its forecast office, and the zones that office warns are checked for active alerts, with the wave forecast for the point attached.

Two properties of the source shape every answer. Wind arrives in kilometres per hour, pressure in pascals and visibility in metres, and each is converted into the unit a mariner reads — knots, hectopascals and kilometres. And the forecast is not a single hourly series: the agency gives every variable its own time axis, wave height in multi-day blocks and wind hour by hour, so the two are expanded onto a shared clock before they are read side by side. A wave height of null means the grid cell carries no marine layer at all — inland, or sheltered — while a zero is a genuine forecast for flat water.


## Available Tools (5)
- **get_wave_forecast**: Give a latitude and longitude in decimal degrees; the point is resolved to its forecast office and grid cell, and the marine variables of that cell are reported as the current values plus an hourly series. Wave height is in metres, period in seconds, wind in knots, and swell directions in degrees with a compass point. Marine variables exist only where the grid cell is over water: an inland cell reports null for every wave field and the response says so rather than inventing calm, while a sheltered cell can report a true height of zero — a null means the cell has no sea layer at all, a zero means it measured flat. Wind is reported either way. Ask for up to 168 hours; the default is 24.

The wave, swell and wind forecast for a coastal point — significant wave height, wave period, primary and secondary swell, wind waves, wind speed and gusts, hour by hour
- **list_marine_zones**: The catalogue holds all 699 marine zones: coastal and offshore, around the Atlantic, Gulf, Pacific, Great Lakes, Alaska, Hawaii, Puerto Rico and the Pacific islands. Filter by zone_type coastal or offshore, by the three-letter forecast office cwa such as LOX, or by a name fragment like "Chesapeake"; every zone carries the cwa field, which is the join the alert layer uses. Zones have no geometry and no state in this catalogue, so a zone cannot be found by drawing a polygon or by a state alone — name or office is the way. Results are paginated with offset and amount.

The catalogue of NWS marine zones — 699 coastal and offshore zones with their ids, names and the forecast office that warns each one
- **check_marine_conditions**: Give a latitude and longitude in decimal degrees — for example 32.72, -117.17 for San Diego. The point is resolved to its National Weather Service forecast office, every marine zone that office warns is checked for active alerts, and the wave and swell forecast for the point is attached. Marine zones lie over water, so a point query by itself cannot find their warnings — this tool does the office join and reports which zones were checked. Alerts are sorted most severe first and carry the headline, the timing and the recommended action. An answer with no alerts means no official warning, not necessarily calm water: waves and wind are reported alongside, and a Small Craft Advisory can be issued an hour after this answer, so re-check close to departure.

The marine go/no-go for a location — official NWS marine warnings in effect for those waters, plus the wave, swell and wind forecast, in one answer
- **get_current_conditions**: Give a latitude and longitude; the point resolves to its forecast office and grid cell, the stations covering that cell are listed, and the newest observation from the nearest one is reported with its timestamp. Observations are measurements, so they disagree with the forecast when the forecast is for a different time or place — trust the observation for "right now". Some stations report empty values for every sensor, which the response flags, and a grid cell with no covering stations reports none rather than inventing a reading.

The latest observation from the weather station covering a point — measured wind, pressure, visibility, temperature and humidity, not a forecast
- **get_marine_alerts**: The id looks like "ANZ531" — three letters then digits. Each alert reports its severity, certainty and urgency, when it took effect and when it ends or expires, the headline the NWS published, the full description, and the action the agency recommends. Alerts are sorted most severe first. An answer of zero alerts means the zone is not under an official warning at this moment — that is a statement about warnings, not about the sea, which may still be rough.

The official marine warnings and advisories in effect for one NWS marine zone — Small Craft Advisories, Gale Warnings, Special Marine Warnings and Beach Hazards, with their full text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Marine Conditions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We're thinking of taking the boat out from Annapolis tomorrow. Are there any marine warnings in effect for the Chesapeake, and what are the waves and wind doing?"

**🤖 AI Agent:**
> I'll run the go/no-go for Annapolis — the point resolves to its forecast office, every marine zone that office warns is checked for active warnings, and the wave and swell forecast is attached, so you get the official picture and the sea state in one answer.

---

**👤 You:**
> "I see a Small Craft Advisory was mentioned for the Chesapeake. What exactly does it say, and until when does it run?"

**🤖 AI Agent:**
> Let me read the warning itself for that zone — the full text the agency published, its severity, when it took effect, when it ends, and the action it recommends, which is the part that tells you who should stay ashore.

---

**👤 You:**
> "Planning a kayak paddle near San Diego for the weekend. What will the sea be like over the next couple of days?"

**🤖 AI Agent:**
> I'll pull the wave forecast for that point — significant height, period, primary and secondary swell and wind, expanded hour by hour across the weekend. If the grid cell reports null for the wave fields rather than a value, that means the cell carries no marine layer and I'll say so instead of reading a flat-calm into it.


## ❓ FAQ

**Q: Why do the alerts come back for zones I did not ask about?**
Marine warnings are issued against zones, and zones lie over water, so a latitude and longitude cannot be looked up in the alert list directly. check_marine_conditions resolves your point to its forecast office and then checks every zone that office warns — that is the join the agency's own workflow uses, and the response names which zones were checked. When you want the warning text for one specific zone, use get_marine_alerts with its id.

**Q: What does a wave height of null mean, and what does zero mean?**
They are different things and the response keeps them distinct. Null means the grid cell carries no marine layer at all — the point is inland, or in a sheltered cell the agency does not forecast swell for — and the response says so rather than presenting a false calm. Zero is a genuine forecast value: the agency modelled that cell and expects flat water there, which happens in bays and behind headlands. Wind is reported either way, because the wind forecast covers inland cells too.

**Q: Can I trust this enough to decide whether to go out?**
As the official picture, not as a guarantee. This is the same warning layer a coast-guard station reads, and an answer of zero alerts means no official warning is in effect at that moment — not that the water is safe. Waves and wind are reported alongside the warnings for that reason, and a Small Craft Advisory can be issued an hour after this answer is given. Re-check close to departure, and read the alert's recommended-action text before deciding.

**Q: Why is the wind in knots when the forecast says kilometres per hour?**
Because knots is the unit boating is done in, and the server converts before answering rather than making you convert. The agency sends wind in kilometres per hour on both the forecast and the observation endpoints, pressure in pascals and visibility in metres; each is turned into knots, hectopascals and kilometres so every reading arrives in the unit a mariner expects. Wave height stays in metres and wave period in seconds, which is how the marine forecast is published.

**Q: Do I need an API key or an account?**
No. The National Weather Service publishes this data openly, and the server reads it without authentication. There is no key to obtain, no quota to manage and no sign-up step.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/marine-conditions](https://vinkius.com/en/ai-agent-connect/marine-conditions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Marine Conditions** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `marine-conditions` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Marine Conditions** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "marine-conditions": {
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
