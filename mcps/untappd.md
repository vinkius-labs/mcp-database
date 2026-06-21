# Untappd MCP Server

Track beers, breweries, and venues. Access check-in feeds, beer metadata, and manage your social drinking profile directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/untappd)

## Overview
**Category:** gaming-entertainment
**Tools Count:** 30

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


## Available Tools
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


## Installation & Usage

To install and use the **Untappd** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/untappd](https://vinkius.com/mcp/untappd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
