# Google Maps MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-maps)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Empower location intelligence via Google Maps — perform geocoding, search millions of places, retrieve rich venue details, and calculate directions directly from any AI agent.

## Description
Connect your **Google Maps Platform** account to any AI agent and take full control of your geospatial intelligence, place discovery, and routing through natural conversation.

### What you can do

- **Geocoding Orchestration** — Convert physical addresses or location names into precise geographic coordinates (Latitude/Longitude) translating human readable locations into spatial API bounds flawlessly
- **Place Discovery** — Finds physical entities within Google Maps database matching text queries like 'Restaurants in New York', retrieving critical PlaceIDs for deep introspection natively
- **Rich Metadata Retrieval** — Retrieve deep details of specific places including phone numbers, user reviews, opening hours, and websites using PlaceIDs to bypass generic search arrays synchronously
- **Route & ETA Calculation** — Triggers routing engine identifying physical transit maps resolving directions, distance, and optimal time calculations between origin and destination bounds flawlessly
- **Travel Mode Support** — Execute directions queries for driving, walking, bicycling, or transit modes to verify travel logistics and ETAs synchronously across your environment
- **Geospatial Intelligence** — Analyze specific localized coordinates to verify presence and proximity of businesses or landmarks within the Google Maps ecosystem securely

### How it works

1. Subscribe to this server
2. Enter your Google Maps API Key (found in Google Cloud Console > Google Maps Platform > Credentials)
3. Start exploring the world from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel & Logistics Planners** — calculate routes and verify ETAs without manual map searches or distance calculations
- **Real Estate & City Analysts** — perform geocoding and search for nearby POIs to analyze location quality using natural language conversation
- **Support & Sales Teams** — quickly look up business details and verify location metadata to resolve customer inquiries in real-time
- **Developers** — test and debug location-based API parameters and verify PlaceID metadata schemas through natural conversation


## Available Tools (4)
- **geocode**: Convert an address or location name into precise geographic coordinates (Latitude / Longitude)
- **place_search**: Search for businesses, restaurants, or spots (e.g. "Pizza in New York", "Hospitals near me")
- **place_details**: Get deep details of a specific Place (Phone number, reviews, opening hours, website) using its PlaceID
- **directions**: Calculate ETA, distance, and optimal route directions between origin and destination


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Maps** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Geocode this address: '1600 Amphitheatre Pkwy, Mountain View, CA'"

**🤖 AI Agent:**
> Address geocoded! The coordinates for 1600 Amphitheatre Pkwy are Lat: 37.4223, Lng: -122.0841. These are the precise coordinates for the Googleplex headquarters.

---

**👤 You:**
> "Find pizza restaurants in Brooklyn and show me details for the best one"

**🤖 AI Agent:**
> Searching for pizza in Brooklyn... I found 10 results. The top-rated is 'L'Industrie Pizzeria' (Rating: 4.8, 2k+ reviews, PlaceID: abc-123). Retrieving details... They are open until 10 PM tonight and offer outdoor seating. Would you like their phone number?

---

**👤 You:**
> "Get directions from San Francisco to San Jose by train"

**🤖 AI Agent:**
> Calculating directions... By transit, the trip from San Francisco to San Jose takes approximately 1 hour and 15 minutes via Caltrain. Total distance is 48 miles. I can provide the specific line information and departure times for you.


## ❓ FAQ

**Q: Can my agent find the latitude and longitude of an address via Google Maps?**
Yes. Use the 'geocode' tool. Provide the physical address or location name, and the agent will translate the string into precise geographic coordinates required for spatial analysis flawlessly.

**Q: How do I get reviews and opening hours for a restaurant via chat?**
First, use 'place_search' to find the restaurant and its PlaceID. Then, use 'place_details' with that ID. Your agent will fetch the full payload including reviews, ratings, and operating hours natively.

**Q: Can I calculate the driving time between two cities through the agent?**
Absolutely. Use the 'directions' tool. Provide the origin and destination addresses and set the mode to 'driving'. The agent will return the distance and estimated time of arrival (ETA) synchronously.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-maps](https://vinkius.com/mcp/google-maps)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Maps** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `google-maps` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Maps** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-maps": {
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
