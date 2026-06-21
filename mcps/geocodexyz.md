# Geocode.xyz MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/geocodexyz)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Convert addresses to coordinates, perform reverse geocoding, and extract location data from text with Geocode.xyz.

## Description
Empower your AI agent with global geographic intelligence using the **Geocode.xyz** MCP server. This integration provides a robust suite of tools for mapping, location extraction, and spatial analysis.

### What you can do

- **Forward Geocoding** — Convert any physical address, city, or landmark into precise latitude and longitude coordinates.
- **Reverse Geocoding** — Identify the nearest physical address or point of interest for any set of GPS coordinates.
- **Geoparsing** — Automatically scan and extract geographic location names from unstructured blocks of text or documents.
- **IP Geolocation** — Determine the physical location, city, and country associated with a specific IP address.
- **Smart Autocomplete** — Get suggestions for partial street names, postal codes, or cities to improve data entry accuracy.

### How it works

1. Subscribe to this server
2. Enter your Geocode.xyz API Key
3. Start querying location data directly from your AI assistant

### Who is this for?

- **Data Analysts** — Enrich datasets with coordinates and regional metadata without manual lookups.
- **Logistics & Operations** — Quickly verify addresses and calculate coordinates for routing and delivery.
- **Content Creators** — Automatically tag locations mentioned in articles or social media posts using geoparsing.


## Available Tools
- **autocomplete**: Provide suggestions for partial street names, postal codes, or city names
- **forward_geocode**: Convert a place name or address into geographic coordinates
- **geoparse**: Uses POST under the hood for long text support.

Identify and extract location names from free-form text
- **ip_geolocation**: Locate an IP address geographically
- **reverse_geocode**: Convert latitude and longitude coordinates into a physical address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Geocode.xyz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the coordinates for 'The Colosseum in Rome'."

**🤖 AI Agent:**
> I've located the Colosseum. The coordinates are Latitude: 41.8902, Longitude: 12.4922.

---

**👤 You:**
> "What address is located at latitude 48.8584 and longitude 2.2945?"

**🤖 AI Agent:**
> The coordinates 48.8584, 2.2945 correspond to the Eiffel Tower, located at Champ de Mars, 5 Avenue Anatole France, 75007 Paris, France.

---

**👤 You:**
> "Extract all locations from this text: 'Our team is traveling from New York to London next week.'"

**🤖 AI Agent:**
> I've parsed the text and found two locations: 'New York' (USA) and 'London' (United Kingdom).


## ❓ FAQ

**Q: Can I extract multiple location names from a long paragraph of text?**
Yes! Use the `geoparse` tool. Provide the text in the `scantext` parameter, and the agent will identify and return all geographic locations mentioned within that text.

**Q: How do I find the address for a specific set of GPS coordinates?**
Use the `reverse_geocode` tool. Simply provide the `lat` (latitude) and `long` (longitude) values, and the server will return the closest physical address.

**Q: Is it possible to locate a user based on their IP address?**
Yes, the `ip_geolocation` tool allows you to input an IP address and retrieve the associated city, region, and country data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geocodexyz](https://vinkius.com/mcp/geocodexyz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Geocode.xyz** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `geocodexyz` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Geocode.xyz** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "geocodexyz": {
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
