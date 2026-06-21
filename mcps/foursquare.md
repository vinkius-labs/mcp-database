# Foursquare MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/foursquare)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Empower location intelligence via Foursquare — search millions of places, retrieve rich venue details and photos, and discover nearby POIs directly from any AI agent.

## Description
Connect your **Foursquare** account to any AI agent and take full control of your geospatial intelligence and place discovery workflows through natural conversation.

### What you can do

- **Place Discovery Orchestration** — Identify bounded routing spaces inside the headless Foursquare POI graph and extract explicitly attached REST arrays targeting specific search queries near any GPS pin
- **Rich Metadata Inspection** — Perform structural extraction of properties driving active node schemas, retrieving mega-document payloads including hours, ratings, and precise mapping arrays natively
- **Visual & Social Auditing** — Retrieve explicit cloud logging tracing media URL limits to compile dynamic image URLs and capture raw text sentiments left by humans to track venue quality
- **Geospatial Intelligence** — Execute immediate queries within custom drawn multi-point geometries or specific radius boundaries to find what exists physically adjacent to any target
- **Precise Venue Matching** — Dispatch automated validation checks routing explicit duplication logic to force Foursquare to confidently return exactly one node for ambiguous strings
- **Intelligent Autocomplete** — Provision highly-available JSON payloads generating fast typeaheads by querying partial letters to predict user intent natively
- **Taxonomy Oversight** — Enumerate explicitly attached structured rules exporting the entire official Foursquare classification tree to resolve internal type codes flawlessly

### How it works

1. Subscribe to this server
2. Enter your Foursquare API Key (found in the Foursquare Developer Console > Projects > API Keys)
3. Start exploring the world from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel & Logistics Planners** — search for venues and verify hours of operation without manual web searches
- **Real Estate & City Analysts** — audit POI density and venue quality within specific polygons using natural language
- **App Developers** — test and debug location-based search parameters and verify venue schemas through natural conversation
- **Marketing Researchers** — monitor foot traffic trends and user tips for specific store locations in real-time


## Available Tools (10)
- **autocomplete_venues**: Provision a highly-available JSON Payload generating fast typeaheads
- **list_venue_categories**: Enumerate explicitly attached structured rules exporting active Taxonomy
- **get_place_photos**: Retrieve explicit Cloud logging tracing explicit Media URL limits
- **get_place_details**: Perform structural extraction of properties driving active Node schemas
- **get_place_tips**: Identify precise active arrays spanning native User Reviews
- **match_venue_exactly**: Dispatch an automated validation check routing explicit Duplication logic
- **search_nearby_venues**: Inspect deep internal arrays mitigating specific Radius targets
- **search_within_polygon**: Retrieve the exact structural matching verifying Geofence alternatives
- **search_within_radius**: Irreversibly vaporize explicit validations extracting rich schema scopes
- **search_places**: Identify bounded routing spaces inside the Headless Foursquare POI graph


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Foursquare** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find coffee shops near '40.71, -74.00'"

**🤖 AI Agent:**
> Searching places... I found 10 coffee shops nearby. Top results include 'Blue Bottle Coffee' (0.2 miles away) and 'Everyman Espresso'. Would you like the detailed ratings or hours for 'Blue Bottle'?

---

**👤 You:**
> "What are the opening hours for 'Central Park Zoo'?"

**🤖 AI Agent:**
> Retrieving details for Central Park Zoo... They are open today from 10:00 AM to 5:00 PM. It is currently rated 4.5/5 by over 2,000 visitors. Would you like to see some recent photos of the zoo?

---

**👤 You:**
> "Show me user tips for 'The Met Museum'"

**🤖 AI Agent:**
> Retrieving tips... Visitors recommend: 'Go early to avoid crowds', 'Don't miss the Egyptian wing', and 'The rooftop view is incredible'. I found 50+ detailed tips for your visit.


## ❓ FAQ

**Q: Can my agent search for places within a specific drawn area (polygon)?**
Yes. Use the 'search_within_polygon' tool. Provide a coordinate string representing the multi-point geometry. The agent will analyze the localized boundaries and restrict the POI lookup strictly inside that drawn area.

**Q: How do I retrieve the opening hours and ratings for a venue via chat?**
Use the 'get_place_details' tool. Provide the Foursquare ID (fsq_id). The agent will fetch the full payload including operating hours, average ratings, and price levels natively from the places graph.

**Q: Can I see photos and user tips for a specific store through the agent?**
Absolutely. Use the 'get_place_photos' and 'get_place_tips' tools. Your agent will pull dynamic image URLs and capture raw text sentiments left by other visitors to help you evaluate venue quality flawlessly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/foursquare](https://vinkius.com/mcp/foursquare)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `foursquare` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Foursquare** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "foursquare": {
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
