# Ticketmaster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ticketmaster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Search for live events, venues, and attractions, and manage ticket reservations directly through Ticketmaster's APIs.

## Description
Connect your AI agent to the **Ticketmaster** ecosystem to discover live entertainment and manage ticketing workflows through natural language.

### What you can do

- **Event Discovery** — Search for concerts, sports, and theater events using keywords, location, dates, and genres via `search_events`.
- **Venue & Attraction Insights** — Find detailed information about stadiums, arenas, and performers using `search_venues` and `search_attractions`.
- **Ticket Management** — Initiate ticket reservations and manage cart details including shipping and billing through the Partner API tools like `reserve_tickets` and `add_shipping`.
- **Smart Suggestions** — Get real-time search suggestions for keywords and entities using the `suggest` tool.
- **Deep Event Details** — Retrieve full metadata, pricing ranges, and seat maps for specific events using `get_event`.

### How it works

1. Subscribe to this server
2. Enter your Ticketmaster Developer Consumer Key (API Key)
3. Start searching for the best live experiences from Claude, Cursor, or any MCP client

### Who is this for?

- **Event Planners** — Quickly find venue availability and event schedules without manual browsing.
- **Travel & Concierge Agents** — Automate the discovery of local entertainment for clients based on their travel dates and cities.
- **Developers** — Integrate live event data and ticketing capabilities into custom workflows or applications.


## Available Tools (22)
- **add_billing**: Add billing to a cart (Partner API)
- **add_shipping**: Add shipping to a cart (Partner API)
- **commit_purchase**: Commit a ticket purchase (Partner API)
- **get_discovery_feed**: Get bulk event data download URIs per country
- **get_event**: Get details for a specific event
- **get_intl_event**: Get international event details (EU)
- **get_intl_similar_attractions**: Find similar attractions in international markets (EU)
- **get_inventory_status**: Get near real-time availability status for primary and resale inventory
- **get_order**: Retrieve detailed order info (Partner API)
- **get_top_picks**: Get seat recommendations based on availability and quality scores
- **get_top_picks_universal**: Get seat recommendations using a Universal Event ID
- **publish_attraction**: Publish a new attraction
- **publish_event**: Publish a new event
- **publish_venue**: Publish a new venue
- **reserve_tickets**: Reserve tickets for an event (Partner API)
- **search_attractions**: Search for artists, sports teams, etc
- **search_classifications**: Search for genres, segments, and sub-genres
- **search_events**: Find events by location, date, keyword, etc
- **search_intl_events**: Search events in international markets (EU)
- **search_venues**: Search for venues
- **suggest**: Find search suggestions
- **update_published_event**: Update an existing published event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ticketmaster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find music events in New York for next month."

**🤖 AI Agent:**
> I've found several music events in New York for next month, including 'Madison Square Garden Concert Series' and 'Brooklyn Steel Indie Night'. Would you like the specific dates for any of these?

---

**👤 You:**
> "Search for venues in Los Angeles with 'Arena' in the name."

**🤖 AI Agent:**
> I found 3 venues in Los Angeles matching 'Arena': Crypto.com Arena, Galen Center Arena, and Kia Forum Arena. Which one would you like to see events for?

---

**👤 You:**
> "Get the details for event ID 'vvG17Z9pG7k6z'."

**🤖 AI Agent:**
> Fetching details for event vvG17Z9pG7k6z... This is 'The Eras Tour' at SoFi Stadium. Tickets range from $99 to $499, and the event starts at 7:00 PM local time.


## ❓ FAQ

**Q: Can I search for events by genre like 'Music' or 'Sports'?**
Yes! Use the `search_events` tool and provide the `classificationName` parameter (e.g., 'music', 'sports', 'arts') to filter results by category.

**Q: How do I get information about a specific stadium or theater?**
You can use the `search_venues` tool with a keyword or location to find the venue's details, including its address and upcoming event capacity.

**Q: Does this server support ticket purchasing?**
The server includes Partner API tools like `reserve_tickets`, `add_shipping`, and `add_billing` to facilitate the reservation and checkout process for authorized partners.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ticketmaster](https://vinkius.com/mcp/ticketmaster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ticketmaster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ticketmaster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ticketmaster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ticketmaster": {
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
