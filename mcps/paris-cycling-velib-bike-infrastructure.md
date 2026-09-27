# Paris Cycling: Vélib’ & Bike Infrastructure MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paris-cycling-velib-bike-infrastructure)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless Paris cycling data: live Vélib’ station availability, the bike-lane network, bicycle & multimodal traffic counters with their readings, and the cumulative km of bike infrastructure.

## Description
Everything the City of Paris publishes about cycling — the live Vélib’ fleet, the protected-lane network and the counting programme — keyless, from opendata.paris.fr.

### What you can do
- **list_velib_stations** — the Vélib’ bike-share stations in live availability form: station code/name, arrondissement, whether it is renting, bikes and e-bikes currently available; filter by arrondissement and by minimum bikes/e-bikes
- **list_bike_lanes / bike_lanes_summary** — the protected two-wheel lane segments (type of amenagement, speed cap, export year) and the network summarised by type and year
- **bike_network_length** — the cumulative kilometres of two-wheel infrastructure per year (the annee filter)
- **list_bike_counters / bike_counter_daily_counts** — the fixed bicycle counters (by installation year or name) and the hourly reading series of one counter over a lookback window (days, default 14, max 90)
- **multimodal_counter_sites / multimodal_counts** — the multimodal counting sites (bike/pedestrian/bus) by voie type, and the hourly counts at one site per mode over a window (days, default 3, max 30)

### Who is this for
Route planners comparing bike options across Paris, anyone sizing a bike counter before a study, or reading how the city's cycle network grows year over year. Vélib’ availability updates frequently — treat it as a snapshot, not a guarantee. Counting series are hour-granular: sum the window's rows for a daily figure. Text filters are exact matches; page with limit (max 100) and offset.


## Available Tools (8)
- **bike_counter_daily_counts**: g. "100003096-353242251") over a lookback window on the reading date (days defaults to 14, max 90). Each row is one hour, with the counter name, the timestamp and the count of cyclists that hour (sum_counts can be null for a missing reading). A full day is 24 rows, so a 14-day window is up to 336 rows — page with limit/offset (100 rows max per call). Sum the window's rows for a daily/total figure.

Get daily bike counts for one counter
- **bike_lanes_summary**: Use it to describe the network ("about 47,000 dedicated bike lanes, 36,000 two-way cycling streets, ...") and to pick an exact amenagement value for list_bike_lanes.

Summarize the Paris bike-lane network by type and export year
- **bike_network_length**: Use it to answer "how long is the bike network / how much did it grow". The annee filter is the snapshot year as a string, e.g. "2024"; without it every snapshot is returned (12 rows, one page).

Report the cumulative km of Paris bike infrastructure
- **list_bike_counters**: g. "Totem 64 Rue de Rivoli O-E"), the installation year and the coordinates. Use it to discover a counter before asking for its daily counts in bike_counter_daily_counts, or to answer "where does the city count cyclists". The year filter is the installation year as a string, e.g. "2023". Page with limit/offset (100 rows max per call — the list spans two pages).

List bicycle traffic counters in Paris
- **list_bike_lanes**: Use it to answer "is there a bike lane on street X". Filters are exact stored values: amenagement is "piste cyclable", "double-sens cyclable simple", "voie piétonne", "couloir bus ouvert aux vélos", "bande cyclable", "voie verte", "vélorue" or a closed lane; arrondissement is the plain number "1".."20"; bois is "oui" (the two city woods) or "non"; date_export is the export year, "2026" is the current one; vitesse_maximale_autorisee is "30 km/h", "50 km/h", "20 km/h", "15 km/h", "10 km/h", "au pas" or "non définie". Page with limit/offset (100 rows max per call).

List Paris bike-lane segments
- **list_velib_stations**: Each station has its code, name, installed flag, dock capacity, the available docks, the available bikes (conventional + e-bike counts), the mechanical-breakdown count, the renting/returning flags, the data timestamp and the commune it sits in. Use it to answer "where is a bike nearby I can rent". Filters are exact stored values: commune is the commune name, "Paris" (about 1,000 stations), "Créteil", "Boulogne-Billancourt", "Clichy" or similar (accent matters); is_renting / is_returning / is_installed are "OUI" or "NON" (uppercase); min_bikes and min_ebikes keep stations with at least that many available conventional bikes / e-bikes. Page with limit/offset (100 rows max per call).

List Vélib' bike-share stations with live availability
- **multimodal_counter_sites**: Use it to discover a site before asking for its hourly mode split in multimodal_counts, or to answer "where does the city count pedestrians and cyclists". The voie filter is exact: "Piste cyclable", "Coronapiste", "Voie Bus" or "Voie de circulation générale". Page with limit/offset (100 rows max per call).

List multimodal traffic counting sites in Paris
- **multimodal_counts**: g. "10136") over a lookback window on the reading timestamp (days defaults to 3, max 30). Each row is one hour with the observed mode, the user count for that hour, the street and direction. Use it to answer "how many cyclists / pedestrians / buses pass this street". Without a site id the window spans every site (100 rows per page) — pick a site first for a coherent series. The mode filter is exact: "Vélos", "Piétons", "Autobus et autocars", "Trottinettes" or "2 roues motorisées". Page with limit/offset (100 rows max per call).

Get hourly multimodal counts at a site


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paris Cycling: Vélib’ & Bike Infrastructure** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which Vélib’ stations in the 6th have at least 3 free e-bikes?"

**🤖 AI Agent:**
> list_velib_stations with commune: "6" and min_ebikes: "3" returns the stations in the 6th arrondissement with at least 3 e-bikes available right now; add min_bikes to require classic bikes too.

---

**👤 You:**
> "How many cyclists pass the Pont de Sèvres on a typical day?"

**🤖 AI Agent:**
> list_bike_counters with name set to the counter's stored name (or find the counter id via its installation year) locates the counter; bike_counter_daily_counts with that counter and days: "14" returns the last two weeks of hourly readings — sum the rows per day for daily figures.

---

**👤 You:**
> "Which streets count pedestrians as well as cyclists, and how?"

**🤖 AI Agent:**
> multimodal_counter_sites lists the multimodal counting sites (bike, pedestrian, bus, e-scooter) with their voie and trajeto; multimodal_counter_sites + multimodal_counts at one site (site id) over days: "30" returns the hourly counts split by mode.


## ❓ FAQ

**Q: Do I need an API key?**
No. opendata.paris.fr serves all city datasets anonymously over its Opendatasoft REST API. This MCP defines no credentials and needs nothing configured.

**Q: Is the Vélib’ data real-time?**
list_velib_stations reads the live availability dataset (stations currently renting, bikes and e-bikes available now). It refreshes on the platform's schedule — treat the result as a current snapshot, not a guarantee of stock when you arrive.

**Q: How do I size a counter for a study?**
list_bike_counters shows the installed counters (by year or name); bike_counter_daily_counts then returns one counter's hourly readings over up to 90 days. For pedestrians, buses and e-scooters use multimodal_counter_sites + multimodal_counts (up to 30 days), which split counts by mode.

**Q: Can I see how the bike network is growing?**
bike_network_length reports the cumulative km of two-wheel infrastructure per year (filter with annee), and bike_lanes_summary breaks the exported segments down by type and export year — put the two together to track growth.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paris-cycling-velib-bike-infrastructure](https://vinkius.com/en/ai-agent-connect/paris-cycling-velib-bike-infrastructure)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paris Cycling: Vélib’ & Bike Infrastructure** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paris-cycling-velib-bike-infrastructure` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paris Cycling: Vélib’ & Bike Infrastructure** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paris-cycling-velib-bike-infrastructure": {
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
