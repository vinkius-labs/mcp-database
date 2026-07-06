# Skyscanner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/skyscanner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search flights worldwide — compare prices by date, find cheapest days to fly and discover flight routes.

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


## Available Tools (6)
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
- **autosuggest_places**: Useful for finding the correct place IDs to use in flight searches. Returns place names, IATA codes and types.

Search for places (airports, cities) by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Skyscanner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find flights from New York to London on June 15, 2025."

**🤖 AI Agent:**
> Found flights from $385 (British Airways), $412 (Virgin Atlantic), $438 (Delta). Cheapest days nearby: Jun 14 ($372), Jun 16 ($390).

---

**👤 You:**
> "What's the cheapest day to fly from São Paulo to Miami in July?"

**🤖 AI Agent:**
> Cheapest days in July: Jul 8 ($412), Jul 15 ($425), Jul 22 ($438). Most expensive: Jul 4 ($589), Jul 25 ($567). Mid-week flights are consistently cheaper.

---

**👤 You:**
> "What's the airport code for Tokyo?"

**🤖 AI Agent:**
> Tokyo airports: NRT (Narita Intl), HND (Haneda). City code: TYOA (both airports). Use TYOA for searches that include both airports.


## ❓ FAQ

**Q: Do I need an API key?**
No! Skyscanner's Travel API is free with a public key. No registration needed for basic access.

**Q: How do I find airport codes?**
Use autosuggest_places to search for airports and cities by name. It returns IATA codes and place IDs you can use in flight searches.

**Q: Are these real-time prices?**
Prices are indicative and cached. They're useful for exploring price ranges and comparing dates, but may differ slightly from live booking prices.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/skyscanner](https://vinkius.com/mcp/skyscanner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Skyscanner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `skyscanner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Skyscanner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "skyscanner": {
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
