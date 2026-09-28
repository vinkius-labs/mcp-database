# Paris Plaques: Commemorative Memorials MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paris-plaques-commemorative-memorials)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless Paris commemorative-plaque data: the 2,600+ city plaques (century, material, theme, person, arrondissement) plus the 1,200+ dedicated 1939-1945 memorials.

## Description
Paris's two commemorative-plaque datasets — keyless, straight from the Paris open-data platform (opendata.paris.fr).

### What you can do
- **list_plaques / plaque_lookup / count_plaques** — the ~2,600 city plaques: index (the lookup key), arrondissement (integer 1..20), UPPERCASE address, exact placement, the inscription (retranscription), material (~20 stored values), title, century (stored text: "12".."20" plus range values like "18-19"), theme, commemorated person and countries
- **plaques_by_century / plaques_by_arrondissement** — fast totals for one century or one arrondissement
- **plaques_overview** — the preset facets: the century split, the top arrondissements and the top materials
- **list_ww2_plaques / count_ww2_plaques** — the dedicated 1939-1945 dataset (~1,200 rows): the inscription, the full address, the address detail, the postal code and the WGS84 coordinates

### Who is this for
History enthusiasts, journalists on Paris's memory sites, and anyone following a street to see whose plaques hang on its façades. Century values are stored as text — including range labels like "18-19" — while the arrondissement and plaque-index columns are plain integers; the tools build the right clause type for each.


## Available Tools (8)
- **list_ww2_plaques**: Each row has: the record identifier (identifiant, integer), the inscription (commemore, e.g. "DESNOS Robert" or a longer memorial text), the full address (adresse_complete), the address detail (precision_adresse), the postal code (stored under the field name "empty", e.g. 75011) and the WGS84 coordinates (xy, an object with lon and lat). No filters; page with limit/offset (100 rows max per call).

List the 1939-1945 commemorative plaques
- **plaque_lookup**: g. 4975) matches the given value. index_plaque is required; 0 or 1 row comes back with the address, placement, inscription, material, century, theme and the commemorated person.

Look up a plaque by its index
- **count_plaques**: 20), siecle (stored century text), pays, objet (stored theme) or personalite — the same exact-match filters as list_plaques. A fast total count; use it to compare plaque density between arrondissements or centuries.

Count plaques by arrondissement, century, theme or person
- **count_ww2_plaques**: No parameters.

Count the 1939-1945 plaques
- **list_plaques**: Each row has: the plaque index (index_plaque, the integer lookup key), the arrondissement number (ardt, 1..20), the street address (adresse, UPPERCASE as stored, e.g. "12 RUE PIERRE ET MARIE CURIE"), the exact placement (emplacement, e.g. "RDC" or "1er étage Façade"), the inscription (retranscription), the material (materiau, ~20 stored values like "cuivre" or "marbre"), the title (titre), the century (siecle, stored as text: "12".."20" plus range values like "18-19"), the theme (objet_1, e.g. "les artistes (théâtre et cinéma)"), the commemorated person (personalite) and the countries involved (pays, comma-separated). Filters: ardt is an integer exact match, siecle/pays/objet/personalite are exact stored values. Page with limit/offset (100 rows max per call).

List the commemorative plaques of Paris
- **plaques_by_arrondissement**: ardt is required: the number 1..20 applied as a bare integer filter on the ardt column.

Count the plaques in one arrondissement
- **plaques_by_century**: g. "19" for the 19th century or the range value "18-19"). siecle is required.

Count the plaques commemorating one century
- **plaques_overview**: No parameters.

Overview of the plaque inventory: centuries, arrondissements, materials


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paris Plaques: Commemorative Memorials** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many 19th-century plaques are in the 6th arrondissement?"

**🤖 AI Agent:**
> Call count_plaques with ardt "6" and siecle "19" — one fast total (the platform verified 282 for 6th + 19th century).

---

**👤 You:**
> "What are the most common plaque materials?"

**🤖 AI Agent:**
> plaques_overview returns the top materials facet by count, alongside the century split and the top arrondissements.

---

**👤 You:**
> "List some 1939-1945 memorials."

**🤖 AI Agent:**
> Call list_ww2_plaques with a small limit — each row has the inscription (commemore), the full address, the address detail, the postal code and the coordinates.


## ❓ FAQ

**Q: Do I need an API key?**
No. opendata.paris.fr serves all city datasets anonymously over its Opendatasoft REST API. This MCP defines no credentials and needs nothing configured.

**Q: What is the difference between the two plaque datasets?**
The main dataset (~2,600 rows) is the city-wide inventory across all centuries and themes, with the material, theme and person fields; the 1939-1945 dataset (~1,200 rows) is a dedicated WWII memorials register with its own fields (identifiant, commemorore, adresse_complete, postal code and coordinates).

**Q: Why does siecle accept "18-19"?**
Century values are stored as text, and the source uses range labels for plaques spanning two centuries — "18-19" is a stored value you can filter on exactly like "19".

**Q: Are the addresses complete enough to geocode?**
The main dataset stores the street address and the exact placement (floor, façade) plus WGS84 coordinates; the 1939-1945 dataset adds the postal code (stored under the odd field name "empty") and an xy coordinate object.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paris-plaques-commemorative-memorials](https://vinkius.com/en/ai-agent-connect/paris-plaques-commemorative-memorials)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paris Plaques: Commemorative Memorials** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paris-plaques-commemorative-memorials` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paris Plaques: Commemorative Memorials** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paris-plaques-commemorative-memorials": {
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
