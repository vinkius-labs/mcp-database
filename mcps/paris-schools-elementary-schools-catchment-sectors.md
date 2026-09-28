# Paris Schools: Elementary Schools & Catchment Sectors MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paris-schools-elementary-schools-catchment-sectors)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Keyless Paris elementary-school data: the school census (name, address, arrondissement, school year, 2020–2027) and the catchment sectors that assign streets to up to four schools.

## Description
The City of Paris elementary-school census and its catchment-sector (secteur scolaire) assignments — keyless, straight from the Paris open-data platform (opendata.paris.fr).

### What you can do
- **list_schools / count_schools / school_lookup** — the ~2,200 school-year rows: the stored name (e.g. "LITTRE (6) ELEM" — the number is the school code), street address, arrondissement, school year and type (Elémentaire / Polyvalent)
- **list_school_sectors / count_school_sectors** — the ~2,500 catchment-sector rows: each sector labels its zone and lists up to four assigned schools (lib_etab_1..4) with their addresses
- **find_school_sectors** — the reverse lookup: given a school name, which sectors assign children to it (all four columns are probed and deduplicated)
- **school_census** — the two dataset totals for a school year, with the city-wide totals for context

### Who is this for
Parents checking which school their address feeds into, journalists and researchers tracking school supply, and anyone comparing a school year's census against its sectors. Names are stored UPPERCASE with the code in parentheses — use school_lookup or list_schools to discover the exact stored form first.


## Available Tools (7)
- **count_school_sectors**: A fast total count — about 370–380 sectors per school year.

Count catchment-sector rows, optionally filtered
- **school_census**: "2026-2027"): how many school census rows and how many catchment-sector rows that year holds, plus the city-wide totals without the year filter for context. A fast overview — use it before paging list_schools / list_school_sectors for a year.

Summarize the school census and sector counts for a school year
- **count_schools**: A fast total count — the city-wide census per year is about 350–380 rows.

Count elementary-school rows, optionally filtered
- **find_school_sectors**: g. "LITTRE (6) ELEM") is matched against all four assigned-school columns of the sector dataset (lib_etab_1..lib_etab_4) and the matching sectors are returned, optionally for one school year (annee_scol). Use it to answer "which streets/sectors send children to school X". The match is an exact stored-name equality, so use the stored UPPERCASE form from list_schools / school_lookup.

Find the catchment sectors that assign to a given school
- **list_school_sectors**: Each row has the sector label (libelle, e.g. "Z. MANIN(30)/MANIN(40B)"), the zone commune, up to four assigned schools (lib_etab_1..lib_etab_4 and their addresses) and the year. A sector is a catchment area: children of its addresses are assigned to the schools listed in the lib_etab columns. Filters are exact stored values; page with limit/offset (100 rows max per call).

List elementary-school catchment sectors (secteurs scolaires)
- **list_schools**: Each row has the school name as stored (libelle, e.g. "LITTRE (6) ELEM" — number in parentheses is the school code), the street address, the arrondissement (arr_libelle as stored "Xème Ardt", plus the arr_insee code), the school year (annee_scol, "2020-2021".."2026-2027") and the type (type_etabl: "Elémentaire" or "Polyvalent"). Filters are exact stored values; page with limit/offset (100 rows max per call).

List Paris public elementary schools
- **school_lookup**: g. "LITTRE (6) ELEM". Names are stored UPPERCASE with the school code in parentheses and an ELEM/POLY suffix, and the same school appears once per school year, so expect up to 7 rows. Use list_schools first to discover the exact stored form.

Look up Paris elementary schools by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paris Schools: Elementary Schools & Catchment Sectors** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which catchment sectors assign children to the LITTRÉ school?"

**🤖 AI Agent:**
> Resolve the stored name first ("LITTRE (6) ELEM" from list_schools / school_lookup), then run find_school_sectors with that libelle and the school year — it probes all four assigned-school columns and deduplicates.

---

**👤 You:**
> "How many elementary schools does Paris run in the 2026-2027 year?"

**🤖 AI Agent:**
> Call count_schools with annee_scol "2026-2027" — the fast total; school_census adds the sector total for the same year alongside the city-wide totals.

---

**👤 You:**
> "List the polyvalent schools of the 6th arrondissement in 2025-2026."

**🤖 AI Agent:**
> Run list_schools with arr_libelle "6ème Ardt", type_etabl "Polyvalent" and annee_scol "2025-2026" — the arrondissement label keeps its "Ardt" abbreviation exactly as stored.


## ❓ FAQ

**Q: Do I need an API key?**
No. opendata.paris.fr serves all city datasets anonymously over its Opendatasoft REST API. This MCP defines no credentials and needs nothing configured.

**Q: What is a catchment sector?**
A secteur scolaire is a neighborhood group that the city assigns to up to four elementary schools (the lib_etab_1..4 columns). Children in the sector's zone are enrolled in those schools — find_school_sectors answers "which sectors send children to school X".

**Q: Why do I sometimes get 0 rows from school_lookup?**
Names are stored UPPERCASE with the school code in parentheses and an ELEM/POLY suffix ("LITTRE (6) ELEM"). The match is exact — run list_schools first to discover the stored form. School years rotate, so a school may only appear in the years it was open.

**Q: Which school years are covered?**
Both datasets span 2020-2021 through 2026-2027; the census also holds a few rows with a null year. The newest year (2026-2027) is the current assignment calendar.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paris-schools-elementary-schools-catchment-sectors](https://vinkius.com/en/ai-agent-connect/paris-schools-elementary-schools-catchment-sectors)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paris Schools: Elementary Schools & Catchment Sectors** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paris-schools-elementary-schools-catchment-sectors` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paris Schools: Elementary Schools & Catchment Sectors** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paris-schools-elementary-schools-catchment-sectors": {
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
