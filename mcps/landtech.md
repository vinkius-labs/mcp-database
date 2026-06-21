# LandTech MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/landtech)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/landtech-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/landtech-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Research land ownership, planning applications, and property development opportunities with geospatial intelligence tools.

## Description
Connect your **LandTech** account to any AI agent and access property intelligence through natural conversation.

### What you can do

- **Land Search** — Search parcels by location, size, and zoning criteria
- **Ownership Analysis** — Browse ownership records and title information
- **Planning Applications** — Track planning permissions and application status
- **Site Assessment** — Access environmental, flood risk, and constraint data
- **Development Tracking** — Monitor construction activity and project pipelines

### How it works

1. Subscribe to this server
2. Enter your LandTech API Key
3. Start searching properties from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Property Developers** — search for development sites and track planning
- **Estate Agents** — access land data and ownership information
- **Planners** — monitor applications and constraints


## Available Tools
- **get_api_status**: Check connection
- **get_price_comparables**: Find similar sales
- **get_site_constraints**: Check development risks
- **get_real_estate_market_data**: Get regional insights
- **get_planning_details**: Get planning info
- **get_planning_policy**: Get policy details
- **get_building_data**: Get property-level info
- **get_ownership_title**: Get property title info
- **list_local_authority_plans**: List regional policies
- **list_saved_sites**: List portfolio sites
- **search_land_parcels**: Find land for development
- **search_urban_planning**: Find planning applications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LandTech** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for development sites over 2 acres in London with residential zoning."

**🤖 AI Agent:**
> 12 sites found (>2 acres, residential zoning, London). Top: 1) Wandsworth — 3.2 acres, £8.5M guide, owner: Development Trust Ltd. 2) Hackney — 2.8 acres, £12M, greenfield. 3) Lewisham — 2.1 acres, £6.2M, brownfield (former industrial). Flood risk: Low (10 sites), Medium (2). Planning history: 8 sites with prior applications.

---

**👤 You:**
> "Show ownership details and planning history for the Wandsworth site."

**🤖 AI Agent:**
> Wandsworth site (3.2 acres): Owner: Development Trust Ltd (since 2019). Title: FH. Previous: Southbank Properties (2015-2019). Planning: 2 applications. 1) 2022 — 'Mixed-use development, 120 units + retail' — Approved ✅. 2) 2020 — 'Residential 80 units' — Withdrawn. Constraints: Conservation area buffer (partial), Tree Preservation Order (2 trees). Flood risk: Low. Transport: Zone 3.

---

**👤 You:**
> "List recent planning applications in Hackney and show environmental constraints."

**🤖 AI Agent:**
> Hackney planning (last 90 days): 14 applications. Approved: 8. Pending: 4. Refused: 2. Major: 'King's Row — 200 units' (pending, 2.8 acres). Environmental: Air quality: Moderate. Noise: AQMA zone. Green space: 15% requirement. Heritage: 3 listed buildings nearby. Biodiversity: Net gain required.


## Installation & Usage

To install and use the **LandTech** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/landtech](https://vinkius.com/mcp/landtech)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
