# Paris Waste: TriLibre Stations & Per-Capita Streams MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paris-waste-trilibre-stations-per-capita-streams)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless Paris waste data: the 438 voluntary-drop (TriLibre) collection stations by address and arrondissement, plus the per-capita waste-stream series 2019–2024 with year-over-year deltas.

## Description
Paris's waste infrastructure and its per-capita waste streams — keyless, straight from the Paris open-data platform (opendata.paris.fr).

### What you can do
- **list_trilib_stations / trilib_station_lookup / count_trilib_stations** — the 438 voluntary-drop stations: code, street address, arrondissement postal code and equipment status; the whole city or one arrondissement at a time
- **waste_per_capita** — one year's rows for the five waste streams (glass packaging, multi-material, bio-waste, occasional waste, residual household waste), optionally one stream; quantities in kg per inhabitant per year
- **waste_history** — a stream's 2019–2024 series with the computed first-to-last-year delta, or all five streams side by side
- **waste_types_overview** — the preset facets: the exact stored stream labels (with their emoji) and the year span, so you can discover the filter values

### Who is this for
Sustainability dashboards, journalism on recycling performance, and anyone looking for where to drop waste in a given street. The stream filter matches the letters-only core, so "verre" finds the stored "Emballages en verre"; the annee column is date-typed and the tools window it automatically.


## Available Tools (6)
- **list_trilib_stations**: Each row has the station code (identifiant, 4 digits, e.g. "4618"), the street address (adr), the arrondissement postal code (arrdt, "75001".."75020") and the equipment status (emplacement_statut, stored as "Mobilier en service" for the current fleet). Use it to answer "where is a waste drop point near …" — filter by arrdt for one arrondissement. Page with limit/offset (100 rows max per call).

List the Paris voluntary-drop waste collection stations (TriLibre)
- **count_trilib_stations**: "75020"). A fast total count — the city-wide total is 438.

Count waste stations, optionally by arrondissement
- **trilib_station_lookup**: g. "4618"): street address, arrondissement postal code and status. identifiant is required; codes are 4-digit numbers as seen in list_trilib_stations.

Look up a waste station by its code
- **waste_history**: The type parameter matches the letters-only core of the stored emoji-labeled stream names (e.g. "verre" -> "♻️ Emballages en verre"); omit it to get all five streams side by side. Omitting type returns up to 30 rows (5 streams × 6 years).

Read the per-capita waste series of one stream across years
- **waste_per_capita**: The dataset covers 2019–2024 and holds exactly 5 rows per year — one per stream. Streams are stored with a leading emoji label: "♻️ Biodéchets", "♻️ Emballages en verre", "♻️ Multimatériaux", "♻️ Déchets occasionnels" and "🗑️ Ordures ménagères résiduelles"; the type parameter matches the letters-only core, so "verre" or "Biodéchets" work. Omit type to get the whole year (5 rows).

Read the per-capita waste quantity of one stream in one year
- **waste_types_overview**: Use it to discover the exact filter values for waste_per_capita and waste_history.

Overview of the per-capita waste dataset: streams and year span


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paris Waste: TriLibre Stations & Per-Capita Streams** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much residual waste does a Parisian produce per year, and has it gone down since 2019?"

**🤖 AI Agent:**
> Run waste_history with type "résiduelles" and year_from 2019 — it returns the series and the computed delta between the two ends.

---

**👤 You:**
> "Where are the waste drop points near Montmartre?"

**🤖 AI Agent:**
> Montmartre sits mostly in the 18th arrondissement: call list_trilib_stations with arrdt "75018" and page through the rows for the address of the closest code.

---

**👤 You:**
> "Give me the 2024 quantities of all five waste streams."

**🤖 AI Agent:**
> Run waste_per_capita with year 2024 and no type — the dataset holds exactly five rows per year, one per stream, each in kg per inhabitant.


## ❓ FAQ

**Q: Do I need an API key?**
No. opendata.paris.fr serves all city datasets anonymously over its Opendatasoft REST API. This MCP defines no credentials and needs nothing configured.

**Q: How do I filter by waste stream type?**
Pass the letters-only name — "Biodéchets", "verre", "multimatériaux", "occasionnels" or "résiduelles". The tool resolves it to the stored emoji-labeled value through the dataset facets; an unknown type lists the available ones.

**Q: What do the quantities mean?**
The quantite column is kg per inhabitant per year for the whole City of Paris (no per-arrondissement breakdown). Five streams are tracked: recyclables (glass, multi-material, bio, occasional) and the residual fraction.

**Q: Are the TriLibre station addresses live?**
The station list is the current official reference (438 points, all with the status "Mobilier en service"), but it is a snapshot, not a live feed — closures or relocations appear in the next data refresh.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paris-waste-trilibre-stations-per-capita-streams](https://vinkius.com/en/ai-agent-connect/paris-waste-trilibre-stations-per-capita-streams)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paris Waste: TriLibre Stations & Per-Capita Streams** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paris-waste-trilibre-stations-per-capita-streams` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paris Waste: TriLibre Stations & Per-Capita Streams** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paris-waste-trilibre-stations-per-capita-streams": {
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
