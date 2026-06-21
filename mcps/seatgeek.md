# SeatGeek MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/seatgeek)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [event-management](../categories/event-management.md)

Search and list SeatGeek events, performers, and venues directly from your AI agent.

## Description
Access the vast **SeatGeek** database to discover live events, sports, concerts, and theater performances. This MCP server allows your AI to query real-time event data, performer bios, and venue details.

### What you can do

- **Event Discovery** — Search for events by keyword, date, city, or performer slug using `list_events`.
- **Performer Insights** — Retrieve detailed information about athletes, bands, and performers with `list_performers` and `get_performer`.
- **Venue Information** — List and inspect specific venues to understand where events are happening using `list_venues` and `get_venue`.
- **Category Mapping** — Explore the SeatGeek taxonomy to filter by specific event types with `list_taxonomies`.
- **Detailed Lookups** — Fetch full metadata for specific events using their unique IDs via `get_event`.

### How it works

1. Subscribe to this server
2. Enter your SeatGeek Client ID
3. Start exploring live entertainment from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Planners** — Quickly find venue details and event schedules without manual searching.
- **Data Analysts** — Gather event and performer metadata for market research or trend analysis.
- **Entertainment Enthusiasts** — Use your AI to find the best upcoming shows and sports matches in any city.


## Available Tools
- **list_events**: Search and list SeatGeek events
- **get_event**: Retrieve a specific SeatGeek event
- **get_performer**: Retrieve a specific SeatGeek performer
- **get_venue**: Retrieve a specific SeatGeek venue
- **list_performers**: ).

Search and list SeatGeek performers
- **list_taxonomies**: List SeatGeek event categories (taxonomies)
- **list_venues**: Search and list SeatGeek venues


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SeatGeek** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for upcoming rock concerts in Los Angeles using SeatGeek."

**🤖 AI Agent:**
> I've found several rock concerts in Los Angeles. Notable events include 'The Rolling Stones' at SoFi Stadium and 'Arctic Monkeys' at The Forum. Would you like details for a specific one?

---

**👤 You:**
> "Get the details for the venue with ID 150."

**🤖 AI Agent:**
> Fetching venue details... Venue ID 150 is 'Madison Square Garden' located in New York. It has a capacity of approximately 20,000 and hosts various sports and music events.

---

**👤 You:**
> "List all event taxonomies available on SeatGeek."

**🤖 AI Agent:**
> I've retrieved the taxonomies. Categories include 'sports', 'concert', 'theater', 'ncaa_basketball', 'broadway_tickets_national', and many more. Which category are you interested in?


## ❓ FAQ

**Q: How can I find events happening in a specific city?**
You can use the `list_events` tool and provide the city name in the `venue_city` parameter. For example, searching for 'New York' will return all upcoming events in that location.

**Q: Can I get detailed information about a specific music band or athlete?**
Yes! Use the `list_performers` tool to search for them by name, and then use `get_performer` with their specific ID to retrieve full metadata and bios.

**Q: How do I see what types of event categories SeatGeek supports?**
Simply run the `list_taxonomies` tool. It will return a comprehensive list of all event categories (like sports, concerts, or theater) used by the platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/seatgeek](https://vinkius.com/mcp/seatgeek)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SeatGeek** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `seatgeek` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SeatGeek** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "seatgeek": {
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
