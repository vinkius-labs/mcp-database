# Georef Argentina MCP Server

Access official Argentine geographic data—normalize addresses, list administrative divisions, and perform reverse geocoding directly from your AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/georef-argentina)

## Overview
**Category:** data-management
**Tools Count:** 7

## Description
Connect your AI agent to the official **Georef Argentina** service to access precise geographic and administrative information. This server allows you to interact with the national database of provinces, departments, municipalities, and streets.

### What you can do

- **Administrative Hierarchy** — List and filter provinces, departments, and municipalities by name or ID using `get_provincias`, `get_departamentos`, and `get_municipios`.
- **Address Normalization** — Convert messy address strings into structured data with precise components using `normalize_direccion`.
- **Street Database** — Search for specific streets (vías) within any locality or department using `get_vias`.
- **Reverse Geocoding** — Provide latitude and longitude to identify the exact administrative location with `reverse_geocoding`.
- **Data Enrichment** — Fetch centroids and metadata for geographic entities to power maps and analytics.

### How it works

1. Subscribe to this server
2. Enter your Georef API Key (if required for high-volume access)
3. Start querying Argentine geography from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Delivery** — Normalize customer addresses to ensure accurate shipping and routing.
- **Data Analysts** — Clean and categorize datasets containing Argentine location information.
- **Developers** — Integrate official government geographic data without manual scraping or complex API setups.


## Available Tools
- **get_departamentos**: Get a list of departments in Argentina
- **normalize_direccion**: g., "Av. Mayo 100").

Normalize a full address string into its components
- **get_localidades**: Get a list of localities in Argentina
- **get_municipios**: Get a list of municipalities in Argentina
- **get_provincias**: Can filter by ID or name.

Get a list of provinces in Argentina
- **reverse_geocoding**: ) for lat/lon.

Get geographic location for a given set of coordinates
- **get_vias**: Get a list of streets (vías) in Argentina


## Installation & Usage

To install and use the **Georef Argentina** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/georef-argentina](https://vinkius.com/mcp/georef-argentina)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
