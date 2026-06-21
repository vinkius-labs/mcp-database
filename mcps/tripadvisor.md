# TripAdvisor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tripadvisor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search hotels, restaurants, and attractions via TripAdvisor Content API — get reviews, ratings, and POI details.

## Description
Connect your AI agent to the world's largest travel platform. The TripAdvisor Content API integration allows you to discover and inspect destinations, accommodations, and dining experiences with real-time data from millions of users.

### What you can do

- **POI Discovery** — Find any location by name, address, or geographic coordinates
- **Trusted Reviews** — Read the latest user feedback and detailed ratings to make informed travel decisions
- **Visual Content** — Fetch high-quality professional and traveler photos of hotels and attractions
- **Deep Insights** — Access specific metadata like price levels, rankings, and award information
- **Nearby Exploration** — Search for the best restaurants or hotels around a specific GPS coordinate

### How it works

1. Subscribe to this server
2. Enter your **TripAdvisor API Key** (obtained via the TripAdvisor Developer Portal)
3. Start planning and researching travel destinations directly through chat

### Who is this for?

- **Travel Enthusiasts** — research and plan your next trip without leaving your chat
- **Concierge Services** — quickly find and vet recommendations for clients
- **Data Analysts** — explore travel trends and location-based sentiment


## Available Tools (5)
- **get_location_details**: Get comprehensive details for a specific location using its ID
- **get_location_photos**: Retrieve professional and user photos for a specific location
- **get_location_reviews**: Retrieve the latest user reviews for a specific location
- **get_nearby_locations**: Search for locations near a specific geographic coordinate
- **search_location**: Search for hotels, restaurants, and attractions by name or address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TripAdvisor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for top-rated attractions in Paris."

**🤖 AI Agent:**
> I've found several top attractions in Paris, including the Eiffel Tower (Location ID: 188757) and the Louvre Museum (Location ID: 188757). Would you like to see reviews for any of them?

---

**👤 You:**
> "Show me photos and details for location ID 188151."

**🤖 AI Agent:**
> Retrieving data for Location ID 188151... It's the Colosseum in Rome. It has a 4.5 rating with over 150k reviews. Here are some photos of the landmark.


## ❓ FAQ

**Q: How do I get an API Key for TripAdvisor?**
You need to register at the [TripAdvisor Developer Portal](https://www.tripadvisor.com/developers), create a new application, and request an API key.

**Q: Does this tool support booking hotels?**
No, this integration uses the Content API which is focused on information, ratings, and reviews. For booking, you would need to visit the TripAdvisor website directly via the provided links.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tripadvisor](https://vinkius.com/mcp/tripadvisor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TripAdvisor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tripadvisor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TripAdvisor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tripadvisor": {
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
