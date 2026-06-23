# Untappd MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/untappd)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming-entertainment](../categories/gaming-entertainment.md)

Track beers, breweries, and venues. Access check-in feeds, beer metadata, and manage your social drinking profile directly from your AI agent.

## Description
Connect your **Untappd** account to any AI agent to explore the world of craft beer through natural conversation. This MCP server provides comprehensive access to the Untappd social network for beer enthusiasts.

### What you can do

- **Activity Feeds** — Monitor friend check-ins, user activity, or specific feeds for beers, breweries, and venues.
- **Beer & Brewery Intelligence** — Fetch detailed metadata, ratings, and descriptions for millions of beers and breweries using unique IDs.
- **Social Interaction** — Add check-ins, post comments, toggle toasts, and manage friend requests directly from your agent.
- **Discovery & Search** — Search for new beers or breweries and stay updated with trending beers in the community.
- **Personal Management** — Access your user profile, badges, wishlist, and distinct beer history to track your tasting journey.

### How it works

1. Subscribe to this server
2. Enter your Untappd Access Token
3. Start exploring beers and managing your check-ins from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Beer Enthusiasts** — quickly check beer ratings and details while at a bar or brewery without opening the app
- **Social Drinkers** — keep up with friends' activities and interact with their check-ins via simple commands
- **Data Analysts** — gather brewery and beer metadata for personal research or trend tracking


## Available Tools (30)
- **accept_friend**: Accept a friend request
- **add_checkin**: Check-in to a beer
- **add_comment**: Add a comment to a checkin
- **add_to_wishlist**: Add a beer to the authenticated user's wish list
- **get_beer_activity**: Activity feed for a single beer
- **get_beer_info**: Get detailed information about a beer
- **get_brewery_activity**: Activity feed for a single brewery
- **get_brewery_info**: Get detailed information about a brewery
- **get_checkin_details**: Extended details for a checkin including location, comments, and toasts
- **foursquare_lookup**: Translate a Foursquare v2 ID into an Untappd Venue ID
- **get_friend_activity**: Requires authentication.

Obtain the friend check-in feed of the authenticated user
- **get_notifications**: Get feed of toasts, comments, and news for the authenticated user
- **get_pending_friends**: Get pending friend requests
- **reject_friend**: Reject a friend request
- **remove_comment**: Remove a comment from a checkin
- **remove_friend**: Remove a friend
- **remove_from_wishlist**: Remove a beer from the authenticated user's wish list
- **request_friend**: Send a friend request
- **search_beer**: Search for beers
- **search_brewery**: Search for breweries
- **toggle_toast**: Toast or Untoast a checkin
- **get_trending_beers**: Returns macro and micro trending beers globally
- **get_user_activity**: If username is omitted, returns authenticated user feed.

Obtain the check-in feed of a selected user
- **get_user_badges**: Get a list of badges for a user
- **get_user_distinct_beers**: Get a list of distinct beers a user has had
- **get_user_friends**: Get a list of friends for a user
- **get_user_info**: Get user profile information
- **get_user_wishlist**: Get a user's wish list
- **get_venue_activity**: Activity feed for a single venue
- **get_venue_info**: Get detailed information about a venue


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Untappd** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the latest beer check-ins from my friends."

**🤖 AI Agent:**
> I've retrieved your friend feed. Your friend 'JohnD' just checked into a 'Punk IPA' by BrewDog at 'The Craft Bar' with a 4.25 rating. 'SarahB' is having a 'Guinness Draught' at home.

---

**👤 You:**
> "What are the details for beer ID 4481?"

**🤖 AI Agent:**
> Beer ID 4481 is 'Anchor Steam Beer' by Anchor Brewing Company. It's a California Common style with 4.9% ABV and 33 IBU. It has a global rating of 3.51 based on over 300,000 check-ins.

---

**👤 You:**
> "Search for a brewery named 'Stone Brewing'."

**🤖 AI Agent:**
> I found 'Stone Brewing' (ID: 1204) located in Escondido, CA. They have over 500 beers listed and a brewery rating of 4.02. Would you like to see their most popular beers?


## ❓ FAQ

**Q: How can I see what my friends have been drinking recently?**
You can use the `get_friend_activity` tool. It fetches the latest check-in feed from your Untappd friends, including beer names, ratings, and locations.

**Q: Can I get detailed information about a specific beer if I have its ID?**
Yes! Use the `get_beer_info` tool with the Beer ID (bid). It will return comprehensive metadata, including ABV, IBU, brewery details, and global ratings.

**Q: Is it possible to add a new beer check-in through the AI agent?**
Absolutely. The `add_checkin` tool allows you to post a new check-in by providing the Beer ID, and optionally a rating, comments, and location.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/untappd](https://vinkius.com/mcp/untappd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Untappd** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `untappd` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Untappd** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "untappd": {
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
