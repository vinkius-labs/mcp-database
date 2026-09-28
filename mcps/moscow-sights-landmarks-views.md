# Moscow Sights, Landmarks & Views MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moscow-sights-landmarks-views)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Keyless Moscow sightseeing: attractions, viewpoints and fountains with a walking-distance list of the nearest sights, plus the curated Wikipedia landmark roll.

## Description
Moscow for a visitor, keyless — about 1,500 attractions, 90 viewpoints and 230 fountains mapped, plus a ready-made walking list and the Wikipedia landmark roll.

### What you can do
- **find_attractions** — attractions (about 1,500) filtered by name, free-or-paid and open now, with hours and coordinates
- **find_viewpoints** — viewpoints and panorama platforms — from Sparrow Hills to the Ostankino decks
- **find_fountains** — fountains and water features (about 230), from the VDNKH fountains to the river park
- **sights_nearby** — a walking-distance shortlist: attractions, viewpoints and artworks within a radius, sorted by distance from your coordinate
- **moscow_landmarks** — the curated Russian Wikipedia roll of Moscow landmarks, with a short encyclopaedia entry for the first
- **tourism_profile** — citywide counts of attractions, viewpoints, artworks, fountains, museums and theatres in one call

### Who is this for
Visitors with a free afternoon and residents showing someone around: what to see within a 2 km walk, what is open, and what Wikipedia says about it.


## Available Tools (6)
- **find_attractions**: Each row carries the name, description, opening hours, fee flag and centre coordinate. Filter by name fragment (e.g. "Парк", "ВДНХ"), keep only what is open right now with open_now: "true", or narrow to a neighbourhood with lat/lon/km. For museums and theatres use the culture MCP; this tool is the broader list of things worth seeing.

Find Moscow attractions and sights
- **find_fountains**: Filter by name fragment (e.g. "Похищение", "Дружбы") or narrow to a neighbourhood with lat/lon/km. Drinking-water springs are a separate amenity and are not included here.

Find Moscow fountains and water features
- **find_viewpoints**: Each row carries the name, description and coordinate. Filter by name fragment or narrow to a neighbourhood with lat/lon/km. Pair with the geography MCP to reverse-geocode what you see from the top.

Find Moscow viewpoints and panorama platforms
- **moscow_landmarks**: Pass detail: "true" to fetch the summary of the first landmark; otherwise the tool returns the plain title list.

Notable Moscow landmarks from Russian Wikipedia
- **sights_nearby**: Requires lat and lon. Use it to answer "what can I see within a 2 km walk from here?" — then call find_attractions for full details on any one of them.

List the nearest Moscow sights within walking distance
- **tourism_profile**: Use it to size the city for planning ("how many mapped fountains are there in Moscow?") without paging through lists. No filters — this is a profile, not a search.

Citywide Moscow sightseeing profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moscow Sights, Landmarks & Views** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What can I see within a 2 km walk from Red Square?"

**🤖 AI Agent:**
> sights_nearby with the Red Square coordinates and km: "2" returns the ranked shortlist with distance per sight.

---

**👤 You:**
> "Are there any free attractions open right now?"

**🤖 AI Agent:**
> find_attractions with fee: "no" and open_now: "true" keeps only the free ones that are open at the moment of the call.

---

**👤 You:**
> "How many fountains are there in Moscow?"

**🤖 AI Agent:**
> tourism_profile returns the citywide fountain count (the map records about 230) alongside attractions, viewpoints and museums in one call.


## ❓ FAQ

**Q: Do I need an API key?**
No. Every source is keyless and global: OpenStreetMap (Overpass + Nominatim) and Russian Wikipedia. The MCP defines no credentials.

**Q: How is this different from the culture MCP?**
The culture MCP covers museums, theatres and libraries in depth. This one is the broader list of things worth seeing — attractions, viewpoints, fountains and street art — plus a distance-sorted walking shortlist.

**Q: Why are the counts bigger than the rows I get?**
Yes. OSM maps most large venues as areas (stadiums, monastery enclosures, university campuses), and every list tool uses the nwr selector, so nodes, ways and relations all count.

**Q: Can I find sights near a point?**
Pass lat + lon (and optionally km, 0.1–25) and the query narrows to a radius instead of the whole city. Do it before a long list — a citywide scan is capped at 200 rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moscow-sights-landmarks-views](https://vinkius.com/en/ai-agent-connect/moscow-sights-landmarks-views)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moscow Sights, Landmarks & Views** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moscow-sights-landmarks-views` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moscow Sights, Landmarks & Views** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moscow-sights-landmarks-views": {
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
