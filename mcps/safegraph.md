# SafeGraph MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/safegraph)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Integrate SafeGraph's premier geospatial dataset into your AI. Discover detailed POIs, analyze foot traffic patterns, and process precise building geometries seamlessly from conversational prompts.

## Description
Empower your AI with direct connectivity to **SafeGraph**, the foundational geospatial and mobility dataset trusted by top analytics and enterprise organizations globally. This robust integration converts your AI into an expert geographical analyst capable of retrieving precise intelligence surrounding global structures, Points of Interest (POIs), and detailed patterns—all without touching complex database pipelines.

### What you can do

- **Rich Context on POIs** — Fetch exhaustive lists of businesses or brands within targeted radii (`search_distance_radius`, `search_brand_places`). You can also slice the results according to their designated NAICS industry codes region-to-region (`search_industry_naics`).
- **Deep Geospatial Footprints** — Look up exact WKT polygons for targeted individual buildings (`lookup_building_geometry`) or identify everything bounded inside designated custom city borders (`search_wkt_polygon`). Understand structural hierarchies immediately by querying parent containers like malls or industrial complexes (`lookup_parent_polygon`).
- **Pedestrian and Mobility Insights** — Audit recent visit metrics, dwell times, and absolute foot traffic measurements attached to individual structures leveraging historical aggregation points (`lookup_place_patterns`).
- **Native GraphQL Exploration** — Pass perfectly structured GraphQL queries straight to the root mapping infrastructure for fully-unlocked edge cases (`graphql_raw_query`). Request and resolve bulk Placekeys efficiently on demand (`batch_lookup_placekeys`).

### How it works

1. Install this SafeGraph mapping block into your AI workspace.
2. Sign into the SafeGraph Dashboard environment.
3. Request or generate a valid GraphQL API Key within your workspace settings.
4. Input that key securely. Chat instantly: "Find all coffee shop POIs located within a 500-meter radius around longitude -122.33, latitude 47.60."


## Available Tools (10)
- **batch_lookup_placekeys**: Provide them as a JSON array.

Performs multiple Placekey lookups in a single request
- **graphql_raw_query**: Provide the query string and optional variables.

Executes a raw GraphQL query against the SafeGraph API
- **lookup_building_geometry**: Retrieves the building footprint (polygon) for a specific Placekey
- **lookup_parent_polygon**: Identifies the parent Placekey for a location (e.g., mall or airport)
- **lookup_place_patterns**: Retrieves historical foot traffic patterns for a specific Placekey
- **lookup_placekey**: Retrieves detailed attributes for a specific location by its Placekey
- **search_brand_places**: g., "Starbucks") in a specific city.

Searches for locations of a specific brand in a city
- **search_distance_radius**: Specify lat, lon, and radius in meters.

Searches for places within a specific radius from a point
- **search_industry_naics**: Searches for places by NAICS industry code and region
- **search_wkt_polygon**: Finds all places within a specific geometric polygon (WKT)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SafeGraph** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all the Starbucks branches strictly inside the city of Seattle, WA."

**🤖 AI Agent:**
> I've successfully queried SafeGraph places. Found 50 highly visible Starbucks locations associated inside Seattle, providing the unique Placekey IDs sequentially for each site mapped correctly.

---

**👤 You:**
> "Check what the detailed building geometry polygon is for Placekey '22m-xyz-1234'."

**🤖 AI Agent:**
> I executed a targeted building geometry lookup securely. The geometric bounding lines forming the structure of site '22m-xyz-1234' are POLYGON((-122.123 47.982, ...)), completely reflecting its physical real-world footprint mapped securely.

---

**👤 You:**
> "Can you gather the historical pedestrian traffic patterns evaluating typical visit frequencies around Placekey '123-abc-987'?"

**🤖 AI Agent:**
> The foot traffic data has been cleanly retrieved from the registry! Based on safe historical compilations, this location captures an approximate volume of 12,000 visitors routinely holding a median dwell time reaching precisely 45 minutes on active days.


## ❓ FAQ

**Q: Can I manipulate or delete existing POIs present inside the global SafeGraph spatial indexes?**
No. The AI interacts safely with the GraphQL API strictly on a 'read-only' query-bound basis. It has absolutely no inherent capability to corrupt or perform unauthorized destructive operations such as erasing core places or overwriting coordinates in your environment.

**Q: Are geometric polygons always provided for queried structures automatically?**
No, they must be explicitly queried utilizing the `lookup_building_geometry` functionality along with a verified Placekey, or structured thoroughly using the standard GraphQL command when available. Otherwise most basic list operations only return textual descriptors and simple pinpoint latitude/longitude figures.

**Q: Does the AI download huge databases directly into my storage limit when filtering large geographical boundary ranges (WKT)?**
The integration employs a managed response methodology natively implemented through GraphQL constraints. The output responses are strictly paginated securely filtering hundreds of points effectively rather than attempting to sync gigabytes directly to the chatbot at once.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/safegraph](https://vinkius.com/mcp/safegraph)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SafeGraph** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `safegraph` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SafeGraph** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "safegraph": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
