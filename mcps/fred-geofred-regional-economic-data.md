# FRED GeoFRED — Regional Economic Data MCP Server

Access regional economic data for every U.S. state, county, metro area, and Federal Reserve district — unemployment by state, median income by MSA, GDP by county, all from the official GeoFRED database.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fred-geofred-regional-economic-data)

## Overview
**Category:** brain-trust
**Tools Count:** 3

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


## Installation & Usage

To install and use the **FRED GeoFRED — Regional Economic Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fred-geofred-regional-economic-data](https://vinkius.com/mcp/fred-geofred-regional-economic-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
