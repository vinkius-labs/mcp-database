# Bridge Data Output MCP Server

Access standardized real estate data via the Bridge API — browse MLS listings, property details, and agent info directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bridge-data-output)

## Overview
**Category:** real-estate
**Tools Count:** 10

## Description
Connect your **Bridge Interactive (Zillow Group)** account to any AI agent and orchestrate your real estate research, listing analysis, and market data workflows through natural conversation.

### What you can do

- **Listing Oversight** — Browse thousands of real estate listings (properties) from various MLS datasets with advanced OData filtering.
- **Property Deep Dives** — Retrieve detailed metadata for specific properties, including physical characteristics and historical values.
- **Directory Access** — List real estate members (agents) and offices associated with specific datasets.
- **Media Management** — Access links to high-resolution photos, virtual tours, and media associated with property listings.
- **Market Analysis** — Search for properties by city, price range, or recent modifications to track market trends.
- **Dataset Discovery** — List all available data systems (MLSs) your application has access to.

### How it works

1. Subscribe to this server
2. Enter your Bridge Server Token (Bearer)
3. Start exploring real estate markets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Real Estate Analysts** — quickly gather listing data for market reports without manual dashboard exports.
- **App Developers** — verify data structures and query logic using natural language.
- **Investment Teams** — monitor specific areas and price ranges for new opportunities.


## Available Tools
- **get_dataset_metadata**: Get schema metadata for a specific dataset
- **get_property**: Get details of a specific property
- **list_data_systems**: List all available real estate data systems (MLSs)
- **list_media**: List media (photos/videos) from a dataset
- **list_members**: List real estate agents (members) from a dataset
- **list_offices**: List real estate offices from a dataset
- **list_properties**: List properties from a specific dataset
- **list_recent_listings**: List the most recently modified properties
- **search_properties_by_city**: Search for properties in a specific city
- **search_properties_by_price**: Search for properties above a specific price


## Installation & Usage

To install and use the **Bridge Data Output** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bridge-data-output](https://vinkius.com/mcp/bridge-data-output)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
