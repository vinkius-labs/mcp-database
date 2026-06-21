# FRED GeoFRED — Regional Economic Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fred-geofred-regional-economic-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fred-geofred-regional-economic-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fred-geofred-regional-economic-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Access regional economic data for every U.S. state, county, metro area, and Federal Reserve district — unemployment by state, median income by MSA, GDP by county, all from the official GeoFRED database.

## Description
Compare economic performance across U.S. regions. GeoFRED turns national time series into cross-sectional geographic data.

### What you can do
- **Regional Snapshots** — Unemployment, income, poverty, housing prices per state, county, or MSA
- **Series Groups** — Discover which geographic breakdowns exist for any FRED series
- **Shape Data** — Get GeoJSON-compatible boundaries for mapping

### Region Types
`state` · `county` · `msa` · `bea` (Bureau of Economic Analysis) · `frb` (Federal Reserve District) · `censusregion`

### Who is this for?
Real estate analysts, location intelligence platforms, regional economists, policy makers, and anyone building geographic economic dashboards.


## Available Tools
- **get_regional_data**: Use get_series_group first to find the series_group ID for a FRED series. Region types: state, county, msa, bea, frb, necta, country, censusregion.

Get cross-sectional regional economic data
- **get_series_group**: Enter a FRED series ID (e.g., UNRATE for unemployment) to discover the series_group ID, available region types, units, and seasonality.

Get series group info for GeoFRED mapping
- **get_geo_shapes**: Shape values: bea, msa, frb, necta, state, country, county, censusregion.

Get geographic shape files for mapping


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FRED GeoFRED — Regional Economic Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the unemployment rate by state?"

**🤖 AI Agent:**
> 📊 **Unemployment Rate by State (Latest)**

| State | Rate |
|-------|------|
| Nevada | 5.4% |
| DC | 5.2% |
| California | 5.1% |
| ...national avg... | 3.7% |
| South Dakota | 2.0% |
| Vermont | 1.9% |
| North Dakota | 1.8% |

51 regions returned from GeoFRED.

---

**👤 You:**
> "Compare median household income across metro areas"

**🤖 AI Agent:**
> 💵 **Median Household Income — Top 5 MSAs**

1. San Jose-Sunnyvale: $145K
2. Washington-Arlington: $118K
3. San Francisco-Oakland: $115K
4. Seattle-Tacoma: $105K
5. Boston-Cambridge: $102K

National median: $75K

---

**👤 You:**
> "Get the geographic boundaries for U.S. states"

**🤖 AI Agent:**
> 🗺 **State Boundaries — GeoJSON**

Returned shape data for all 50 states + DC.
Includes: FIPS codes, state names, boundary coordinates.

Use with regional data to build choropleth maps.


## Installation & Usage

To install and use the **FRED GeoFRED — Regional Economic Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fred-geofred-regional-economic-data](https://vinkius.com/mcp/fred-geofred-regional-economic-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
