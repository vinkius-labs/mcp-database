# NYC Sanitation (DSNY) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-sanitation-dsny)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless NYC sanitation data: DSNY collection garages, special waste and e-waste drop-off locations, pharma and syringe sites, the DonateNYC donation directory, commercial waste zones and disposal facilities — no API key.

## Description
New York City Department of Sanitation (DSNY) records, keyless.

### What you can do
- **Collection garages** — the under-100 DSNY garbage and recycling collection garages by name, address, city-area value and district code
- **Special waste sites** — the five special/hazardous household waste drop-off sites
- **E-waste drop-offs** — the ~100 electronics drop-off locations by site name, borough, ZIP or neighborhood tabulation area
- **Pharma & syringe sites** — the ~340 pharmaceutical and syringe (sharps) drop-off sites by site type ("PHARMACEUTICALS Drop-off" or "SYRINGE/SHARPS Drop-off"), with phone number and open days/hours
- **DonateNYC sites** — the ~1,500 donation sites with the item categories they accept, hours, phone and website
- **Commercial waste zones** — the ~20 DSNY commercial waste collection zones with their code, name and the community districts they cover
- **Disposal facilities** — the ~25 waste disposal facilities and sites with type code, address and coordinates

### Who is this for
Waste operations, sustainability programs, retail (e-waste and pharma locations near a store) and civic service lookups. The city-area values mix borough names with Queens neighborhood names (and "New York" means Manhattan), so use the list tools to see the exact values before filtering.


## Available Tools (7)
- **list_commercial_waste_zones**: g. "BX-1"), the zone name (e.g. "Bronx West") and the list of community districts it covers. A short list (about twenty zones). Use it to find out which commercial waste zone a community district belongs to.

List DSNY commercial waste zones
- **list_disposal_facilities**: g. "MTS" for marine transfer station), street address, city-area value, ZIP and coordinates. A short list (about 25 facilities). Filter by facility type or city-area value.

List waste disposal facilities used by DSNY
- **list_donatenyc_sites**: g. "Books/Media, Toys/Games"), its hours and the DSNY zone / district it belongs to. About 1,500 sites. Filter by boro, NTA or site name.

List DonateNYC donation sites
- **list_dsnv_garages**: g. "BX06G"), address, the city-area value, the DSNY district code and ZIP. There are under a hundred garages citywide. The city-area value mixes borough names ("Brooklyn", "Bronx", "New York" for Manhattan, "Staten Island") with Queens neighborhood names ("Woodside", "Flushing", ...). Filter by that value or by district code.

List DSNY garbage and recycling collection garages
- **list_ewaste_dropoffs**: g. "Brooklyn"), neighborhood tabulation area, and the DSNY zone / district / section it belongs to. About a hundred locations. Filter by boro, NTA or site name.

List e-waste (electronics) drop-off locations
- **list_pharma_syringe_sites**: About 340 sites. Filter by site type, boro or NTA.

List pharmaceutical and syringe drop-off locations
- **list_special_waste_sites**: This is a very short list (five sites) covering special/hazardous household waste drop-off locations.

List DSNY special waste drop-off sites


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Sanitation (DSNY)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where can I drop off old electronics in Brooklyn?"

**🤖 AI Agent:**
> list_ewaste_dropoffs with borough: "Brooklyn" returns the e-waste drop-off locations in Brooklyn with their site name and address; add site_name or zipcode to narrow it.

---

**👤 You:**
> "Which sites accept expired medicines?"

**🤖 AI Agent:**
> list_pharma_syringe_sites with site_type: "PHARMACEUTICALS Drop-off" returns the pharma sites with their address, phone number and open days/hours; use "SYRINGE/SHARPS Drop-off" for sharps.

---

**👤 You:**
> "Which community districts does commercial waste zone BX-1 cover?"

**🤖 AI Agent:**
> list_commercial_waste_zones with zone: "BX-1" returns the zone with its name ("Bronx West") and the community district codes it covers; list_disposal_facilities then shows the facilities, e.g. the MTS marine transfer stations.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: Do the text filters ignore case or match partial values?**
No. The NYC data platform only supports exact-match filters, so a filter value must equal the stored value. In this MCP, boroughs in the drop-off tables are stored in title case ("Brooklyn", "Manhattan"), pharma/syringe site types as "SYRINGE/SHARPS Drop-off" or "PHARMACEUTICALS Drop-off", and the garage/facility city-area values mix borough names, Queens neighborhood names and "New York" for Manhattan. Use a list tool with no filters to see the exact stored values before filtering.

**Q: What is DonateNYC?**
DonateNYC is the city's directory of donation sites — about 1,500 locations that accept items like books, toys and clothing. list_donatenyc_sites returns each site with the categories it accepts, its hours, phone and website; the category text is free-form, so filter by borough, NTA or site name instead.

**Q: How are boroughs stored in the sanitation datasets?**
It differs per dataset: the e-waste, pharma/syringe and DonateNYC tables store the borough in title case ("Brooklyn", "Manhattan"); the DSNY garages and disposal facilities store a city-area value that mixes borough names, Queens neighborhood names and "New York" for Manhattan. Use a list tool with no filters to see the exact values.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-sanitation-dsny](https://vinkius.com/en/ai-agent-connect/nyc-sanitation-dsny)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Sanitation (DSNY)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-sanitation-dsny` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Sanitation (DSNY)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-sanitation-dsny": {
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
