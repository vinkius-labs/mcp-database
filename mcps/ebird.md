# eBird MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ebird)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time bird sightings, hotspots, and taxonomic data from the global eBird database directly from your AI agent.

## Description
Transform your AI into an expert ornithology assistant. This MCP server provides a direct bridge to the Cornell Lab of Ornithology's eBird API, the world's most comprehensive source of bird observation data.

### What you can do

- **Real-time Sightings** — Query recent observations by region (country, state, county) or specific species codes using `get_recent_observations` and `get_recent_observations_by_species`.
- **Nearby Discovery** — Use GPS coordinates to find birds currently being seen around you or within a specific radius with `get_recent_nearby_observations`.
- **Hotspot Analysis** — Identify the best birding locations in any given region to plan trips or research using `get_hotspots_in_region` or `get_nearby_hotspots`.
- **Checklist Details** — Inspect specific checklists to see full trip reports and species counts with `get_checklist` and `get_recent_checklists`.
- **Taxonomy & Regions** — Access the eBird/Clements taxonomy and sub-region information to understand species relationships and geographic boundaries.

### How it works

1. Subscribe to this server
2. Enter your eBird API Token
3. Start exploring global biodiversity data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Scientists** — Instantly retrieve observation data for specific regions or species to support biodiversity studies.
- **Birdwatchers & Enthusiasts** — Find out what's being seen nearby or at your next travel destination without leaving your chat interface.
- **Conservationists** — Monitor recent sightings and checklist activity in critical habitats and hotspots.


## Available Tools (12)
- **get_checklist**: Get checklist details
- **get_hotspots_in_region**: Get hotspots in a region
- **get_nearby_hotspots**: Get nearby hotspots
- **get_recent_checklists**: Get recent checklists in a region
- **get_recent_nearby_observations**: Get recent nearby observations
- **get_recent_observations_by_species**: Get recent observations of a species in a region
- **get_recent_observations**: g., country, state, or county).

Get recent observations in a region
- **get_region_info**: Get region info
- **get_sub_regions**: g., states within a country).

List sub-regions
- **get_taxonomic_groups**: Get taxonomic groups
- **get_taxonomy**: Get eBird taxonomy
- **get_top_100**: Get top 100 observers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **eBird** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get recent bird observations for the region US-NY."

**🤖 AI Agent:**
> I've retrieved the latest sightings for New York. Notable observations include a Snowy Owl in Central Park and several Pine Grosbeaks in the Adirondacks. Would you like the full list of species?

---

**👤 You:**
> "Find recent sightings of species 'pingro' in region US-NY."

**🤖 AI Agent:**
> Searching for Pine Grosbeak (pingro) in New York... I found 3 recent observations. The most recent was at Saratoga Spa State Park on October 24th. Do you want the specific location details?

---

**👤 You:**
> "List birding hotspots in the region US-FL."

**🤖 AI Agent:**
> I've identified several top hotspots in Florida, including Everglades National Park (L128523) and Fort De Soto Park (L109156). Which one would you like to explore for recent sightings?


## ❓ FAQ

**Q: How do I find recent sightings of a specific bird species in my area?**
Use the `get_recent_observations_by_species` tool. Provide the `regionCode` (e.g., 'US-NY') and the `speciesCode` (e.g., 'pingro' for Pine Grosbeak) to see the latest reports.

**Q: Can I find birding locations near my current GPS coordinates?**
Yes, use `get_recent_nearby_observations` with your latitude and longitude. You can also use `get_nearby_hotspots` to find established birding locations within a specific radius.

**Q: How do I get information about a specific region's birding activity?**
Use `get_region_info` for general data or `get_recent_checklists` to see the most recent trip reports submitted by birders in that region.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ebird](https://vinkius.com/mcp/ebird)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **eBird** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ebird` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **eBird** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ebird": {
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
