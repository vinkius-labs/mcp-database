# Moscow Sport: Stadiums, Pools & Pitches MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moscow-sport-stadiums-pools-pitches)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sports-fitness](../categories/sports-fitness.md)

Keyless Moscow sport: sport centres and fitness clubs, pitches by surface and lighting, pools, stadiums, ice rinks and playgrounds, plus the Wikipedia stadium roll.

## Description
The mapped sport estate of the city, keyless — over 1,000 sport centres and fitness clubs, nearly 4,000 pitches, a few hundred pools and stadiums, and the Wikipedia stadium roll.

### What you can do
- **find_sport_centres** — sport centres, fitness clubs and running tracks (over 1,000) filtered by sport, name and open now
- **find_pitches** — outdoor pitches and courts (nearly 4,000) filtered by sport, surface and floodlighting
- **find_swimming_pools** — swimming pools (a few hundred), indoor or outdoor, with hours and contacts
- **find_stadiums** — stadiums and arenas — Luzhniki, CSKA, Dynamo — filtered by name and sport
- **find_ice_rinks_and_ski** — ice rinks and ski bases for the winter season, filtered by name and sport
- **find_playgrounds** — children playgrounds (several thousand) — mostly unnamed, usable as a density map around an address
- **stadiums_wiki** — the Russian Wikipedia roll of Moscow stadiums, with a short encyclopaedia entry for the first
- **sport_profile** — citywide counts of sport centres, fitness clubs, pitches, pools, stadiums, ice rinks and playgrounds in one call

### Who is this for
People who want a swim, a court or a gym tonight; parents planning a playground route; and visitors heading to a match at Luzhniki.


## Available Tools (8)
- **find_ice_rinks_and_ski**: Each row carries the name, sport, lighting and the coordinate. Filter by name fragment (e.g. "Каток") or narrow to a neighbourhood with lat/lon/km. Seasonal outdoor rinks appear and disappear; the open_now filter uses the mapped opening hours, which not every rink carries.

Find Moscow ice rinks and ski bases
- **find_pitches**: Each row carries the name, the sport, the surface, the lighting flag and the coordinate. Filter by sport (e.g. "soccer", "basketball", "tennis", "table_tennis") or find the pitches around you with lat/lon/km.

Find Moscow sport pitches and courts
- **find_playgrounds**: Each row carries the name where mapped, the surface and the coordinate. Filter by surface or find the playgrounds around an address with lat/lon/km. Most playgrounds are unnamed; use the coordinate list as a density map rather than a directory.

Find Moscow children playgrounds
- **find_sport_centres**: Each row carries the name, the sport tags, the opening hours, the surface and the coordinate. Filter by sport (e.g. "fitness", "tennis", "boxing") or narrow to a neighbourhood with lat/lon/km.

Find Moscow sport centres and fitness clubs
- **find_stadiums**: Each row carries the name, sport tags, capacity where mapped, opening hours and the coordinate. For the encyclopaedic roll of Moscow stadiums use stadiums_wiki.

Find Moscow stadiums and arenas
- **find_swimming_pools**: Each row carries the name, the opening hours, whether the pool is covered and the coordinate. Filter by name fragment or narrow to a neighbourhood with lat/lon/km.

Find Moscow swimming pools
- **sport_profile**: Use it to size a district ("how many mapped football pitches are there in Moscow?") without paging through lists. No filters — this is a profile, not a search.

Citywide Moscow sport profile
- **stadiums_wiki**: Useful for the capacity, opening year and home club of a ground, none of which OSM tags reliably carry. Pass detail: "true" to fetch the summary of the first listed stadium.

Moscow stadium roll from Russian Wikipedia


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moscow Sport: Stadiums, Pools & Pitches** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is there a floodlit football pitch near me?"

**🤖 AI Agent:**
> find_pitches with sport: "soccer", lit: "yes" and your coordinates returns the mapped pitches with surface and lighting.

---

**👤 You:**
> "Where can I swim indoors right now?"

**🤖 AI Agent:**
> find_swimming_pools with covered: "yes" lists the indoor pools with hours; add open_now: "true" when the tool supports it for the moment-of-call check.

---

**👤 You:**
> "Tell me about the Luzhniki stadium."

**🤖 AI Agent:**
> find_stadiums with name: "Лужники" locates the arena; stadiums_wiki with detail: "true" adds the Wikipedia entry for the first listed stadium.


## ❓ FAQ

**Q: Do I need an API key?**
No. Every source is keyless and global: OpenStreetMap (Overpass + Nominatim) and Russian Wikipedia. The MCP defines no credentials.

**Q: Why does the Wikipedia roll matter for stadiums?**
OSM gives the location and the sport tags; Wikipedia carries the capacity, the opening year and the home club — none of which the map tags reliably hold.

**Q: Why are the counts bigger than the rows I get?**
Yes. OSM maps most large venues as areas (stadiums, monastery enclosures, university campuses), and every list tool uses the nwr selector, so nodes, ways and relations all count.

**Q: Can I find a gym near me?**
Pass lat + lon (and optionally km, 0.1–25) and the query narrows to a radius instead of the whole city. Do it before a long list — a citywide scan is capped at 200 rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moscow-sport-stadiums-pools-pitches](https://vinkius.com/en/ai-agent-connect/moscow-sport-stadiums-pools-pitches)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moscow Sport: Stadiums, Pools & Pitches** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moscow-sport-stadiums-pools-pitches` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moscow Sport: Stadiums, Pools & Pitches** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moscow-sport-stadiums-pools-pitches": {
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
