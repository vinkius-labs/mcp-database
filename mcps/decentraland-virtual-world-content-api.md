# Decentraland (Virtual World Content API) MCP Server

Explore Decentraland's virtual world—track hot scenes, list events, analyze parcel stats, and browse the marketplace directly through AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/decentraland-virtual-world-content-api)

## Overview
**Category:** data-analytics
**Tools Count:** 15

## Description
Connect to the **Decentraland** ecosystem and interact with the metaverse's content layer through natural conversation. This server provides deep access to real-time world data, community activities, and marketplace listings.

### What you can do

- **Real-time Discovery** — Use `get_hot_scenes` and `list_places` to find where the community is gathering right now based on live user counts.
- **Event Management** — Query upcoming community gatherings with `list_events` or check your personal schedule with `list_attending_events`.
- **World Analytics** — Monitor the health of the metaverse infrastructure via `get_catalyst_about` and track user distribution across the map with `get_parcel_stats`.
- **Marketplace Access** — Browse the virtual economy by fetching the latest items and catalog listings from the Decentraland Marketplace.
- **Content Moderation** — Authorized users can update place ratings to ensure a safe environment for all explorers.

### How it works

1. Subscribe to this server
2. Enter your Decentraland Bearer Token (if required for authenticated actions)
3. Start exploring the metaverse from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Metaverse Explorers** — Find the best parties, galleries, and games without manually searching through external maps.
- **Content Creators & Land Owners** — Monitor traffic to your parcels and keep track of competing hot scenes in real-time.
- **Data Analysts** — Gather statistics on user distribution and realm health for research or reporting.


## Available Tools
- **list_attending_events**: Requires authentication.

List events the authenticated user is attending
- **get_catalyst_about**: Retrieve health and configuration of all catalyst services
- **create_auth_request**: Create an authentication request
- **create_event**: Requires authentication.

Create a new event
- **list_destinations**: Unified list of Genesis City places and Worlds
- **list_events**: List active/upcoming events
- **get_auth_request**: Get status of an authentication request
- **get_hot_scenes**: Real-time tracking of popular scenes
- **get_main_realm_about**: Get detailed configuration for the optimal main realm
- **get_marketplace_catalog**: Browse and filter wearables/emotes in the marketplace
- **get_marketplace_items**: Query specific NFT items and their trading history
- **get_parcel_stats**: Get user counts per parcel
- **list_places**: List scenes with filters (popularity, coordinates, search)
- **get_realms**: List all healthy catalyst realms with user counts
- **update_place_rating**: Requires authentication.

Update content rating for a place (Admin/Moderator only)


## Installation & Usage

To install and use the **Decentraland (Virtual World Content API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/decentraland-virtual-world-content-api](https://vinkius.com/mcp/decentraland-virtual-world-content-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
