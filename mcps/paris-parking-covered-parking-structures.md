# Paris Parking: Covered Parking Structures MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paris-parking-covered-parking-structures)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless Paris parking data: the 125 covered parking structures (parkings en ouvrages) of Paris — capacity, PMR/bike/shared-mobility places, per arrondissement.

## Description
The 125 covered parking structures (parkings en ouvrage) of Paris — keyless, straight from the Paris open-data platform (opendata.paris.fr).

### What you can do
- **list_parking_garages / parking_garage_lookup / count_parking_garages** — the 125 structures: name (stored uppercase, e.g. "INVALIDES"), arrondissement INSEE, address, user type ("abonnés" / "tous"), place counts (total, standard, PMR, bicycle, shared-mobility, carpool), height limit, operator SIRET and WGS84 coordinates
- **pmr_garages / bike_garages / shared_mobility_garages** — the structures with at least one place in each category (integer >= 1 filters), optionally in one arrondissement
- **parking_capacity_overview** — the city-wide sums: structures, total places, standard, PMR, bicycle and shared-mobility places

### Who is this for
Anyone locating a parking structure by name or arrondissement, counting accessible or bike-friendly capacity, or benchmarking the city's underground parking stock. The whole dataset (125 rows) fits in two calls; structure names are stored uppercase without accents — use list_parking_garages to discover the exact stored form. Every structure is paid (the gratuit flag is 0 everywhere) and the electric-vehicle column is null across the dataset, so neither is exposed as a filter.


## Available Tools (7)
- **list_parking_garages**: Each row has: the name (nom, stored in uppercase, e.g. "INVALIDES" or "FREMICOURT"), the arrondissement INSEE code (insee, "75101".."75120" plus one suburban "94080" entry), the street address, who it serves (type_usagers: "abonnés" for reserved-only, "tous" for open to all), the free/paid flag (gratuit: 1 = free — currently every structure is paid, so 0), the place counts (nb_places total, nb_pr standard places, nb_pmr handicap-accessible places, nb_velo bicycle places, nb_autopartage shared-mobility places, nb_covoit carpool places, all integers), the optional height limit (hauteur_max, meters), the operator SIRET (num_siret) and WGS84 coordinates (xlong / ylat). The whole dataset fits in two calls; page with limit/offset (100 rows max per call).

List the covered parking structures (parkings en ouvrage) in Paris
- **parking_capacity_overview**: Null counts are treated as zero. No parameters.

Sum the parking capacity of all covered structures in Paris
- **parking_garage_lookup**: g. "OPERA", "INVALIDES" or "GREMILLET". Names are stored in uppercase without accents; use the stored form from list_parking_garages when unsure. Optionally restrict to one arrondissement (insee). Returns 0, 1 or a few rows with the full place counts, address, user type and coordinates.

Find parking structures by name
- **pmr_garages**: Optionally restrict to one arrondissement (insee). Each row keeps the full place breakdown so you can see how many PMR places each structure offers next to its total capacity.

List parking structures with accessible (PMR) places
- **bike_garages**: Optionally restrict to one arrondissement (insee). Each row keeps the full place breakdown so you can see the bicycle places next to the total capacity.

List parking structures with bicycle places
- **count_parking_garages**: "75120") and type_usagers ("abonnés" / "tous") — the same exact-match filters as list_parking_garages. A fast total count; use it to compare structure counts between arrondissements.

Count parking structures, optionally by arrondissement or user type
- **shared_mobility_garages**: Optionally restrict to one arrondissement (insee).

List parking structures with shared-mobility places


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paris Parking: Covered Parking Structures** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many PMR places does the 7th arrondissement offer?"

**🤖 AI Agent:**
> Run pmr_garages with insee "75107" — each row carries nb_pmr (the accessible places per structure); parking_capacity_overview gives the city-wide PMR total for context.

---

**👤 You:**
> "Which parking structures have bicycle places?"

**🤖 AI Agent:**
> Call bike_garages — it lists every structure with nb_velo >= 1, with the full place breakdown; add insee to restrict to one arrondissement.

---

**👤 You:**
> "How many places does the city park in total, and how many are shared-mobility?"

**🤖 AI Agent:**
> parking_capacity_overview returns all five sums in one call — total_places alongside shared_mobility_places, standard, PMR and bicycle totals.


## ❓ FAQ

**Q: Do I need an API key?**
No. opendata.paris.fr serves all city datasets anonymously over its Opendatasoft REST API. This MCP defines no credentials and needs nothing configured.

**Q: Why are all the structures paid?**
The gratuit flag is 0 on every one of the 125 rows — the city currently has no free covered structure. Free surface parking (parkings de surface) is a separate dataset not covered by this MCP.

**Q: What do the place-count columns mean?**
nb_places is the total, nb_pr the standard places, nb_pmr the handicap-accessible places, nb_velo the bicycle places, nb_autopartage the shared-mobility places and nb_covoit the carpool places. All are integers; the PMR, bike and shared-mobility tools apply a >= 1 filter on the relevant column.

**Q: Does insee always mean a Paris arrondissement?**
Mostly: "75101".."75120" are the 20 arrondissements, but one structure sits in Saint-Denis ("94080"). Filter by the "751xx" codes when you only want Paris proper.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paris-parking-covered-parking-structures](https://vinkius.com/en/ai-agent-connect/paris-parking-covered-parking-structures)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paris Parking: Covered Parking Structures** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paris-parking-covered-parking-structures` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paris Parking: Covered Parking Structures** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paris-parking-covered-parking-structures": {
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
