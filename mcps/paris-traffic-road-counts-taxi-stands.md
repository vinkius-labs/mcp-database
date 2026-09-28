# Paris Traffic: Road Counts & Taxi Stands MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paris-traffic-road-counts-taxi-stands)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless Paris road-traffic data: hourly vehicle counts, mean speed and congestion state at ~3,700 permanent counter sites, plus the 420 official taxi stands — filter by site code, state, arrondissement.

## Description
The City of Paris permanent road-traffic counters and its official taxi stands — keyless, straight from the Paris open-data platform (opendata.paris.fr).

### What you can do
- **list_traffic_sites / traffic_site_lookup / count_traffic_sites** — the ~3,700 counter-site reference (code iu_ac, road name, neighboring counters, measurement period)
- **traffic_counts** — hourly measurements at one site (vehicle count q, mean speed k, congestion state), with an ISO time window on t_1h and an optional state filter
- **traffic_counts_by_state** — how many hourly rows sit in a state ("Fluide", "Pré-saturé", "Saturé", "Inconnu"), city-wide or at one site
- **list_taxi_stands / taxi_stand_lookup / count_taxi_stands** — the ~420 official taxi stands: name, arrondissement, address, bay count, status

### Who is this for
Anyone reasoning about Paris congestion — which counter is on a given street, how busy it was in a window, how long a corridor stayed saturated — and anyone looking for an official taxi stand. Filters match stored values exactly (the states keep their accents: "Pré-saturé"). A bare time window over the 29.6M-row counter dataset is rejected by the platform, so traffic_counts always reads one site.


## Available Tools (7)
- **count_taxi_stands**: "75120"), statut ("en service" / "station provisoire") or emplacements — the same exact-match filters as list_taxi_stands. A fast total count; use it to compare stand counts between arrondissements.

Count taxi stands, optionally by arrondissement or status
- **list_traffic_sites**: Each row has the site code (iu_ac, e.g. "1232"), the road name with underscores as stored (libelle, e.g. "Av_Gambetta"), the upstream/downstream neighboring counter codes and names, and the measurement period start/end dates. Use iu_ac as the join key for the counting tools. The iu_ac filter is an exact match. Page with limit/offset (100 rows max per call).

List the permanent road-traffic counter sites in Paris
- **taxi_stand_lookup**: g. "Porte de Pantin" or "OPEA" (stored "OPERA"). The names are stored without accents in many cases and the match is exact, so use the stored form from list_taxi_stands when unsure. Returns 0, 1 or a few rows with the address, arrondissement INSEE, bay count and status.

Find taxi stands by name
- **traffic_counts**: 6 million rows, one row per site per hour, with the hourly vehicle count (q, ~42% of rows null), the mean speed in km/h (k), and the congestion state (etat_trafic: "Fluide", "Pré-saturé", "Saturé" or "Inconnu"). iu_ac is required (a bare time window over the whole dataset is rejected by the platform). since/until are ISO timestamps (YYYY-MM-DDTHH:MM:SS, optionally with a UTC offset) delimiting the t_1h column. Pass a few hours, not months — rows are capped at 100 per call, so page with offset to read longer windows. An optional etat_trafic filter is an exact match on one of the four stored states.

Read hourly traffic counts at a counter site
- **traffic_counts_by_state**: A fast total count on the 29.6-million-row dataset — use it to gauge how long a corridor stays in a state (e.g. how many hours a site spent "Saturé" recently, combined with the since/until window of traffic_counts). No since/until window is applied here; the count spans the whole dataset.

Count hourly rows in a congestion state, optionally at one site
- **traffic_site_lookup**: g. "1232"): road name as stored (underscores), the neighboring upstream/downstream counters and the measurement period dates. iu_ac is required. 0, 1 or a few rows come back (some road names carry several codes).

Look up a traffic counter site by its iu_ac code
- **list_taxi_stands**: Each row has the stand name (nom, e.g. "OPERA" for the Opéra stand), the INSEE code of the arrondissement it sits in (insee, "75101".."75120", the 751xx form), the street address, the number of parking bays (emplacements, a number stored as text, "2" up to "20"+) and the status (statut: "en service" for almost all, "station provisoire" for a few). Filters are exact stored values. The whole dataset fits in one or two calls; page with limit/offset (100 rows max).

List official taxi stands (bornes d’appel) in Paris


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paris Traffic: Road Counts & Taxi Stands** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which traffic counter sits on Avenue de Gambetta, and how many cars passed at 8am today?"

**🤖 AI Agent:**
> Look up the site via traffic_site_lookup or list_traffic_sites with libelle "Av_Gambetta", then read traffic_counts for its iu_ac with an ISO window covering 08:00 — the row returns q (vehicles/hour), k (mean speed km/h) and etat_trafic.

---

**👤 You:**
> "How many hours did the counter at iu_ac 1232 stay saturated in the last week?"

**🤖 AI Agent:**
> Call traffic_counts_by_state with iu_ac "1232" and etat_trafic "Saturé" — it returns the number of hourly rows in that state; combine with traffic_counts to list the actual hours.

---

**👤 You:**
> "List the official taxi stands in the 8th arrondissement."

**🤖 AI Agent:**
> Run list_taxi_stands with insee "75108" (the 8th arrondissement's INSEE code) — each row has the stand name, address and bay count.


## ❓ FAQ

**Q: Do I need an API key?**
No. opendata.paris.fr serves all city datasets anonymously over its Opendatasoft REST API. This MCP defines no credentials and needs nothing configured.

**Q: Why does traffic_counts require a site code?**
The counter dataset holds ~29.6M hourly rows, and the ODS platform rejects a bare time-window query over it. Pass an iu_ac site code (from list_traffic_sites) and the window applies to that site.

**Q: What are the congestion states?**
Four stored values: "Fluide" (free-flowing), "Pré-saturé" (near capacity), "Saturé" (saturated) and "Inconnu". Accents matter — use them exactly.

**Q: Are the taxi stands live?**
No — the dataset is a static official reference of the ~420 stands (name, address, arrondissement, bay count, status), not a real-time occupancy feed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paris-traffic-road-counts-taxi-stands](https://vinkius.com/en/ai-agent-connect/paris-traffic-road-counts-taxi-stands)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paris Traffic: Road Counts & Taxi Stands** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paris-traffic-road-counts-taxi-stands` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paris Traffic: Road Counts & Taxi Stands** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paris-traffic-road-counts-taxi-stands": {
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
