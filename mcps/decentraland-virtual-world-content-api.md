# Decentraland (Virtual World Content API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/decentraland-virtual-world-content-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Explore Decentraland's virtual world—track hot scenes, list events, analyze parcel stats, and browse the marketplace directly through AI.

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


## Available Tools (15)
- **get_hot_scenes**: Real-time tracking of popular scenes
- **get_main_realm_about**: Get detailed configuration for the optimal main realm
- **get_marketplace_catalog**: Browse and filter wearables/emotes in the marketplace
- **get_marketplace_items**: Query specific NFT items and their trading history
- **get_parcel_stats**: Get user counts per parcel
- **list_places**: List scenes with filters (popularity, coordinates, search)
- **get_realms**: List all healthy catalyst realms with user counts
- **update_place_rating**: Requires authentication.

Update content rating for a place (Admin/Moderator only)
- **list_attending_events**: Requires authentication.

List events the authenticated user is attending
- **get_catalyst_about**: Retrieve health and configuration of all catalyst services
- **create_auth_request**: Create an authentication request
- **create_event**: Requires authentication.

Create a new event
- **list_destinations**: Unified list of Genesis City places and Worlds
- **list_events**: List active/upcoming events
- **get_auth_request**: Get status of an authentication request


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Decentraland (Virtual World Content API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the top 5 hot scenes in Decentraland right now."

**🤖 AI Agent:**
> I've found the most active spots! Currently, 'Genesis Plaza' has 120 users, followed by 'WonderMine' with 85, and 'Dragon City' with 60. Would you like the coordinates for any of these?

---

**👤 You:**
> "List all upcoming events for this weekend."

**🤖 AI Agent:**
> There are several exciting events scheduled! I see a 'Metaverse Music Festival' starting Saturday at 2 PM UTC and a 'Community Town Hall' on Sunday. I can provide the full list of 12 events if you'd like.

---

**👤 You:**
> "Search for scenes related to 'art galleries' near coordinates 0,0."

**🤖 AI Agent:**
> Searching near the center... I found 'Sotheby's Gallery' at (1,1) and 'MUSE Art Space' at (-2,3). Both are highly rated and currently active.


## ❓ FAQ

**Q: How can I find the most crowded places in Decentraland right now?**
You can use the `get_hot_scenes` tool to get a real-time list of popular scenes with active user counts, or `get_parcel_stats` for a granular view of user distribution across coordinates.

**Q: Can I see what events are happening today?**
Yes! The `list_events` tool retrieves all active and upcoming community-organized events, including their descriptions and locations.

**Q: Is it possible to search for specific scenes by name or coordinates?**
Absolutely. Use the `list_places` tool with the `search` parameter for names or the `coordinates` parameter (e.g., "-23,-96") to find content in specific areas.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/decentraland-virtual-world-content-api](https://vinkius.com/mcp/decentraland-virtual-world-content-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Decentraland (Virtual World Content API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `decentraland-virtual-world-content-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Decentraland (Virtual World Content API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "decentraland-virtual-world-content-api": {
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
