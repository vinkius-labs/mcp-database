# FRED Series — U.S. Economic Time Series MCP Server

Search and retrieve data from 816,000+ official U.S. economic time series: GDP, inflation, unemployment, interest rates, money supply — with built-in transformations, frequency aggregation, and vintage analysis.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fred-series-us-economic-time-series)

## Overview
**Category:** the-unthinkable
**Tools Count:** 5

## Description
Connect your AI agent to the **most powerful economic data engine in the world**. FRED Series gives you direct access to the Federal Reserve's complete time series database.

### What you can do
- **Search 816,000+ Series** — Find any economic indicator by keyword. GDP, CPI, unemployment rate, federal funds rate, housing starts, and hundreds of thousands more
- **Retrieve Observations** — Get actual date/value pairs with built-in unit transformations (percent change, log, year-over-year) and frequency aggregation (daily → monthly → quarterly → annual)
- **Series Metadata** — Full details: title, units, frequency, seasonal adjustment, observation range, source, and notes
- **Recent Updates** — Monitor which series were just updated — essential for tracking economic releases
- **Vintage Analysis** — Access ALFRED-style historical revisions to understand how data was revised over time

### Popular Series IDs
`GDP` · `UNRATE` · `CPIAUCSL` · `FEDFUNDS` · `DGS10` · `SP500` · `M2SL` · `MORTGAGE30US` · `DEXUSEU` · `T10YIE`

### Who is this for?
Quantitative analysts, economists, financial advisors, portfolio managers, data journalists, academic researchers, and anyone building AI agents that need authoritative U.S. economic data.


## Available Tools
- **search_series**: Returns matching series with title, frequency, units, popularity. Use order_by=popularity to find the most-used series. Examples: "GDP", "unemployment rate", "inflation CPI".

Search 816,000+ economic time series by keyword
- **get_series**: Use well-known IDs like GDP, UNRATE, CPIAUCSL, FEDFUNDS, DGS10, SP500, M2SL.

Get metadata for a specific FRED series
- **get_observations**: Supports date filtering, unit transformations (percent change, log, etc.), and frequency aggregation. This is the primary tool for retrieving economic data.

Get actual data values for a FRED time series
- **get_series_updates**: Useful for monitoring new data releases. Filter by macro (large/popular series) or regional.

Get recently updated FRED series
- **get_vintage_dates**: Essential for ALFRED-style vintage analysis and understanding data revisions.

Get historical revision dates for a series


## Installation & Usage

To install and use the **FRED Series — U.S. Economic Time Series** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fred-series-us-economic-time-series](https://vinkius.com/mcp/fred-series-us-economic-time-series)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
