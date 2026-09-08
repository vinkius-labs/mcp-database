# GSI Japan Terrain & Geocoding MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/gsi-japan-terrain-geocoding)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Japan's Geospatial Information Authority as an MCP: official elevation for any point (1m laser DEM — Mt. Fuji at 3770m), Japanese address geocoding and multi-point terrain profiles. Keyless.

## Description
The **Geospatial Information Authority of Japan (GSI, 国土地理院)** — the official national mapping agency — as a single MCP server.

### What you can do
- **Official elevation** — query any point in Japan against the GSI DEM: from 1m-resolution laser scans (Mt. Fuji reads 3770.4m) down to 10m grids; the source (`hsrc`) is always disclosed
- **Address geocoding** — resolve Japanese addresses and landmarks (東京都千代田区, 東京タワー, 大阪城) to coordinates via the official GSI matcher
- **Elevation profiles** — batch up to 25 points to build terrain profiles for routes, hikes or flood analysis
- **Place comparisons** — geocode + elevation for multiple places in one call: "how high is Kyoto vs Tokyo vs Fuji?"

### Why GSI?
Mountains define Japan. Global DEMs (SRTM, ASTER) give coarse 30-90m grids; the GSI laser survey measures the actual ground at 1m resolution — the same data behind Japan's earthquake, landslide and flood models. And its geocoder understands kanji addresses that confuse generic geocoders.

### Who is this for?
Hiking and outdoor apps, real-estate and construction analysis, disaster/terrain research, logistics, game development and AI agents that need authoritative Japanese terrain and address data.


## Available Tools (4)
- **get_location_elevation_profile**: Points without DEM data return null elevation.

Get elevations for up to 25 coordinates at once (elevation profile for a route or area)
- **get_elevation**: Coordinates: lon 120-150 (e.g. 139.69 Tokyo), lat 30-46 (e.g. 35.69). Returns null elevation for water or unmeasured points — useful for terrain analysis, flood/hiking checks, geology.

Get the official elevation of any point in Japan (GSI 1m/5m/10m laser DEM)
- **geocode_address**: g. 東京都千代田区, 東京タワー, 札幌市): coordinates [lon, lat], display title and address code. Accepts partial names — broader terms return multiple candidate areas ranked by the GSI matcher. Japanese input strongly recommended.

Geocode a Japanese address or place name to coordinates (official GSI search)
- **compare_places_terrain**: Returns name, coordinates, elevation and DEM source — quick way to answer "how high is X vs Y" without juggling tools.

Compare multiple places: geocode each name then fetch its elevation in one call


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GSI Japan Terrain & Geocoding** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How high is Mount Fuji according to official data?"

**🤖 AI Agent:**
> 🗻 **Mt. Fuji (138.7274, 35.3606) — GSI official**

Elevation: **3770.4 m** (source: 1m laser DEM)

That's the survey-grade value at the summit — right between the official 3775.63m (Kengamine peak marker) and 3776m commonly cited. Want the profile along a climbing route?

---

**👤 You:**
> "Where exactly is Osaka Castle and how high is it?"

**🤖 AI Agent:**
> 🏯 **Osaka Castle (大阪城) — GSI**

Coordinates: 135.5133, 34.6872 (Osaka-jo, Chuo-ku, Osaka)
Elevation: **17.8 m** (5m DEM)

Built on a hill above the moat — strategically ~10m above the surrounding city. Want Kyoto's Nijo Castle for comparison?

---

**👤 You:**
> "Build an elevation profile from Tokyo station to the summit of Fuji"

**🤖 AI Agent:**
> ⛰️ **Tokyo → Fuji elevation profile (GSI 1m DEM)**

1. Tokyo Station: 3.5 m
2. Hachioji: 122.0 m
3. Gotemba: 465.0 m
4. 5th Station (km 0): 1440.0 m
5. Summit: 3770.4 m

Total gain ~3767 m over ~100km. I can add more waypoints or reverse the profile.


## ❓ FAQ

**Q: Do I need an API key or registration?**
No. Both the GSI elevation service and the address search are public endpoints — no key, no registration. Keep request rates reasonable and they work indefinitely.

**Q: Why does elevation sometimes return null?**
Points on water, or outside areas covered by the current DEM grids (some remote islands), have no elevation value. The response also tells you which DEM layer served the value (1m laser, 5m or 10m), so you can judge precision.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/gsi-japan-terrain-geocoding](https://vinkius.com/ai-agent-connect/gsi-japan-terrain-geocoding)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GSI Japan Terrain & Geocoding** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gsi-japan-terrain-geocoding` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GSI Japan Terrain & Geocoding** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gsi-japan-terrain-geocoding": {
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
