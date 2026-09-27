# NYC Parks & Open Land (DCA) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-parks-open-land-dca)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environment](../categories/environment.md)

Keyless NYC parks data: DCA park properties by type, acreage and waterfront, the Forever Wild conservation sites, functional parkland, DCA playgrounds and synthetic turf fields — no API key.

## Description
New York City parks and open land, keyless.

### What you can do
- **Park properties** — the city's ~2,000 park properties with name, acreage, street address, property type (e.g. "Garden", "Neighborhood Park", "Triangle/Plaza") and subcategory, waterfront and retired flags, jurisdiction and district codes; filter by borough (full name or letter code B/M/Q/R/X), type, subcategory, waterfront or minimum acreage
- **Property lookup** — one park property by its exact stored name
- **Top park types** — property types ranked by count, to discover the exact type values
- **Property count** — a fast count of the properties matching a filter
- **Forever Wild sites** — the ~140 protected land-and-tree sites the city commits to keeping wild, by site name
- **Functional parkland** — the ~2,000 parkland parcels by borough, ZIP or precinct
- **DCA playgrounds** — the ~1,000 playgrounds with a dedicated children area, by name, borough or system
- **Synthetic turf fields** — the ~340 synthetic turf fields by park, system type, turf type or infill material

### Who is this for
Recreation and green-space planning, real estate (proximity and waterfront), and civic analysis. Filter values are exact matches on the stored values: park-property boroughs are single letters (B, M, Q, R, X — R is Staten Island), and the flag fields are the strings "True"/"False".


## Available Tools (8)
- **count_park_properties**: A single fast count — use it to gauge how large a list_park_properties call will be.

Count NYC park properties matching a filter
- **list_forever_wild_sites**: A small list (a few hundred sites). Optionally pin one property name.

List NYC Parks Forever Wild sites
- **list_functional_parkland**: About 2,000 parcels; filter by boro or ZIP to narrow the result.

List functional parkland parcels
- **list_park_properties**: g. "Garden", "Neighborhood Park", "Playground", "Triangle/Plaza") and subcategory, whether it is on the waterfront, whether it is retired, the jurisdiction, the boro code and the community board / council district / precinct. About 2,000 properties; filter by boro, type or waterfront to narrow the result.

List NYC Parks properties
- **list_playgrounds_dca**: About a thousand playgrounds; filter by boro to narrow the result.

List playgrounds with dedicated children areas
- **list_synthetic_turf_fields**: g. "Field Group"), the turf type and the infill material. A few hundred fields. Filter by park name, system type or turf type to narrow the result.

List NYC synthetic turf playing fields
- **lookup_park_property**: g. "Wishing Well Garden"): acreage, street address, property type and subcategory, waterfront and retired flags, jurisdiction, boro code and the community board / council district / precinct. If no property matches the name, an error is returned with guidance to list_park_properties to see available names.

Look up a NYC park property by name
- **top_park_types**: Each row is one property type with its count. Use it to see what the Parks portfolio looks like before listing properties of one type.

Count NYC park properties by type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Parks & Open Land (DCA)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the most common NYC park types?"

**🤖 AI Agent:**
> top_park_types returns the property types ranked by count — the first rows are "Triangle/Plaza", "Garden" and "Neighborhood Park". Use those exact values as the typecategory filter of list_park_properties.

---

**👤 You:**
> "Which parks in Manhattan of over 50 acres have a waterfront?"

**🤖 AI Agent:**
> list_park_properties with boro: "Manhattan", min_acres: "50" and waterfront: "True" returns the matching park properties with their acreage, address and type.

---

**👤 You:**
> "Where are the synthetic turf fields at Inwood Hill Park?"

**🤖 AI Agent:**
> list_synthetic_turf_fields with park: "Inwood Hill Park" returns the turf fields at that park with the system type, turf type, infill material and the maintaining unit; add turf_type: "Infill" to narrow it.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: Do the text filters ignore case or match partial values?**
No. The NYC data platform only supports exact-match filters, so a filter value must equal the stored value. In this MCP, property types are stored as "Garden", "Triangle/Plaza" or "Neighborhood Park", subcategories as e.g. "Greenthumb", and the waterfront/retired flags as the strings "True" or "False". Use top_park_types, or a list tool with no filters, to see the exact stored values before filtering.

**Q: How do I filter park properties by borough?**
Park properties, functional parkland and DCA playgrounds store the borough as a single letter — B (Brooklyn), M (Manhattan), Q (Queens), R (Staten Island), X (Bronx). The tools accept the full name ("Manhattan", "Staten Island") and convert it to the letter automatically; passing the letter directly works too.

**Q: What do the waterfront and retired flags mean?**
Both are stored as the strings "True" or "False". waterfront marks properties with a water edge; retired marks properties that have left the active Parks portfolio. Filter with the string values, e.g. waterfront: "True".


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-parks-open-land-dca](https://vinkius.com/en/ai-agent-connect/nyc-parks-open-land-dca)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Parks & Open Land (DCA)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-parks-open-land-dca` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Parks & Open Land (DCA)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-parks-open-land-dca": {
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
