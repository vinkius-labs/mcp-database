# RATP Stations: Ridership & Network Amenities MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ratp-stations-ridership-network-amenities)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless RATP network data: metro/RER station annual ridership rankings, public restrooms, water fountains, AED defibrillators and approved proximity shops at stations, hourly air quality at 7 stations, and the La Défense peak-smoothing experiment.

## Description
Station-level knowledge about the RATP network (Paris metro + RER) — keyless, from data.ratp.fr.

### What you can do
- **station_ridership_ranking** — the annual entry ridership of the network's stations ranked (top_n, filter by reseau "Métro"/"RER")
- **get_station_ridership** — one station's annual ridership rows
- **list_restrooms / list_water_fountains / list_defibrillators** — the amenities inside the network, filterable by line, PMR/free access, postal code and availability
- **list_station_shops** — the approved proximity shops located near stations (by trade type and commune)
- **air_quality_station** — hourly air-quality readings at one metro/RER station (station is one of: chatelet, auber, franklin-d-roosevelt, saint-germain-des-pres, iena, nation, luxembourg), over a lookback window
- **la_defense_peak_smoothing** — the La Défense peak-smoothing experiment rows (type_jour: weekday/weekend)

### Who is this for
Network planners and visitors: where is the busiest station, where can a visitor find a toilet or water inside the network, and how is the air where they board. Ridership figures are annual aggregates; air-quality rows are hourly and the station list is fixed to the 7 monitored stations. Text filters are exact matches; page with limit (max 100) and offset.


## Available Tools (8)
- **station_ridership_ranking**: Each row has the station name, its network, the yearly entry count, up to five corresponding lines and, for Paris stations, the arrondissement. The rank is computed within each network, so without a network filter the top-N mixes the top-N metro and top-N RER stations. Use it to answer "which station is busiest". The reseau filter is "Métro" or "RER"; top_n is how many rows to return (default 20, max 100).

Rank Paris metro/RER stations by annual entry ridership
- **list_station_shops**: Use it to answer "what convenience shops supply the metro network". The trade filter (type) is an exact stored value: "café tabac" (the large majority), "tabac loto", "tabac presse", "tabac", "civette", "librairie", "tabac librairie", "presse", "café", "boulangerie" or "presse tabac". Page with limit/offset (100 rows max per call).

List approved proximity shops near RATP stations
- **air_quality_station**: Each row has the timestamp and the station's pollutants: NO2, NO, the 10 and 25 µg/m³ fractions, the CO2 level, temperature and relative humidity (the field names are per-station suffixes, e.g. nocha4 / 10cha4 / c2cha4 / tcha4 / hycha4 at Châtelet). Values are text: numbers are in µg/m³, "<2" means below the 2 µg/m³ sensor floor, "ND" means the sensor was out of service, and temperature/humidity use a comma decimal (22,2). Some stations lag: Châtelet, Auber and Franklin D. Roosevelt series start in 2021, Saint-Germain in 2024, Iéna in 2025, Nation and the Luxembourg gate carry shorter series — a window may return fewer rows than requested. The station parameter picks the dataset: chatelet, auber, franklin-d-roosevelt, saint-germain-des-pres, iena, nation or luxembourg. Page with limit/offset (100 rows max per call).

Get hourly air quality at a metro/RER station
- **get_station_ridership**: The name must match the stored value: uppercase, the station sign, e.g. "MONTPARNASSE-BIENVENUE", "SAINT-LAZARE", "CHATELET-LES HALLES-RER", "GARE DE LYON". Use station_ridership_ranking to discover the exact names. Each row has the network, the yearly entry count, the station rank within its network and the arrondissement (for Paris stations).

Get the annual ridership of one station
- **la_defense_peak_smoothing**: The experiment compared two day types: "DIJFP" (a regular day, about 110k daily entries) and "JOHV" (a day with the evening peak softened, about 380k–400k entries). Use it to compare hub frequencies between the two day types. The type filter is exact: "JOHV" or "DIJFP". Page limit/offset (100 rows max per call).

Get the La Défense peak-smoothing experiment data
- **list_defibrillators**: g. "Métro 3 Bourse", "RER A TORCY"), the commune, the coordinates and the availability flags. Use it to answer "is there a defibrillator at station X". Filters are exact stored values: com_nom is the commune, "PARIS" (about 315) or a suburb; dispo_i is "7j/7" (available every day); acc is "Intérieur" or "Extérieur"; line matches the access location text prefix, e.g. "Métro" or "RER A" — pass it to the location param. Page with limit/offset (100 rows max per call).

List AED defibrillators in the RATP network
- **list_restrooms**: Use it to answer "where is a public toilet on line X / near station Y". Filters are exact stored values: ligne is "A", "B" or a metro line "1","3","5","6","7","8","11","12","13","14"; pmr is "oui" (fully accessible); free is "gratuit" or "payant"; in_controlled_zone is "oui"/"non". Page with limit/offset (100 rows max per call).

List public restrooms inside the RATP network
- **list_water_fountains**: Use it to answer "where can I drink water in the metro". Filters are exact stored values: ligne is "A", "B" or a metro line, e.g. "1", "14"; postal_code is the 5-digit code, e.g. "75003". Page with limit/offset (100 rows max per call).

List water fountains in the RATP network


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RATP Stations: Ridership & Network Amenities** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which is the busiest metro station in Paris?"

**🤖 AI Agent:**
> station_ridership_ranking with reseau: "Métro" and top_n: "5" returns the five metro stations with the highest annual entry ridership; widen top_n or switch reseau to "RER" for the RER ranking.

---

**👤 You:**
> "Where can I find a free restroom inside the metro network, on line 1?"

**🤖 AI Agent:**
> list_restrooms with ligne: "M1" and free: "oui" returns the network restrooms on line 1 that are free, with their location and PMR access flags.

---

**👤 You:**
> "How is the air quality at Châtelet today?"

**🤖 AI Agent:**
> air_quality_station with station: "chatelet" and days: "1" returns the last 24 hourly readings (pollutants and index values) at the Châtelet station; a bigger days value widens the window (100 rows per page).


## ❓ FAQ

**Q: Do I need an API key?**
No. data.ratp.fr serves all RATP datasets anonymously over its Opendatasoft REST API. This MCP defines no credentials and needs nothing configured.

**Q: Which stations have air-quality data?**
Seven monitored metro/RER stations: chatelet, auber, franklin-d-roosevelt, saint-germain-des-pres, iena, nation and luxembourg. air_quality_station returns the hourly readings at one of them over a lookback window; any other station name is rejected with the list of valid values.

**Q: Are the ridership figures current?**
They are annual aggregates published by RATP, not live counts. station_ridership_ranking and get_station_ridership read the published per-station annual entry figures; use them for comparisons, not for today's occupancy.

**Q: What is the La Défense peak-smoothing experiment?**
A transport-demand management experiment at the La Défense business district shifting morning peaks; la_defense_peak_smoothing returns its published rows, filterable by type_jour (weekday vs weekend).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ratp-stations-ridership-network-amenities](https://vinkius.com/en/ai-agent-connect/ratp-stations-ridership-network-amenities)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RATP Stations: Ridership & Network Amenities** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ratp-stations-ridership-network-amenities` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RATP Stations: Ridership & Network Amenities** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ratp-stations-ridership-network-amenities": {
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
