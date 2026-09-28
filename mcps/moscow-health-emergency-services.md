# Moscow Health & Emergency Services MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moscow-health-emergency-services)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Keyless Moscow emergency and health data: hospitals (with emergency departments), pharmacies and 24-hour ones, police and fire stations, plus a citywide safety profile.

## Description
Where to get help in Moscow, keyless, from OpenStreetMap — about 530 hospitals, 7,200 pharmacies, 940 police stations and 250 fire stations inside the city.

### What you can do
- **find_hospitals** — hospitals and clinical hospitals (about 530), filterable by emergency department, name fragment, open now and proximity
- **find_pharmacies** — the mapped pharmacies (about 7,200) with brand, phone and hours, filterable by chain and open now
- **find_pharmacies_open24** — the pharmacies whose mapped hours run around the clock (about 600) — for medicine at 3am
- **find_police_stations** — police stations and posts (about 940)
- **find_fire_stations** — fire stations (about 250)
- **safety_profile** — one call with citywide counts: hospitals total and with emergency, clinics, pharmacies total and 24-hour, police, fire and public defibrillators

### Who is this for
Residents and visitors with an urgent or practical question: the nearest emergency room, a pharmacy open now, or how well a district is covered.


## Available Tools (6)
- **find_fire_stations**: Each row carries the name (often a unit number, e.g. "ПСЧ № 1"), the operator and the centre coordinate. Filter by name fragment or by proximity to a point.

Find fire stations in Moscow
- **find_hospitals**: Each row carries the name, the phone, the emergency flag and the centre coordinate. Filter to emergency departments with emergency: "yes", or narrow by name fragment (e.g. "Боткин", "Склифосовского"). For neighbourhood clinics use the public-services MCP; for the nearest hospital around you pass lat/km.

Find hospitals in Moscow
- **find_pharmacies**: Each row carries the name, the brand/chain (e.g. "Аптека Ригла", "Эркафарм"), the phone and opening hours. Use open_now: "true" to keep only pharmacies open at the moment of the call, or brand to pick a chain. For 24-hour pharmacies use find_pharmacies_open24.

Find pharmacies in Moscow
- **find_pharmacies_open24**: Each row carries the name, brand, phone and coordinate. Use it for "where can I get medicine at 3am". The list reflects what the map records as 24/7; always call ahead for the chain's night window. Pass lat/km to search around a point.

Find 24-hour pharmacies in Moscow
- **find_police_stations**: Each row carries the name (often the unit number, e.g. "Отдел полиции № 2"), the phone and the centre coordinate. Filter by name fragment or by proximity to a point.

Find police stations in Moscow
- **safety_profile**: Public AEDs are barely mapped in Moscow (a handful of points) — treat that count as "not covered" rather than "not present". Use the profile to size a category before listing it with the other tools.

Citywide safety profile of Moscow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moscow Health & Emergency Services** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where is the nearest hospital with an emergency department?"

**🤖 AI Agent:**
> find_hospitals with emergency: "yes" and your lat/lon lists them by proximity; each row carries the phone and the coordinate.

---

**👤 You:**
> "Which pharmacies are open at 3am?"

**🤖 AI Agent:**
> find_pharmacies_open24 lists the pharmacies whose mapped hours run 24/7 — pass lat/lon to sort them around you, and call ahead for the chain’s night window.

---

**👤 You:**
> "How well is Moscow covered for emergency services?"

**🤖 AI Agent:**
> safety_profile answers in one call: citywide counts for hospitals, emergency hospitals, clinics, pharmacies, 24-hour pharmacies, police, fire and defibrillators.


## ❓ FAQ

**Q: Do I need an API key?**
No. Every source is keyless and global: OpenStreetMap (Overpass + Nominatim), Open-Meteo and Russian Wikipedia. The MCP defines no credentials.

**Q: In a real emergency, what should I do?**
Call 112 (the single emergency number in Russia), or 103 for an ambulance. Use this MCP to find where to go next, not to replace the call.

**Q: Why is the defibrillator count so low?**
Public AEDs are barely mapped in Moscow — only a handful of points. Treat that count as "not covered" on the map, not as absent from the city.

**Q: Can I find the nearest hospital around me?**
Pass lat + lon (and optionally km, 0.1–25) and the query narrows to a radius instead of the whole city. Use it before a long list — a citywide scan is heavy and capped at 200 rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moscow-health-emergency-services](https://vinkius.com/en/ai-agent-connect/moscow-health-emergency-services)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moscow Health & Emergency Services** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moscow-health-emergency-services` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moscow Health & Emergency Services** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moscow-health-emergency-services": {
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
