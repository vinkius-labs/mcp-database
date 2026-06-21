# Zillow MCP Server

Access real estate data, Zestimates, and property details directly from Zillow — search addresses, get valuations, and analyze market trends.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zillow-alternative)

## Overview
**Category:** real-estate
**Tools Count:** 12

## Description
Connect your **Zillow** API access to any AI agent to retrieve comprehensive real estate data and property valuations through natural conversation.

### What you can do

- **Property Search** — Find specific properties using addresses and retrieve their unique Zillow Property IDs (ZPID) and basic Zestimates.
- **Deep Property Insights** — Access rich data including lot size, year built, bedroom/bathroom counts, and square footage for any target address.
- **Valuation & Zestimates** — Get the most recent Zestimate, valuation ranges, and rankings for millions of homes.
- **Market Comparisons** — Retrieve lists of comparable recent sales (comps) with detailed property data to understand local market value.
- **Visual Trends** — Generate URLs for historical Zestimate charts to visualize property value changes over 1, 5, or 10 years.
- **Demographics & Regions** — Fetch market affordability, real estate metrics, and demographic data for specific cities or neighborhoods.

### How it works

1. Subscribe to this server
2. Enter your Zillow Web Services ID (ZWSID)
3. Start querying real estate data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Real Estate Investors** — quickly analyze potential deals, check comps, and view historical value trends without manual searching.
- **Home Buyers & Sellers** — get instant Zestimates and detailed property facts to make informed decisions.
- **Data Analysts** — retrieve regional demographics and market metrics directly into your workflow.


## Available Tools
- **get_chart**: Generates a URL for an image file displaying historical Zestimates
- **get_comps**: Returns a list of comparable recent sales
- **get_deep_comps**: ) for both the principal and comparable properties.

Returns rich property data for comparable properties
- **get_deep_search_results**: ) in addition to standard search results.

Finds a property and returns rich property data
- **get_demographics**: Returns demographic data for a specified region
- **get_monthly_payments**: Returns estimated monthly payments
- **get_rate_summary**: Returns current mortgage rates
- **get_region_chart**: Generates a URL for an image file displaying historical Zestimates for a region
- **get_region_children**: g., neighborhoods within a city) for a specified region.

Returns a list of subregions for a specified region
- **get_search_results**: Finds a property for a specified address
- **get_updated_property_details**: Returns home facts edited by the owner or agent
- **get_zestimate**: Returns the most recent Zestimate for a ZPID


## Installation & Usage

To install and use the **Zillow** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zillow-alternative](https://vinkius.com/mcp/zillow-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
