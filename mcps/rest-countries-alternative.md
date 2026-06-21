# REST Countries MCP Server

Access comprehensive global data including country names, capitals, currencies, and languages via the REST Countries API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/rest-countries-alternative)

## Overview
**Category:** data-management
**Tools Count:** 12

## Description
Connect your AI agent to the **REST Countries** database to retrieve instant, accurate information about any nation or territory in the world. This server provides a powerful interface to query geographic, economic, and political data through natural conversation.

### What you can do

- **Comprehensive Search** — Find countries by common or official names, capital cities, or international codes (ISO 3166-1).
- **Economic & Linguistic Data** — Query countries based on the currencies they use or the languages spoken by their citizens.
- **Regional Filtering** — Browse nations by continent (Region) or specific subregions to analyze geographic clusters.
- **Demographics & Identity** — Search by demonyms (what citizens are called) or check independence status.
- **Localized Results** — Search for countries using translated names in various languages.

### How it works

1. Subscribe to this server
2. Since this is a public API, no specific token is required (enter 'public' if prompted)
3. Start asking about world geography and country statistics in Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts** — quickly gather country-level metadata for research and reporting
- **Developers** — verify ISO codes, currency formats, and language mappings without leaving the IDE
- **Educators & Students** — explore global facts and regional statistics through an interactive AI assistant


## Available Tools
- **get_all_countries**: You MUST specify the fields you need (up to 10) to avoid 400 Bad Request.

Retrieve information about all countries
- **search_by_capital**: Search by capital city
- **search_by_code**: Search by country code
- **search_by_codes**: Search for multiple countries by their codes
- **search_by_currency**: Search by currency code or name
- **search_by_demonym**: Search by demonym
- **filter_by_independent**: Filter by independence status
- **search_by_language**: Search by language code or name
- **search_by_name**: Search by country name
- **filter_by_region**: g., Africa, Americas, Asia, Europe, Oceania).

Filter countries by region
- **filter_by_subregion**: g., Northern Europe, South America).

Filter countries by subregion
- **search_by_translation**: Search by translation name


## Installation & Usage

To install and use the **REST Countries** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rest-countries-alternative](https://vinkius.com/mcp/rest-countries-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
