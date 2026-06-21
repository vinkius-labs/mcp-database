# FCC Geo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fcc-geo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fcc-geo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fcc-geo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [telecommunications](../categories/telecommunications.md)

Instantly convert geographic coordinates into precise US Census Blocks and Telecommunication zones with zero authentication.

## Description
The **FCC Geo MCP Server** connects your AI agent directly to the United States Federal Communications Commission's geographic intelligence endpoints. Completely frictionless and requiring zero API keys, it provides instant spatial intersection analysis.

### Core Capabilities

- **Census Block Resolution** — Convert any latitude and longitude across the US into precise State, County, and Census Block FIPS codes.
- **Telecom Territorial Mapping** — Discover precisely which Cellular Market Areas (CMA), Economic Area Groupings (EAG), and spectrum licensing zones overlap with any physical location.
- **Zero-Friction Access** — Fully open and unmetered endpoints, removing all authentication barriers for immediate geospatial data engineering.

Ideal for real estate analysts, logistics AI systems, urban planners, and spectrum licensing researchers needing instantaneous conversion from coordinates to official US government zones.


## Available Tools
- **get_census_block_by_lat_lon**: Essential for mapping physical spaces to regulatory regions.

Convert exact geographic coordinates into US Census Blocks, Counties, and FIPS codes
- **get_fcc_areas_by_lat_lon**: Retrieve FCC telecommunication boundaries (CMA, PEA, EAG) intersecting given coordinates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FCC Geo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the Census Block for coordinates 40.0 latitude and -85.0 longitude."

**🤖 AI Agent:**
> I've checked the FCC geodatabase. Those coordinates correspond to Wayne County in Indiana (State FIPS 18, County FIPS 18177). The exact Census Block FIPS code is 181770103002008.

---

**👤 You:**
> "Which telecommunication economic areas overlap with coordinates 40, -85?"

**🤖 AI Agent:**
> According to the FCC Area boundaries, coordinates 40.0, -85.0 fall under Cellular Market Area (CMA) 408, Major Economic Area (MEA) 019, and Economic Area Grouping (EAG) 704.

---

**👤 You:**
> "Convert the coordinate pair 34.05, -118.24 into proper Census details."

**🤖 AI Agent:**
> Checking the FCC Geo repository...
Coordinates map directly to California (State FIPS 06), Los Angeles County (County FIPS 06037). The block FIPS evaluates firmly to 060372074001004 natively effortlessly.


## Installation & Usage

To install and use the **FCC Geo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fcc-geo](https://vinkius.com/mcp/fcc-geo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
