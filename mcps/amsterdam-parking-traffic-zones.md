# Amsterdam Parking & Traffic Zones MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/amsterdam-parking-traffic-zones)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless access to Amsterdam parking zones, individual parking bays, parking zone exceptions, emission (milieu) zones, zero-emission zones and touring car stops — the city's open-data platform, no API key.

## Description
The complete picture of where you can park — and where you cannot — in the city of Amsterdam, in one keyless integration. Data comes from the city's official DSO open-data platform.

### What you can do
- **Parking zones** — every parking zone as a polygon: zone name, domain code, geometry
- **Parking bays** — individual bays with street, neighbourhood, type and fiscal/non-fiscal category
- **Zone exceptions** — spots inside parking zones where rules are partially or temporarily exempted
- **Emission (milieu) zones** — where each vehicle class (vans, mopeds, taxis, tour buses, trucks) is restricted
- **Zero-emission zones** — where only zero-emission delivery trucks/vans and mopeds may enter
- **Touring car stops** — the designated coach/bus stops of the city

### Who is this for
Logistics and delivery operators planning routes around restricted zones, fleet managers checking which zone applies to a delivery address, and mobility analysts.


## Available Tools (6)
- **list_parking_zones**: Useful to check which zone a location falls under.

List Amsterdam parking zones (parkeerzones)
- **list_parking_zone_exceptions**: g. permit validity windows), validity dates, usage goal and whether the exception is publicly visible.

List parking zone exceptions (uitzonderingen)
- **list_parking_bays**: g. Langs = parallel), category (fiscal or non-fiscal), count, version date, regimes and polygon geometry (EPSG:28999).

List individual parking bays (parkeervakken)
- **list_milieu_zones**: Vehicle classes: bestelbus (light delivery van), bromensnorfiets (mopeds), taxi, touringcar (touring bus) or vrachtauto (truck). Each row has the vehicle class and the effective-from date.

List emission (milieu) zones per vehicle class
- **list_zero_emission_zones**: List zero-emission zones (uitstootvrije zones)
- **list_touring_car_stops**: g. H7: Spui), nearest location, number of stops and point geometry (EPSG:28999).

List touring car (coach/bus) stops in Amsterdam


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amsterdam Parking & Traffic Zones** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which parking zones exist in the West part of Amsterdam?"

**🤖 AI Agent:**
> 🅿️ **Parking zones**

The zone named West 6 and other West zones, each as a MultiPolygon (EPSG:28999) with its domain code. Match the polygon against your address to see the rules that apply.

---

**👤 You:**
> "Where is the zero-emission zone for delivery trucks?"

**🤖 AI Agent:**
> The vracht_en_bestelauto zero-emission zone is returned as polygons (EPSG:28999) — areas inside which only zero-emission delivery and truck vehicles may drive.

---

**👤 You:**
> "List the touring car stops in the city centre."

**🤖 AI Agent:**
> 🚌 **Touring car stops**

Designated coach stops such as "H7: Spui" (Nieuwezijds Voorburgwal 355), each with its stop count and point geometry (EPSG:28999).


## ❓ FAQ

**Q: Do I need an API key?**
No. The parkeerzones, parkeervakken, milieuzones, uitstootvrije_zones and touringcars services of the city's DSO open-data platform are public (OPENBAAR) and work without credentials.

**Q: What are the coordinates in?**
All geometries are in EPSG:28999 (RD New, the Dutch national coordinate system, metres). Convert to WGS84 latitude/longitude before plotting on most world maps.

**Q: Can I check whether my street has public parking bays?**
Yes. list_parking_bays filters by street name (straatnaam) or neighbourhood code (buurtcode) and returns each bay's type (e.g. Langs = parallel parking), fiscal/non-fiscal category and count.

**Q: What vehicle classes does the emission zone tool cover?**
list_milieu_zones covers bestelbus (light delivery vans), bromensnorfiets (mopeds), taxi, touringcar (tour buses) and vrachtauto (trucks). list_zero_emission_zones covers vracht_en_bestelauto (delivery trucks/vans) and brom_en_snorfiets (mopeds/scooters).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/amsterdam-parking-traffic-zones](https://vinkius.com/en/ai-agent-connect/amsterdam-parking-traffic-zones)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amsterdam Parking & Traffic Zones** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amsterdam-parking-traffic-zones` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amsterdam Parking & Traffic Zones** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amsterdam-parking-traffic-zones": {
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
