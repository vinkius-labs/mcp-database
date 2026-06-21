# FRED Full Access — U.S. Economic Intelligence MCP Server

The ultimate U.S. economic data Mega-Server: 19 tools covering time series, releases, categories, regional GeoFRED data, tags, and 107 data sources — 816,000+ series from the Federal Reserve in one integration.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fred-full-access-us-economic-intelligence)

## Overview
**Category:** the-unthinkable
**Tools Count:** 19

## Description
The **definitive Mega-Server** for U.S. economic intelligence. Why install 5 servers when one does it all?

### What you can do
- **📊 Series (5 tools)** — Search, retrieve data, metadata, updates, and vintage revisions for 816,000+ time series
- **📰 Releases (4 tools)** — Track economic data releases, dates, and discover series within each release
- **📁 Categories (4 tools)** — Navigate the FRED taxonomy tree to discover and filter data
- **🗺 GeoFRED (3 tools)** — Regional economic data by state, county, MSA, and Fed district
- **🏷 Tags & Sources (3 tools)** — Intelligent tag-based discovery + all 107 official data providers

### Popular Series
`GDP` · `UNRATE` · `CPIAUCSL` · `FEDFUNDS` · `DGS10` · `SP500` · `M2SL` · `MORTGAGE30US`

### Who is this for?
Power users, macro analysts, and AI agents that need comprehensive U.S. economic intelligence without managing multiple integrations.


## Available Tools
- **search_series**: Returns matching series with title, frequency, units, popularity. Use order_by=popularity to find the most-used series.

Search 816,000+ economic time series by keyword
- **get_category**: Key: 32991 (Money/Banking), 10 (Employment), 32992 (National Accounts), 32455 (Prices).

Get a FRED category by ID
- **get_category_children**: Start from root (0) to explore top-level categories.

Get child categories of a category
- **get_category_series**: Supports filtering by frequency, units, and tags.

Get series within a category
- **get_category_tags**: Get tags for a category
- **get_regional_data**: Use get_series_group first to find the series_group ID.

Get cross-sectional regional economic data
- **get_series_group**: Enter a FRED series ID to discover the group ID.

Get series group info for GeoFRED
- **get_geo_shapes**: Shapes: bea, msa, frb, necta, state, country, county, censusregion.

Get geographic shape files for mapping
- **search_tags**: Search or browse FRED tags
- **get_series_by_tags**: Example: usa;gdp returns US GDP series.

Get series matching specific tags
- **list_sources**: List all FRED data sources
- **get_series**: Use IDs like GDP, UNRATE, CPIAUCSL, FEDFUNDS, DGS10.

Get metadata for a specific FRED series
- **get_observations**: Supports date filtering, unit transformations (pch, log), and frequency aggregation.

Get actual data values for a FRED time series
- **get_series_updates**: Filter by macro or regional.

Get recently updated FRED series
- **get_vintage_dates**: Essential for ALFRED-style vintage analysis.

Get historical revision dates for a series
- **list_releases**: List all FRED economic data releases
- **get_release**: IDs: 10 (Employment), 53 (GDP), 46 (CPI).

Get details for a specific release
- **get_release_dates**: Omit release_id for full economic calendar.

Get release dates for economic data
- **get_release_series**: Release 10 contains UNRATE, PAYEMS, and hundreds more.

Get all series within a release


## Installation & Usage

To install and use the **FRED Full Access — U.S. Economic Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fred-full-access-us-economic-intelligence](https://vinkius.com/mcp/fred-full-access-us-economic-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
