# Paris Lighting: Street-Light Inventory MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paris-lighting-street-light-inventory)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless Paris street-light inventory: the 165,000+ public fixtures — code, road, public/private category, maintenance sector, arrondissement, lamp and support families.

## Description
Paris's public street-light inventory (eclairage public) — keyless, straight from the Paris open-data platform (opendata.paris.fr).

### What you can do
- **list_light_fixtures / light_fixture_lookup / count_light_fixtures** — the ~165,000 fixtures: code (cod_ouvrag, the lookup key), work type, lighting regime, maintenance notes, WGS84 coordinates, the road label as stored (UPPERCASE), the road category (public / private), the maintenance sector and the zero-padded arrondissement label
- **fixtures_by_road** — how many lamps sit on one road, with the first page of them
- **public_private_split** — the three totals: whole network, public roads and private roads
- **arrondissement_lighting** — one arrondissement's fixture count
- **lighting_overview** — the preset facets: top maintenance sectors, top lamp and support families, and the regime / road-category splits

### Who is this for
Urban designers, journalists on lighting quality, and anyone locating a fixture by its code or counting the lamps on a street. Road labels are stored UPPERCASE with a type suffix (e.g. "LEGENDRE (RUE)"); arrondissements use the zero-padded label "Arrondissement NN", which the tools map from a plain 1..20 number for you. The dataset is the city's fixed asset register — where each fixture is, what it is and its regime — not a live dimming or outage feed.


## Available Tools (7)
- **arrondissement_lighting**: arrondissement is required: the number 1..20, mapped to the stored zero-padded label ("Arrondissement 06" for 6).

Count the fixtures in one arrondissement
- **count_light_fixtures**: 20, mapped to the stored label), voie (stored UPPERCASE road label), voie_categorie ("VOIES PUBLIQUES" / "VOIES PRIVEES") and secteur (stored sector label) — the same exact-match filters as list_light_fixtures. A fast total count; use it to gauge how many lamps a street or sector has.

Count street-light fixtures by road, category, sector or arrondissement
- **lighting_overview**: No parameters.

Overview of the street-light inventory: top sectors, lamps, supports, regimes
- **fixtures_by_road**: voie is required — the stored UPPERCASE road label (voie_libelle), e.g. "LEGENDRE (RUE)". Optionally restrict to one road category (voie_categorie: "VOIES PUBLIQUES" / "VOIES PRIVEES").

Count and list the fixtures on one road
- **light_fixture_lookup**: g. "O10721") exactly matches the given value. cod_ouvrag is required; 0 or 1 row comes back with the work type, lighting regime, maintenance notes, road, sector and coordinates.

Look up a street-light fixture by its code
- **list_light_fixtures**: Each row has the fixture code (cod_ouvrag, e.g. "O10721" — the lookup key), the work type (lib_ouvrag, e.g. "Candélabre"), the lighting regime (lib_regime, e.g. "HORAIRE EP"), maintenance notes (observatio), the WGS84 coordinates as text (x_wgs84 / y_wgs84), the road label as stored (voie_libelle, UPPERCASE, e.g. "LEGENDRE (RUE)"), the road category (voie_categorie: "VOIES PUBLIQUES" or "VOIES PRIVEES"), the maintenance sector (secteur_libelle, e.g. "15_NECKER") and the arrondissement label (zero-padded, "Arrondissement 06".."Arrondissement 20"). All columns are exact-match text filters; pass arrondissement as the number 1..20 and it is mapped to its stored label. Page with limit/offset (100 rows max per call).

List the public street-light fixtures of Paris
- **public_private_split**: Shows how much of the city lighting stock lives on publicly owned streets. No parameters.

Split the fixture inventory between public and private roads


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paris Lighting: Street-Light Inventory** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many street lights does the 6th arrondissement have?"

**🤖 AI Agent:**
> Call arrondissement_lighting with arrondissement "6" — one fast total comes back; count_light_fixtures adds per-road or per-sector filters on top.

---

**👤 You:**
> "How many lamps light the rue Legendre?"

**🤖 AI Agent:**
> Run fixtures_by_road with voie "LEGENDRE (RUE)" — the road label is stored UPPERCASE with its type; you get the total plus a first page of fixture codes and regimes.

---

**👤 You:**
> "How is the lighting network split between public and private roads?"

**🤖 AI Agent:**
> public_private_split returns the three totals in one call: the whole network, the public-road count and the private-road count.


## ❓ FAQ

**Q: Do I need an API key?**
No. opendata.paris.fr serves all city datasets anonymously over its Opendatasoft REST API. This MCP defines no credentials and needs nothing configured.

**Q: How are the road names stored?**
UPPERCASE with a type suffix in parentheses, e.g. "LEGENDRE (RUE)" or "CINQ MARS (AVENUE)". The voie filter is an exact match on the stored label — fetch a page of list_light_fixtures to see the exact forms.

**Q: What does the public/private split mean?**
voie_categorie separates the network between streets maintained on public land (VOIES PUBLIQUES) and privately owned roads lit by the city (VOIES PRIVEES) — public_private_split returns both totals plus the grand total in one call.

**Q: Is this a live sensor feed?**
No. The dataset is the city's fixed asset register of each fixture — its code, location, lamp/support family and lighting regime. It is not a dimming, outage or occupancy feed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paris-lighting-street-light-inventory](https://vinkius.com/en/ai-agent-connect/paris-lighting-street-light-inventory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paris Lighting: Street-Light Inventory** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paris-lighting-street-light-inventory` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paris Lighting: Street-Light Inventory** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paris-lighting-street-light-inventory": {
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
