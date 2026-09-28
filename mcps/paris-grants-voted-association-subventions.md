# Paris Grants: Voted Association Subventions MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paris-grants-voted-association-subventions)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless Paris association-grant data: the 107,000+ voted subventions 2013–2026 — beneficiary, SIRET, amount, direction, type, granting body — with per-year series, big-grant filters and an overview.

## Description
The City of Paris voted association grants (subventions votées) — keyless, straight from the Paris open-data platform (opendata.paris.fr).

### What you can do
- **list_grants / count_grants / grant_lookup** — the ~107,000 grant rows: file number (numero_de_dossier, the lookup key), budget year (display year 2013..2026), granting body (City / Department), the beneficiary association (name + SIRET), the grant object, the voted amount in euros, the granting direction code (DDCT, DJS, DAE, DAC, DASES, DFPE...), the grant type and the association's activity sectors (an array, returned as-is)
- **beneficiary_history** — one association's whole grant history, optionally restricted to one year
- **big_grants** — the grants at or above a minimum voted amount (a bare integer >=; 1e6 returns 501 rows)
- **grants_by_year** — per-year totals across 2013..2026 (capped at 12 years, most recent first when the range is wider) with the range sum and the last-minus-first delta
- **grants_by_direction / grants_overview** — one direction's total, and the preset facets: top beneficiaries, the type split, the granting bodies and the top directions

### Who is this for
Civic journalists, researchers on Paris's associative fabric, and anyone checking whether a given association receives city money. The budget-year column is date-typed, so the annee filter is applied as a quoted ISO year window; the amount is a plain integer with a bare >= filter.


## Available Tools (8)
- **grants_by_direction**: g. "DDCT" culture — the largest with ~25,000 files — "DAC", "DJS" sport, "DFPE", "DASES", "DAE"). direction is required; optionally restrict to one budget year.

Count the grants of one granting direction
- **grants_overview**: No parameters.

Overview of the voted-grants dataset: top beneficiaries, types, bodies, directions
- **grant_lookup**: g. "2021_04573") exactly matches the given value. numero_de_dossier is required; 0 or 1 row comes back with the beneficiary, SIRET, amount, direction, type, granting body and the association’s activity sectors.

Look up a grant by its file number
- **grants_by_year**: year_to, 4 digits, both ends clamped to "2013".."2026", default 2015..2026, capped at 12 years — the most recent years win), computed as one fast DATE-window count per year, plus the range total and the last-minus-first delta. Optionally restricted to one direction or one grant type.

Count the grants per budget year
- **beneficiary_history**: beneficiary is required; optionally restrict to one budget year (annee, "2013".."2026"). Each row carries the amount (montant_vote), direction and type, so the response doubles as a small per-association report.

List the grants received by one association
- **big_grants**: min_amount is required; optionally restrict to one budget year (annee) and/or one grant type (nature). Useful to surface the city’s largest associations’ grants, e.g. min_amount 1000000 (501 rows city-wide at that floor in the current data).

List the largest grants by a minimum voted amount
- **count_grants**: "2026"), direction (code), nature (stored type), collectivite ("Ville de Paris" / "Département de Paris"), beneficiary (stored association name) and min_amount (euros on montant_vote). A fast total count — use it to compare volumes between directions, types or years.

Count association grants by year, direction, type, body or amount
- **list_grants**: Each row has: the file number (numero_de_dossier, e.g. "2021_04573" — the lookup key), the budget year (annee_budgetaire, the display year "2013".."2026" — the column is DATE-typed, so the annee filter maps to a quoted ISO year window over it), the granting body (collectivite: "Ville de Paris" or "Département de Paris" — a small legacy "v" value also exists), the beneficiary association (nom_beneficiaire, with its SIRET), the grant object (objet_du_dossier), the voted amount in euros (montant_vote, an integer), the granting direction (direction, a code such as "DDCT" culture, "DAE" European affairs, "DJS" sport, "DAC", "DASES" or "DFPE"), the grant type (nature_de_la_subvention: "Fonctionnement", "Projet", "Investissement", "Non précisée" or "Indéterminée") and the association’s activity sectors (secteurs_d_activites_definies_par_l_association, an array — returned as-is, not filterable). Page with limit/offset (100 rows max per call).

List the voted association grants (subventions) of the City of Paris


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paris Grants: Voted Association Subventions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many grants did the sport direction file in 2021?"

**🤖 AI Agent:**
> Call count_grants with direction "DJS" and annee "2021" — one fast total; grants_by_direction gives the all-years count for the same direction.

---

**👤 You:**
> "Which associations received the largest grants?"

**🤖 AI Agent:**
> Run big_grants with min_amount "1000000" — the rows list the beneficiary, its SIRET, the direction and the voted amount; page with limit/offset for the long tail.

---

**👤 You:**
> "Does the LESTUDIO TALENTS association receive city grants?"

**🤖 AI Agent:**
> Call beneficiary_history with beneficiary "LESTUDIO TALENTS" — the total counts its grants across all years and the rows show each amount, direction and type; add annee for one year.


## ❓ FAQ

**Q: Do I need an API key?**
No. opendata.paris.fr serves all city datasets anonymously over its Opendatasoft REST API. This MCP defines no credentials and needs nothing configured.

**Q: What do the direction codes mean?**
Each grant is issued by a city department identified by a code: DDCT (culture, the largest with ~25,000 files), DAC, DJS (sport, ~12,000), DASES, DAE, DASCO, DFPE, DPSP... grants_overview lists the top directions by count so you can discover the codes.

**Q: What grant types exist?**
Five stored values: Fonctionnement (operations), Projet, Investissement, Non précisée and Indéterminée. The nature filter is an exact match on the stored text, accents included.

**Q: Does a 0 amount mean nothing was paid?**
montant_vote is the voted amount and the source data contains rows where it is 0. Use a min_amount filter (big_grants, or the same filter on list_grants) to keep only positive grants.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paris-grants-voted-association-subventions](https://vinkius.com/en/ai-agent-connect/paris-grants-voted-association-subventions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paris Grants: Voted Association Subventions** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paris-grants-voted-association-subventions` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paris Grants: Voted Association Subventions** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paris-grants-voted-association-subventions": {
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
