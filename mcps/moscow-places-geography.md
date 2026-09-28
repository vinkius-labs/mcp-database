# Moscow Places & Geography MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moscow-places-geography)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [geospatial](../categories/geospatial.md)

Keyless Moscow geography: place and address search, structured and reverse geocoding, citywide OSM point-of-interest densities and the official city boundary.

## Description
Where things are in Moscow, keyless, from OpenStreetMap — the city’s own data portals refuse connections from outside Russia, so this family is built on globally reachable sources only.

### What you can do
- **search_places** — free-text search for places, streets and addresses inside the Moscow viewbox (Russian names match best)
- **geocode_address** — structured geocode of a street + house number against the city (Москва by default)
- **reverse_geocode** — the address at a coordinate inside Moscow
- **poi_densities** — one call with citywide counts for 14 classes: hospitals, pharmacies, supermarkets, cafes, museums, metro stations, parks and more
- **moscow_boundary** — the OSM record of Moscow itself (relation 102269): names in several languages, ISO 3166-2 code, population, area and centroid
- **moscow_districts** — the 125 districts and 10 administrative okrugs of the city, listed from Russian Wikipedia

### Who is this for
Anyone locating things in Moscow: visitors planning a route, expats decoding a Cyrillic address, or an app that needs coordinates for a Moscow place.


## Available Tools (6)
- **geocode_address**: Pass the street with the house number, e.g. "улица Арбат, 10" or "Tverskaya 1"; the city defaults to "Москва". Returns the matched locations with coordinates and the parsed address parts (road, house number, district, postcode).

Geocode a Moscow street address
- **moscow_boundary**: Use it to anchor coordinates or to name the city in another language. There is exactly one such relation — the 125 city districts are not mapped in OSM (use moscow_districts for those).

Get the Moscow city boundary record
- **moscow_districts**: OpenStreetMap does not map them, so this tool lists them from Russian Wikipedia: pass category "districts" (Категория:Районы Москвы — the 125 districts), "okrugs" (Категория:Административные округа Москвы — the 10 okrugs). Each entry is a page title; use search_places or the culture tools to locate a district on the map.

List the districts and okrugs of Moscow
- **poi_densities**: 4–56.3 N, 37.0–38.6 E — the city plus its immediate ring): hospitals, pharmacies, supermarkets, cafes, post offices, museums, libraries, theatres, police stations, metro stations, bus stops, EV charging and fuel stations and parks. Counts include mapped areas as well as points. Use it to size a category before listing it ("how many museums does Moscow have") or to compare neighbourhoods by combining it with a proximity filter from the other tools.

Count mapped points of interest across Moscow
- **reverse_geocode**: Use it after a proximity search ("what is at these coordinates") or to name a point picked on a map. Coordinates are decimal degrees (Moscow is roughly lat 55.4–56.3, lon 37.0–38.6).

Reverse-geocode a coordinate in Moscow
- **search_places**: Use it for "where is the Tretyakov Gallery", "Arbat street", "Metro station Sokolniki". Each result carries the display name, the OSM category/type, the latitude/longitude and the parsed address. Text is matched as typed — Russian names work best ("аптека", "музей"); English names work when the map carries them.

Search for places and addresses in Moscow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moscow Places & Geography** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where is the Tretyakov Gallery, and what district is it in?"

**🤖 AI Agent:**
> search_places with the Russian name returns its coordinates and address; reverse_geocode of that point names the containing district.

---

**👤 You:**
> "How well is Moscow mapped — how many hospitals, museums and metro stations?"

**🤖 AI Agent:**
> poi_densities answers in one call: 14 classes with their citywide counts, areas included.

---

**👤 You:**
> "Geocode “улица Арбат, 10” for me."

**🤖 AI Agent:**
> geocode_address with that street returns the matches with display name, latitude and longitude; search_places also finds Arbat street itself.


## ❓ FAQ

**Q: Do I need an API key?**
No. Every source is keyless and global: OpenStreetMap (Overpass + Nominatim), Open-Meteo and Russian Wikipedia. The MCP defines no credentials.

**Q: Why not the city’s own open-data portal?**
Moscow's own portals (data.mos.ru, api.mos.ru, transport.mos.ru) resolve but refuse connections from outside Russia, so this family never depends on them. Coverage comes from the global OSM project, which maps the city in fine detail.

**Q: Why do counts include areas, not just points?**
Yes. OSM maps most large venues as areas (buildings, park outlines), and every tool uses the nwr selector, so nodes, ways and relations all count. Point-only queries would miss them.

**Q: Can I search around a point instead of the whole city?**
Pass lat + lon (and optionally km, 0.1–25) and the query narrows to a radius instead of the whole city. Use it before a long list — a citywide scan is heavy and capped at 200 rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moscow-places-geography](https://vinkius.com/en/ai-agent-connect/moscow-places-geography)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moscow Places & Geography** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moscow-places-geography` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moscow Places & Geography** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moscow-places-geography": {
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
