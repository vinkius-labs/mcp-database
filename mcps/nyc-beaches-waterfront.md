# NYC Beaches & Waterfront MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-beaches-waterfront)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environment](../categories/environment.md)

Keyless NYC beach and waterfront data: the nine public beaches, enterococci water-quality samples against EPA reference values, seasonal beach attendance, and designated waterfront public access areas — no API key.

## Description
New York City beaches and waterfront access, keyless. Built for trip planning — where to swim and whether the water is swimmable, how crowded a beach was, and where the city's designated waterfront access points are.

### What you can do
- **Beach lookup** — the nine named public beaches (Coney Island, Rockaway Beach, Jacob Riis, Orchard Beach, Manhattan Beach, South Beach, Midland Beach, Cedar Grove Beach, Wolfe's Pond Beach) by boro, with their map parcel counts
- **Water samples** — enterococci samples per beach and sample location in a lookback window; the dataset is live (September 2026 samples available)
- **Beach water quality ranking** — the beaches ranked by sample count over the last year with each beach's worst enterococci reading, to read against the EPA reference values
- **Sample count** — a fast count of samples in a window, optionally per beach
- **Seasonal attendance** — daily visitor counts at each beach for one season year (2010-2025)
- **Attendance ranking** — the beaches ranked by total visitors in a season year
- **Waterfront public access areas** — the ~78 designated WPAA areas with status, maintaining party, planning summary, resolution data and published hours

### Who is this for
Beach trip planning: combine the water-sample tools (interpreted against the EPA single-sample advisory of 235 MPN/100 ml and the 4-week geometric-mean criterion of 291) with the attendance rankings. Data freshness differs per tool: water samples are live, while the attendance table ends at 2025-10-08 (most recent season 2025) and the WPAA table is a planning registry with no coordinates.


## Available Tools (7)
- **count_water_samples**: A single fast count — use it to gauge how many samples a search_water_samples call will return.

Count beach water samples in a window
- **list_beaches**: There are no beach parcels in Manhattan (M) — "Manhattan Beach" is in Brooklyn. Use it as the lookup of beach names before calling the water-quality or attendance tools, whose beach filters are exact names.

List NYC public beaches by name and boro
- **list_waterfront_areas**: g. "Approved (to be constructed)"), the maintaining party, a planning summary of the access area, the CPC approval and resolution dates, planned and WPAA areas in square feet, the city planning report URL, the ZAP project link and published hours of operation. About 78 areas citywide; pin one by name or wpaa_id. The table carries no coordinates — pair it with the beach tools for water access. About half of the 78 are not yet constructed, so the status field distinguishes built areas from planned ones.

List NYC waterfront public access areas
- **search_beach_attendance**: Each row is one day at one beach with its attendance. Beach names are exact stored values in title case, e.g. "Orchard Beach", "Rockaway Beach", "Coney Island Beach", "Manhattan Beach", "Jacob Riis", "South Beach", "Midland Beach", "Cedar Grove Beach", "Wolfe's Pond Beach" (straight apostrophe). The dataset has not been updated since October 2025 — recent years return fewer days and the most recent season is 2025.

Search seasonal NYC beach attendance
- **search_water_samples**: Each row is one sample with the beach name (stored UPPERCASE, e.g. "MIDLAND BEACH"), the sample location along the beach ("Left", "Right" or "Center") and the enterococci result in MPN/100 ml; a null result with a units_or_notes of "Result below detection limit" means the bacteria count was below the detectable range. Interpret against the EPA reference values: 291 MPN/100 ml is the 4-week geometric-mean criterion and 235 MPN/100 ml the single-sample advisory level — readings above them flag the water. Samples are taken seasonally (summer through autumn); the dataset is live, with September 2026 samples available. The beach filter is an exact stored name, auto-uppercased — see list_beaches for the nine beach names.

Search NYC beach water-quality samples
- **top_beaches_attendance**: Each row is one beach with its summed attendance for the year. Note the dataset ends at 2025-10-08, so years after 2025 have no data.

Rank beaches by total attendance in a season year
- **top_beaches_water_quality**: Each row is one beach with its sample count in the window and its worst (maximum) enterococci reading in MPN/100 ml, or null when the window had no detectable readings. Compare worst_reading against the EPA single-sample advisory value of 235 MPN/100 ml — beaches whose worst reading exceeds it had at least one sample above the swim advisory. Use it to compare beach water quality across a season.

Beach water quality by beach over the last year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Beaches & Waterfront** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the water swimmable at Orchard Beach right now?"

**🤖 AI Agent:**
> search_water_samples with beach: "orchard beach" and days: "30" returns the recent enterococci samples (auto-uppercased to "ORCHARD BEACH"); read them against the EPA advisory values (235 MPN/100 ml single-sample, 291 4-week geometric mean), then top_beaches_water_quality for the year's worst reading at that beach.

---

**👤 You:**
> "Which NYC beach had the most visitors in 2025?"

**🤖 AI Agent:**
> top_beaches_attendance with year: "2025" ranks the nine beaches by their total 2025-season attendance; search_beach_attendance with the same year and that beach name returns the daily counts.

---

**👤 You:**
> "Which beaches are in Brooklyn?"

**🤖 AI Agent:**
> list_beaches with boro: "Brooklyn" returns the two Brooklyn beach names — "Manhattan Beach" (boro B) and "Coney Island" (boro B) — with their map parcel counts; note there are no beach parcels in Manhattan.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: Do the text filters ignore case or match partial values?**
No. The NYC data platform only supports exact-match filters, and this MCP stores beach names three different ways across its tables: the beach map and the water-sample table use UPPERCASE names ("ORCHARD BEACH" — the water-sample tool auto-uppercases its input), while the attendance table uses title case ("Orchard Beach", "Wolfe's Pond Beach" with a straight apostrophe). Borough codes on the beach map are the single letters B, Q, R, X (there are no beach parcels under M — Manhattan Beach is in Brooklyn). Use list_beaches to see the exact beach names, and a search tool with no filters to see the exact stored values in each table.

**Q: How do I read the enterococci values?**
The samples report enterococci in MPN/100 ml. Use the two EPA reference values: 235 MPN/100 ml is the single-sample advisory level and 291 MPN/100 ml the 4-week geometric-mean criterion. A reading above 235 flags the water above the swim advisory; a null enterococci value means the count was below the detection limit (the units_or_notes field says so). top_beaches_water_quality gives each beach's worst reading over the last year.

**Q: How fresh is each dataset?**
Water samples are live — September 2026 samples are available. The attendance table ends at 2025-10-08, so its tools take a season year (2010-2025, default 2025) rather than a rolling window. The WPAA table is a planning registry (statuses like "Approved (to be constructed)"), not a live status feed, and it carries no coordinates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-beaches-waterfront](https://vinkius.com/en/ai-agent-connect/nyc-beaches-waterfront)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Beaches & Waterfront** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-beaches-waterfront` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Beaches & Waterfront** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-beaches-waterfront": {
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
