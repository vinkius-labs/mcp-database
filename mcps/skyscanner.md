# Skyscanner MCP Server

Search flights worldwide — compare prices by date, find cheapest days to fly and discover flight routes.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/skyscanner)

## Overview
**Category:** productivity
**Tools Count:** 6

## Description
Connect to **Skyscanner** and explore flight prices worldwide through natural conversation — no API key needed.

### What you can do

- **Flight Search** — Search indicative flight prices between any two airports
- **Browse Dates** — Find cheapest days to fly around your preferred date
- **Browse Grid** — Compare prices across multiple date combinations
- **Direct Flights** — Find non-stop flight options only
- **Place Search** — Autosuggest airports and cities by name

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Explore flight prices from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travelers** — compare flight prices, find cheapest travel dates and plan trips
- **Travel Agents** — access flight pricing data for client recommendations
- **Flexible Travelers** — find cheapest days to fly with date browsing


## Available Tools
- **autosuggest_places**: Useful for finding the correct place IDs to use in flight searches. Returns place names, IATA codes and types.

Search for places (airports, cities) by name
- **browse_dates**: Useful for finding the cheapest days to fly. Returns prices for multiple dates at once.

Browse flight prices by date
- **browse_grid**: Useful for flexible date searches. Returns prices for multiple origin-destination date pairs.

Browse flight prices in a date grid
- **get_geo_places**: Useful for discovering available place IDs.

Get a list of all supported places
- **search_direct_flights**: Useful for travelers who prefer no layovers.

Search for direct flights only
- **search_flights_indicative**: Useful for exploring flight options and comparing prices. Use originPlaceId and destinationPlaceId as IATA codes (e.g. "NYCA" for New York, "LOND" for London) or place IDs. Returns cheapest quotes with carrier info.

Search for flight quotes (indicative prices)


## Installation & Usage

To install and use the **Skyscanner** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/skyscanner](https://vinkius.com/mcp/skyscanner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
