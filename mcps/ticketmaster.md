# Ticketmaster MCP Server

Search for live events, venues, and attractions, and manage ticket reservations directly through Ticketmaster's APIs.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ticketmaster)

## Overview
**Category:** ecommerce
**Tools Count:** 22

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


## Available Tools
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


## Installation & Usage

To install and use the **Ticketmaster** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ticketmaster](https://vinkius.com/mcp/ticketmaster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
