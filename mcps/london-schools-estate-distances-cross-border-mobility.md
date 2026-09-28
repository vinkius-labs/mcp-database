# London Schools: Estate, Distances & Cross-Border Mobility MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/london-schools-estate-distances-cross-border-mobility)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Keyless London school data: the 2016 school estate (URN, phase, status, local authority, coordinates), per-school travel-distance trends 2010-2016, home-school distance benchmarks by authority, and 2011 cross-border mobility for children.

## Description
Four official London education datasets — keyless, straight from the London open-data platform (data.london.gov.uk).

### What you can do
- **list_schools / school_lookup / count_schools / schools_by_borough / schools_overview** — the 2016 London school estate: every school's URN (the lookup key), name, type and phase, open/closed status, gender, ward, LSOA, local authority and WGS84 coordinates; counts by phase and status, the borough ranking, and a city-wide snapshot
- **school_distance_trends** — one school's travel-distance series for 2010-2016: pupils attending plus the 25th/50th/75th percentile and mean distance in kilometres, by URN or exact name
- **home_school_distances** — the share of pupils in each authority who travel beyond the standard distance for their phase (primary/secondary), with the authority's local average
- **cross_border_mobility** — the 2011 census cross-border study per borough: how many children live in the borough, how many attend a state school anywhere in London, and the share attending outside their home borough

### Who is this for
Education researchers, housing and transport planners (catchment pressure), and journalists. The estate extract is a 2016 snapshot, the distances run 2010 to 2016 and the mobility study is from the 2011 census — the tools state each vintage in their titles. The school estate carries a trailing null column and the distance sheet has two leading title rows; both are handled inside the tools.


## Available Tools (8)
- **count_schools**: Count London schools with phase/status breakdowns
- **cross_border_mobility**: Sorted by resident children count; optional top-N (max 37).

Cross-border primary-school mobility by resident borough
- **home_school_distances**: Optional phase and la filters (case-insensitive).

Share of London pupils living far from school, by borough
- **list_schools**: Filter by la, phase, status or type (all exact, case-insensitive). Page with limit/offset.

London school records with address, coordinates and status
- **school_distance_trends**: urn takes precedence when both are given.

Pupil travel-distance trends for one school (2010-2016)
- **school_lookup**: g. "100001") or by name (case-insensitive substring, capped at 25 matches). At least one of urn/name is required.

Find London schools by URN or name
- **schools_by_borough**: Optional top-N (max 33).

School counts per London local authority
- **schools_overview**: Citywide snapshot of the London school estate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **London Schools: Estate, Distances & Cross-Border Mobility** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many open primary schools are in Camden?"

**🤖 AI Agent:**
> Call count_schools with la "Camden" — the total and the by-phase and by-status splits come back; read the Primary count with Open as the answer.

---

**👤 You:**
> "Show the travel distances for Argyle Primary School."

**🤖 AI Agent:**
> Call school_distance_trends with urn "100008" (or name "Argyle Primary School") — the 2010-2016 series returns pupils attending plus the 25th/median/75th percentile and mean distance in kilometres.

---

**👤 You:**
> "Which borough has the highest cross-border primary-school mobility?"

**🤖 AI Agent:**
> Run cross_border_mobility with a large top — each row carries the borough, its census children, the state-school attendees and the share attending outside the home borough; sort the share column descending.


## ❓ FAQ

**Q: Do I need an API key?**
No. data.london.gov.uk publishes every dataset as an anonymous file download (CSV or Excel). This MCP defines no credentials and needs nothing configured.

**Q: Which year is the school estate from?**
The estate extract is a 2016 snapshot. That vintage is stated in every tool title that reads it — list_schools, count_schools and the borough ranking all say 2016 extract in the title.

**Q: What do the distance percentiles mean?**
For a given school and year, the pupils field is how many attend, and the q25/median/q75 plus mean fields are the kilometres the pupils travel to get there — the 25th, 50th and 75th percentile of that distribution. Both series run 2010 to 2016.

**Q: What is cross-border mobility?**
From the 2011 census: for each borough, how many of the children who live there attend a state school, and what share of them attend one outside their home borough. The table has one row per borough plus a London row, with children counts, state-school counts and the share attending outside the home borough.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/london-schools-estate-distances-cross-border-mobility](https://vinkius.com/en/ai-agent-connect/london-schools-estate-distances-cross-border-mobility)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **London Schools: Estate, Distances & Cross-Border Mobility** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `london-schools-estate-distances-cross-border-mobility` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **London Schools: Estate, Distances & Cross-Border Mobility** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "london-schools-estate-distances-cross-border-mobility": {
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
