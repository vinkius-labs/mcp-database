# Satellite Tracking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/satellite-tracking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Track 16,000+ satellites in real time — the full Starlink constellation, the ISS, and every active object in orbit, with live orbital elements from Celestrak.

## Description
Connect any AI agent to **live satellite tracking** — orbital elements for everything in Earth orbit, served from Celestrak's public GP data. No API key required.

### What you can do

- **The Starlink constellation** — every satellite SpaceX has put up, with live orbital elements
- **Space stations** — the ISS and the rest of that group
- **Every active satellite** — roughly 16,000+ objects
- **The brightest objects** — the ~150 most likely to be visible during a pass
- **Recent launches** — objects added to the catalog in the last 30 days
- **Single lookups** — by NORAD catalog id, by name, or by launch (international designator)

Each result carries the full GP element set: epoch, inclination, period, apogee, perigee, eccentricity and the NORAD id.

### How it works

1. Subscribe to this server — no account or key needed
2. Ask your agent: "Where is the ISS right now?", "How many Starlinks are in orbit?", "What did the first Starlink launch put up?"
3. Large groups paginate — the agent walks through with offset/limit

Celestrak refreshes orbital elements **once every 2 hours**. A repeat call inside that window comes back unchanged, which the server reports clearly rather than silently re-serving.

### Who is this for

- **Space enthusiasts and educators** — answer orbital questions from a chat instead of scraping TLE files
- **Ham operators and observers** — plan passes from current elements
- **Analysts** — count and inspect a constellation without writing a parser
- **Developers** — prototype space apps with agent-driven element retrieval


## Available Tools (8)
- **get_satellite_by_intdes**: "2019-074" returns the whole first Starlink launch; "2019-074A" returns only its first object. This is the fastest way to list everything a single rocket put up.

Get every object from one launch by its international designator (e.g. 2019-074 = first Starlink launch)
- **get_satellite_by_name**: A partial name can match many objects, so this returns all matches. If nothing matches, switch to the NORAD id with get_satellite_by_norad_id.

Find satellites by name — e.g. "STARLINK-1008", "ISS (ZARYA)", "HST"
- **get_satellite_by_norad_id**: If you have a name instead, use get_satellite_by_name. Returns one element set with epoch, inclination, period, apogee and perigee.

Get the live orbital elements of one satellite by its NORAD catalog id (e.g. 25544 = the ISS)
- **list_space_stations**: No pagination needed in practice. Elements refresh once every 2 hours at Celestrak; a repeat call inside that window says "not updated", which means your data is still current.

List space stations and large orbital infrastructure — the ISS and the rest of that group — with live orbital elements
- **list_active_satellites**: ALWAYS paginate with offset/limit rather than pulling it all into context. Start with limit=100 and increase offset to walk through. If the user wants one constellation or one launch, use list_starlink_satellites or get_satellite_by_intdes instead — this tool is for exhaustive coverage. Elements refresh once every 2 hours at Celestrak.

List every active satellite in orbit — about 16,000+ objects, all with live orbital elements
- **list_brightest_satellites**: This is the right starting point for "what can I see overhead tonight". The orbital elements here let you work out pass geometry; Celestrak refreshes them once every 2 hours.

List the brightest satellites — the ones most likely to be visible to the naked eye during a pass
- **list_recently_launched_satellites**: Useful for tracking a fresh launch before its objects spread out. Elements refresh once every 2 hours at Celestrak.

List satellites launched in the last 30 days — newest objects in orbit
- **list_starlink_satellites**: The constellation is thousands of satellites, so this tool paginates: pass offset to page through results, limit up to 500 per call. Celestrak refreshes these elements only once every 2 hours — a second call inside that window returns "not updated", which means the data you already have is current, not an error. To find one specific Starlink, use get_satellite_by_name with e.g. "STARLINK-1008" instead of paging the whole constellation.

List the full Starlink satellite constellation with live orbital elements from Celestrak


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Satellite Tracking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many Starlink satellites are in orbit right now, and what orbit do they fly?"

**🤖 AI Agent:**
> The constellation has about 7,000 active satellites in low Earth orbit at roughly 53° inclination, circling every ~92 minutes at around 550 km. I pulled the element sets from Celestrak and aggregated the inclination and period.

---

**👤 You:**
> "Get me the ISS's current orbital elements."

**🤖 AI Agent:**
> The ISS (NORAD 25544) is flying at 51.6° inclination with a period of about 92.7 minutes — roughly 420 km perigee and 440 km apogee. Elements are fresh as of the latest Celestrak epoch.

---

**👤 You:**
> "Which satellites are the brightest? I want to actually spot one tonight."

**🤖 AI Agent:**
> The visual group holds 156 objects bright enough to catch with the naked eye, and the top of the list is mostly spent upper stages — ATLAS CENTAUR 2 (NORAD 694), THOR AGENA D R/B (NORAD 733) and a string of SL-8 rocket bodies. Rocket bodies are large and they tumble, so they catch a lot of sunlight and often flare brighter than the working satellites beneath them. Pick one, check its pass times for your location, and look for a steady object drifting across the sky.


## ❓ FAQ

**Q: Does this need an API key?**
No. Celestrak publishes its GP orbital elements openly, so this server works the moment you subscribe. Nothing to generate and nothing to paste.

**Q: Why do the same satellites come back unchanged when I ask again?**
Celestrak refreshes orbital elements once every 2 hours. Requesting the same group inside that window returns a clear "not updated" message rather than new data — the elements you already have are still current. Wait about two hours before re-fetching.

**Q: How do I find one specific satellite?**
Three ways: by NORAD catalog id (25544 is the ISS), by name ("STARLINK-1008", "ISS (ZARYA)"), or by international designator to get an entire launch at once (2019-074 returns the whole first Starlink launch). For a single satellite, name or id is far faster than paging the constellation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/satellite-tracking](https://vinkius.com/en/ai-agent-connect/satellite-tracking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Satellite Tracking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `satellite-tracking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Satellite Tracking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "satellite-tracking": {
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
