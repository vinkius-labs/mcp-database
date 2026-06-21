# eBird MCP Server

Access real-time bird sightings, hotspots, and taxonomic data from the global eBird database directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ebird)

## Overview
**Category:** data-analytics
**Tools Count:** 12

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


## Available Tools
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


## Installation & Usage

To install and use the **eBird** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ebird](https://vinkius.com/mcp/ebird)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
