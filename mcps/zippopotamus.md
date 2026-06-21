# Zippopotam.us MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zippopotamus)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Global postal code intelligence — lookup city, state, and coordinates by zip code via AI.

## Description
Equip your AI agent with global geographic intelligence via the **Zippopotam.us** MCP server. This integration provides instant access to location data for over 60 countries. Your agent can perform reverse lookups of postal codes to retrieve city names, state details, and precise latitude/longitude coordinates. It can also find all postal codes associated with a specific city and state. Whether you are validating addresses, calculating distances, or automating logistics, your agent acts as a dedicated geographic data specialist through natural conversation.

### What you can do

- **Postal Code Lookup** — Retrieve city, state, and coordinates for any zip code in 60+ countries.
- **City Reverse Lookup** — Find all postal codes associated with a specific city and state.
- **Geographic Data** — Access precise latitude and longitude for localized mapping or services.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start querying postal data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Delivery Teams** — quickly verify city and state data from postal codes.
- **Developers** — integrate geographic lookups into their AI-driven applications.
- **Data Scientists** — access a reliable source of structured postal and coordinate data.


## Available Tools
- **lookup_nearby_city**: Lookup zip codes for a city
- **lookup_postcode**: Lookup location by postal code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zippopotam.us** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the city and state for zip code 90210 in the US."

**🤖 AI Agent:**
> The zip code 90210 corresponds to Beverly Hills, California (CA). I also have the exact coordinates: Latitude 34.0901, Longitude -118.4065.

---

**👤 You:**
> "Lookup the postal code 'SW1A 1AA' in Great Britain."

**🤖 AI Agent:**
> In Great Britain (GB), the postal code SW1A 1AA corresponds to London, England. This is the area for Buckingham Palace. The coordinates are 51.501, -0.1419.

---

**👤 You:**
> "List all postal codes for 'Miami', Florida (FL)."

**🤖 AI Agent:**
> Retrieving data for Miami... I've found a large list of zip codes including 33101, 33109, 33125, and many others. Would you like me to list them all or focus on a specific neighborhood?


## ❓ FAQ

**Q: Can I lookup a US zip code and get its coordinates?**
Yes! Use the `lookup_postcode` tool with the country 'US' and the zip code. It will return the city, state, and coordinates for that location.

**Q: Which countries are supported by Zippopotam.us?**
Zippopotam.us supports over 60 countries, including the US, Canada, Great Britain, Brazil, France, Germany, and many others. You can use the standard 2-letter ISO country codes.

**Q: Can I find all zip codes for a specific city?**
Yes! Use the `lookup_city` tool with the country code, state, and city name. It will return a list of all postal codes associated with that urban area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zippopotamus](https://vinkius.com/mcp/zippopotamus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zippopotam.us** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zippopotamus` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zippopotam.us** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zippopotamus": {
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
