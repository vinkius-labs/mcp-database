# TheFork MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thefork)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel-hospitality](../categories/travel-hospitality.md)

Discover, book, and manage restaurant reservations across Europe — search by location, cuisine, and availability through natural AI conversation.

## Description
Transform your AI agent into a personal concierge for dining with **TheFork** — Europe's leading restaurant reservation platform.

### What you can do

- **Restaurant Search** — Find restaurants by location, cuisine type, or keyword with comprehensive rating data
- **Availability Check** — Query real-time table availability for specific dates and party sizes
- **Reviews & Ratings** — Access authentic guest reviews to make informed dining decisions
- **Menu Discovery** — Browse restaurant menus and special offers before booking
- **Reservation Management** — Book tables, check reservation status, and cancel bookings directly
- **Location & Cuisine Browsing** — Explore dining destinations and cuisine categories across the network

### How it works

1. Subscribe to this server
2. Enter your TheFork Partner API key
3. Start discovering and booking restaurants from Claude, Cursor, or any MCP-compatible client

No more switching between apps to find the perfect restaurant. Your AI handles the entire dining workflow — from discovery to booking.

### Who is this for?

- **Foodies & Travelers** — find top-rated restaurants in any European city without endless browsing
- **Executive Assistants** — book restaurants for business dinners and client meetings effortlessly
- **Event Planners** — check availability across multiple venues for group reservations


## Available Tools
- **cancel_reservation**: This action is irreversible.

Cancel a reservation
- **check_availability**: Check restaurant availability
- **create_reservation**: Create a restaurant reservation
- **get_reservation**: Get reservation details
- **get_restaurant**: Get restaurant details
- **get_restaurant_menus**: Get restaurant menus
- **get_restaurant_reviews**: Get restaurant reviews
- **list_cuisines**: List available cuisine types
- **search_locations**: Search for dining locations
- **search_restaurants**: Returns a list of matching restaurants with ratings and availability.

Search for restaurants


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TheFork** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find Italian restaurants near the Eiffel Tower with availability for 4 people tonight."

**🤖 AI Agent:**
> I found 3 Italian restaurants near the Eiffel Tower with tables available tonight! 'Ristorante Tosca' (9.2 rating) has a 20:00 slot, 'Il Carpaccio' (8.8 rating) has 19:30 and 21:00 available. Want me to book one?

---

**👤 You:**
> "Show me the reviews for restaurant ID 45892."

**🤖 AI Agent:**
> Here are the latest reviews for this restaurant. Average rating: 8.7/10. Most guests praise the 'exceptional pasta dishes and attentive service'. Recent concern: 'wait times on weekends can exceed 20 minutes'. Would you like to check availability?


## ❓ FAQ

**Q: Can I book a table at a specific restaurant for tonight?**
Yes! Use the `check_availability` tool to verify open time slots, then `create_reservation` to book directly. You can specify the date, time, party size, and any special requests.

**Q: What information do I get when searching for restaurants?**
Search results include restaurant names, ratings, cuisine types, locations, and real-time availability. You can then drill into any listing for full menus, reviews, and booking options.

**Q: Can I cancel a reservation through the AI agent?**
Yes. The `cancel_reservation` tool lets you cancel any existing booking by providing the reservation ID. Note that cancellation policies vary by restaurant.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thefork](https://vinkius.com/mcp/thefork)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TheFork** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `thefork` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TheFork** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thefork": {
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
