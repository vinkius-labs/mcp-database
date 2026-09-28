# Paris Housing: Rent Caps & Social Housing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paris-housing-rent-caps-social-housing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless Paris housing data: the official rent-control ceilings by room/zone/building era (2019–2025), social-housing program delivery 2001–2024, and the housing waiting-list counts per arrondissement.

## Description
The City of Paris rent-control reference, its social-housing programs, and the housing waiting list — keyless, straight from the Paris open-data platform (opendata.paris.fr).

### What you can do
- **list_rent_caps / count_rent_caps / rent_cap_lookup** — the encadrement des loyers ceilings (€ / m² max and min) per room count (1–4), zone, quartier, building era and furnishing status, for the 2019–2025 vintages
- **list_social_housing / count_social_housing** — the ~4,300 social-housing program rows 2001–2024: dwellings delivered per program, by delivery mode (construction neuve / acquisition réhabilitation / acquisition conventionnement) and arrondissement
- **list_housing_beneficiaries / count_housing_beneficiaries** — the waiting-list beneficiary counts (solo, childless couples, couples with one child) per fiscal year 2013–2025 and arrondissement

### Who is this for
Renters and landlords checking what the legal cap is for a given apartment, and anyone studying Paris's social-housing pipeline or the waiting-list pressure by neighborhood. Note the year semantics: the cap annee is a text value ("2024"), while the social-housing annee and the waiting-list exercice are date-typed columns read through whole-year windows.


## Available Tools (7)
- **count_social_housing**: A fast total count for paging and comparisons between arrondissements or years.

Count social-housing program rows, optionally filtered
- **list_rent_caps**: Each row has the year (annee, a text value "2019".."2025"), the zone (id_zone "1".."14" plus id_quartier / nom_quartier, e.g. "Saint-Merri"), the room count (piece, 1 to 4), the building era (epoque: "Avant 1946", "1946-1970", "1971-1990" or "Apres 1990" — stored exactly so, the accent is missing on "Apres"), whether the cap is for furnished rentals (meuble_txt: "non meublé" or "meublé"), and the cap itself: max (€ / m², the ceiling) and min (€ / m², the floor). Use it to answer "what is the rent cap for a 3-room in zone 11 in 2024". Filters are exact stored values; piece is an integer. Page with limit/offset (100 rows max per call).

List the Paris rent-cap ceilings by room, building era and zone
- **list_social_housing**: Each row has the year (annee; the column is date-typed, so the annee parameter is a 4-digit year read as that whole year), the arrondissement (arrdt, "1".."20" as text), the dwelling breakdown (nb_logmt_total and the nb_plai / nb_pls / nb_plus / nb_pluscd counts by housing type), the delivery mode (mode_real: "construction neuve", "acquisition réhabilitation" or "acquisition conventionnement" — accents matter), the program nature and the address. Use it to answer "how many social-housing units were delivered in arrondissement 11 last year". Filters are exact stored values; page with limit/offset (100 rows max).

List Paris social-housing program finances
- **rent_cap_lookup**: g. "Halles" or "Saint-Merri"), optionally for one vintage year (annee, "2019".."2025"). A quartier spans up to 16 rows: 4 room counts × 2 furnishing statuses (the cap does not depend on the building era). The response carries max/min in € / m² per row.

Look up the rent caps of one quartier
- **count_housing_beneficiaries**: A fast total count.

Count housing waiting-list rows, optionally filtered
- **count_rent_caps**: A fast total count — use it to gauge how much paging list_rent_caps will need for a combination (each city-wide vintage has 2,560 rows: 14 zones × 4 room counts × …).

Count rent-cap rows, optionally filtered
- **list_housing_beneficiaries**: "2025") crossed with the arrondissement (arrondissement, 5-digit postal codes "75001".."75020"). Each row has the household-type breakdown: personne_isolee, couple_sans_enfant, couple_avec_un_enfant and the total. Use it to answer "how many housing applicants in the 16th in 2024". Filters are exact stored values; the dataset is small enough to page through fully.

List waiting-list beneficiaries of the Paris housing office


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paris Housing: Rent Caps & Social Housing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the rent cap for a 3-room unfurnished flat in zone 11 in 2024?"

**🤖 AI Agent:**
> Run list_rent_caps with annee "2024", piece "3", meuble_txt "non meublé" — the rows for that combination give max/min in € / m² (the cap multiplies by the surface).

---

**👤 You:**
> "How many social-housing units did Paris deliver in arrondissement 11 last year?"

**🤖 AI Agent:**
> Call list_social_housing with annee "2024" and arrdt "11" — sum the nb_logmt_total column over the returned programs; count_social_housing gives the row count without fetching.

---

**👤 You:**
> "Which arrondissements have the biggest housing waiting lists in 2024?"

**🤖 AI Agent:**
> Page through list_housing_beneficiaries with exercice "2024" (20 rows total) and compare the total column per arrondissement; the solo/couple columns break it down by household type.


## ❓ FAQ

**Q: Do I need an API key?**
No. opendata.paris.fr serves all city datasets anonymously over its Opendatasoft REST API. This MCP defines no credentials and needs nothing configured.

**Q: What do the cap values mean?**
Each row holds the legal ceiling (max) and floor (min) rent in € per square meter for that room count, building era and furnishing status. The city publishes one reference per year — the 2025 vintage is the most recent.

**Q: Why can I not filter the social housing by the text "2024"?**
The social-housing annee and the waiting-list exercice columns are date-typed: a plain text equality is rejected by the platform. The tools convert your 4-digit year into a whole-year window automatically.

**Q: Which years are covered?**
Rent caps: 2019–2025 (text year). Social-housing programs: 2001–2024. Waiting-list beneficiaries: 2013–2025 (fiscal years).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paris-housing-rent-caps-social-housing](https://vinkius.com/en/ai-agent-connect/paris-housing-rent-caps-social-housing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paris Housing: Rent Caps & Social Housing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paris-housing-rent-caps-social-housing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paris Housing: Rent Caps & Social Housing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paris-housing-rent-caps-social-housing": {
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
