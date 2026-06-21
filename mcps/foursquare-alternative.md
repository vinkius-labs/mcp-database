# Foursquare MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/foursquare-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Manage your location data — audit places, photos, and tips via AI.

## Description
Empower your AI agent to orchestrate your entire location-based intelligence with **Foursquare**, the world's most trusted independent location data platform. By connecting Foursquare to your agent, you transform complex venue discovery into a natural conversation. Your agent can instantly search for places, audit venue metadata, and retrieve customer tips without you ever touching a dashboard. Whether you are conducting market research or managing a localized service, your agent acts as a real-time location scout, ensuring your data is always relevant and precise.

### What you can do

- **Place Auditing** — Search for venues by name, category, or coordinates and retrieve detailed metadata, including addresses and categories.
- **Visual Insights** — List place photos to understand the aesthetic and environment of any venue instantly.
- **Customer Oversight** — Query community tips and reviews to understand public sentiment and venue highlights.
- **Autocomplete Intelligence** — Retrieve real-time naming suggestions to ensure your location queries are always accurate.
- **Geographic Discovery** — Find nearby places based on coordinates to maintain a clear view of any local ecosystem.

### How it works

1. Subscribe to this server
2. Enter your Foursquare API Key
3. Start managing your location data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Market Researchers** — monitor venue distributions and category trends straight from your workflow.
- **Operations Leads** — verify if localized services are correctly identified and categorized in specific regions.
- **Travel Planners** — perform rapid audits of nearby places and retrieve top-rated tips without manual searches.
- **Business Analysts** — automate location querying to orchestrate cross-functional geographic strategy smoothly.


## Available Tools
- **autocomplete_places**: Get autocomplete suggestions for place names
- **get_nearby_places**: Find nearby places based on coordinates
- **get_place_details**: Get details for a specific place
- **get_place_photos**: Get photos for a specific place
- **get_place_tips**: Get tips and reviews for a specific place
- **list_categories**: List all Foursquare venue categories
- **search_places**: Search for places on Foursquare


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Foursquare** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for coffee shops near 'New York, NY'."

**🤖 AI Agent:**
> I've found several coffee shops in New York. Top results include 'Blue Bottle Coffee' and 'Stumptown Coffee Roasters'. Would you like the addresses for any of them?

---

**👤 You:**
> "Show me tips for place ID 4b2af3d6f964a520..."

**🤖 AI Agent:**
> I've retrieved 5 tips for this venue. Customers recommend the 'espresso' and mentioned the 'cozy seating area'. Would you like to see the full list?

---

**👤 You:**
> "Get nearby places for lat 40.7, long -74.0."

**🤖 AI Agent:**
> Finding nearby venues... I've identified several places within 1km, including a 'Fitness Center' and a 'Library'. Would you like the full categories and details?


## ❓ FAQ

**Q: How do I find my Foursquare API Key?**
Log in to the [**Foursquare Developer Console**](https://foursquare.com/developers/apps), create a Project, and you will find your API Key there. Copy and paste it into the field below.

**Q: Can the agent search for places near me?**
Yes. Use the `search_places` tool providing the `ll` (latitude, longitude) or `near` (city name) parameters. Your agent will return matching venues instantly.

**Q: Is it possible to retrieve venue photos via the agent?**
Yes. The `get_place_photos` tool allows your agent to fetch images for any venue by providing its Foursquare Place ID, helping you visualize the location.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/foursquare-alternative](https://vinkius.com/mcp/foursquare-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Foursquare** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `foursquare-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Foursquare** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "foursquare-alternative": {
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
