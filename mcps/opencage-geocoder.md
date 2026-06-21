# OpenCage Geocoder MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opencage-geocoder)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/opencage-geocoder-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/opencage-geocoder-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Convert addresses to coordinates and coordinates to addresses worldwide with the OpenCage Geocoding API.

## Description
Connect the **OpenCage Geocoder** to your AI agent for high-precision global geocoding and reverse geocoding. This server allows your agent to translate between human-readable addresses and geographic coordinates using a single, reliable API.

### What you can do

- **Forward Geocoding** — Convert any address, city, or landmark into precise latitude and longitude coordinates.
- **Reverse Geocoding** — Provide coordinates and receive a formatted, human-readable address with detailed location metadata.
- **Global Coverage** — Access data from multiple open sources (OpenStreetMap, Twofishes, etc.) covering the entire globe.
- **Road Information** — Optionally retrieve specific road data, including nearest road matching and road-specific attributes.
- **Localization** — Get results in specific languages or formats to suit your application's needs.

### How it works

1. Subscribe to this server
2. Enter your OpenCage API Key
3. Start asking your agent for location data, map coordinates, or address lookups

### Who is this for?

- **Developers** — Integrate location data into apps without managing complex geospatial databases.
- **Data Analysts** — Clean and enrich datasets with precise geographic information.
- **Logistics Teams** — Verify addresses and calculate coordinates for routing and delivery services.


## Available Tools
- **forward_geocode**: Forward geocode an address or placename to coordinates
- **reverse_geocode**: Reverse geocode coordinates to an address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenCage Geocoder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the coordinates for the Eiffel Tower in Paris?"

**🤖 AI Agent:**
> I've geocoded the Eiffel Tower. The coordinates are Latitude 48.85837, Longitude 2.29448. It is located at Champ de Mars, 5 Avenue Anatole France, 75007 Paris, France.

---

**👤 You:**
> "What is the address at latitude 52.51627 and longitude 13.37772?"

**🤖 AI Agent:**
> The address for those coordinates is Brandenburger Tor, Pariser Platz, 10117 Berlin, Germany.

---

**👤 You:**
> "Find 'Main Street' but only in the United Kingdom and return the result in French."

**🤖 AI Agent:**
> Searching for 'Main Street' in the UK... I found a primary result: Main Street, Gibraltar, Royaume-Uni (Note: Gibraltar is a British Overseas Territory). Would you like to see other matches within the UK?


## Installation & Usage

To install and use the **OpenCage Geocoder** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opencage-geocoder](https://vinkius.com/mcp/opencage-geocoder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
