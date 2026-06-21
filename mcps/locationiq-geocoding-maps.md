# LocationIQ (Geocoding & Maps) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/locationiq-geocoding-maps)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Build with location data via LocationIQ — geocode addresses, calculate routes, and perform reverse lookups.

## Description
Connect your **LocationIQ** account to any AI agent and take full control of affordable geocoding, routing, and geospatial intelligence through natural conversation.

### What you can do

- **Geocoding & Search** — Convert address strings into precise GPS coordinates and use autocomplete to retrieve suggestions for partial location queries directly from your agent
- **Reverse Geocoding** — Convert latitude and longitude coordinates into human-readable addresses, including precise postal data and localized language translations
- **Advanced Routing** — Calculate optimal driving, walking, or cycling paths between multiple coordinates with support for OSRM-based navigation instructions
- **Distance Matrices** — Compute travel duration and distance tables between multiple origins and destinations to optimize logistics and delivery workflows
- **Road Snapping** — Perfectly align messy GPS signals to the exact street network using native snapping configurations for accurate fleet tracking
- **Geo-Fencing & Filtering** — Restrict searches within specific country ISO codes or geographic bounding boxes to ensure data relevancy and regional compliance

### How it works

1. Subscribe to this server
2. Enter your LocationIQ API Key
3. Start building location-aware applications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Developers** — integrate geocoding and routing services into AI agents and validate coordinate results through natural conversation
- **Logistics Managers** — calculate optimal routes and distance matrices for delivery fleets without manual GIS software
- **Data Analysts** — clean and enrich datasets with precise geolocation and postal address metadata efficiently


## Available Tools
- **search_autocomplete**: php` tracking prefix queries and parsing city datasets quickly.

Retrieve autosuggest lists for partial location search queries
- **check_account_balance**: php` verifying explicitly how many OpenStreetMap queries remain for the Tenant API Key.

Validate current LocationIQ account balance and remaining requests
- **calculate_directions**: Calculate optimal driving, walking, or cycling route between coordinates
- **calculate_distance_matrix**: Calculate travel duration table crossing multiple coordinate sources and destinations
- **snap_nearest_roads**: Snap a coordinate perfectly to the exact street network
- **reverse_geocode**: php` pulling standard Place objects formatting explicit postal addresses over GPS positions.

Convert latitude and longitude coordinates into a human-readable address
- **reverse_language_bias**: Reverse Geocode lat/lon mapping translations inside specific native language tags
- **search_geocode**: php` mapping address strings into specific OpenStreetMap coordinates securely.

Convert an address string into latitude and longitude coordinates
- **search_bounding_box**: Search explicitly bounded within a geographical map rectangle
- **search_country_filter**: Search address coordinates forced within explicit Country codes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LocationIQ (Geocoding & Maps)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the coordinates for the 'Eiffel Tower' in Paris"

**🤖 AI Agent:**
> Resolving address… I've found the Eiffel Tower at latitude 48.8584 and longitude 2.2945. The address is 5 Avenue Anatole France, 75007 Paris, France. Would you like me to find nearby hotels?

---

**👤 You:**
> "What is the best driving route from Lisbon to Porto?"

**🤖 AI Agent:**
> Calculating directions… The optimal route via A1 is approximately 312 km and will take about 2 hours and 55 minutes with current traffic. I can provide the detailed turn-by-turn instructions if you'd like.

---

**👤 You:**
> "Check my remaining LocationIQ request balance"

**🤖 AI Agent:**
> Retrieving balance… You have 4,850 requests remaining out of your 5,000 daily limit. Your account is in good standing. Would you like me to perform any more geocoding lookups?


## ❓ FAQ

**Q: Can I convert GPS coordinates back to a physical address using my agent?**
Yes. Use the `reverse_geocode` tool by providing the latitude and longitude. Your agent will return the human-readable address, including the house number, street, city, and postal code.

**Q: How do I calculate the travel time between multiple points?**
The `calculate_distance_matrix` tool allows you to submit a list of coordinates. Your agent will return a duration table for the specified profile (driving or walking), helping you optimize multi-stop routes.

**Q: Can my agent check how many API requests I have remaining?**
Absolutely. Use the `check_account_balance` tool to retrieve your current credit status. Your agent will report exactly how many OpenStreetMap queries remain for your API key during the current period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/locationiq-geocoding-maps](https://vinkius.com/mcp/locationiq-geocoding-maps)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LocationIQ (Geocoding & Maps)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `locationiq-geocoding-maps` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LocationIQ (Geocoding & Maps)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "locationiq-geocoding-maps": {
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
