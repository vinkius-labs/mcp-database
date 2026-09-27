# NYC Parks, Trees & Street Life MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-parks-trees-street-life)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless NYC day-to-day city data: parks and recreation events, individual street trees with risk ratings, EV charging stations and sessions, monthly sanitation tonnage, recycling bins and litter baskets — no API key.

## Description
The city's day-to-day physical-infrastructure datasets, keyless, for local planning and quick lookups.

### What you can do
- **Parks & recreation events** — program events across the city's parks with dates, titles and categories
- **Street trees** — individual trees with species, trunk size, structure and condition ratings, and risk
- **EV charging** — public and private charging stations (type, ports, borough/street) plus actual charging sessions with energy in kWh
- **Sanitation tonnage** — monthly waste collected by borough: refuse, paper, MGP organics and recycling streams
- **Recycling bins** — DSNY bin sites with paper/MGP bin counts by zone and district
- **Litter baskets** — the city's litter-basket register by street, borough and basket type

### Who is this for
Resident and visitor services, local events planning, greening and EV planning, and any agent that needs a quick, official fact about the physical city around a given address.


## Available Tools (7)
- **get_sanitation_tonnage**: month is the calendar month in "YYYY-MM" form. Without a borough it returns every borough for that month.

DSNY waste collection tonnage by month and borough
- **list_ev_charging_stations**: Filter by agency, borough, street or public-availability flag.

List NYC electric vehicle charging stations
- **list_litter_baskets**: Filter by basket type, borough or street.

List NYC litter basket locations by street and borough
- **list_parks_events**: Filter by park name, category or a start-time window. Registration links and description are included when the park publishes them.

List NYC Parks events (fitness classes, tours, programs)
- **list_recycling_bins**: Filter by DSNY zone, district or site type.

List curbside recycling bin locations by DSNY zone/district
- **search_ev_charging_sessions**: Filter by station name, location name, a charge-date window or session status.

Search EV charging session records (energy delivered per session)
- **search_forestry_trees**: Filter by object id, species or risk rating. These are managed/planted trees, not the full street-tree inventory.

Search NYC Forestry program tree points (planted & protected trees)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Parks, Trees & Street Life** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's on at Prospect Park this weekend?"

**🤖 AI Agent:**
> list_parks_events with park "Prospect Park" and start_after the weekend date returns the scheduled program events.

---

**👤 You:**
> "How many EV charging stations are on 8th Ave?"

**🤖 AI Agent:**
> list_ev_charging_stations with street "8th Ave" and public_only "Yes" returns the public stations there with charger type and port counts; search_ev_charging_sessions with a station name shows real usage.

---

**👤 You:**
> "How much waste does Brooklyn collect in a month?"

**🤖 AI Agent:**
> get_sanitation_tonnage with month "2026-08" and borough "Brooklyn" returns that month's refuse, paper, MGP-organics and recycling tonnage for the borough.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: How fresh is this data?**
Each set updates on its own cycle: events as the parks program calendar changes, tree attributes from the annual inventory, EV sessions continuously, and sanitation tonnage by month. The response always carries the row's own date fields, so you can see exactly how recent each fact is.

**Q: Can I look things up by address?**
Yes, within each tool's scope: EV stations and litter baskets by street name and borough; recycling bins by DSNY zone/district and site location; trees by object id or species; events by park name.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-parks-trees-street-life](https://vinkius.com/en/ai-agent-connect/nyc-parks-trees-street-life)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Parks, Trees & Street Life** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-parks-trees-street-life` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Parks, Trees & Street Life** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-parks-trees-street-life": {
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
