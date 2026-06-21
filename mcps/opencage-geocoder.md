# OpenCage Geocoder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opencage-geocoder)
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


## Available Tools (2)
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


## ❓ FAQ

**Q: Can I limit the search results to a specific country?**
Yes! Use the `countrycode` parameter in the `forward_geocode` tool with ISO 3166-1 alpha-2 codes (e.g., 'us' for USA, 'br' for Brazil) to restrict results to that territory.

**Q: How do I get the address of a specific set of coordinates?**
Use the `reverse_geocode` tool by providing the `lat` (latitude) and `lng` (longitude). The agent will return the most accurate formatted address found for those coordinates.

**Q: Can I get information about the nearest road to a location?**
Yes. By setting the `roadinfo` parameter to true in either `forward_geocode` or `reverse_geocode`, the API will attempt to match the location to the nearest road and include road-specific data in the response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opencage-geocoder](https://vinkius.com/mcp/opencage-geocoder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenCage Geocoder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `opencage-geocoder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenCage Geocoder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opencage-geocoder": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
