# Guidebook MCP Server

Automate mobile app content management via Guidebook — manage guides, sessions, speakers, and custom lists directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/guidebook)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Guidebook Builder** account to any AI agent and manage your mobile event or organization app content through natural conversation.

### What you can do

- **Guide Oversight** — List all mobile guides in your account and retrieve detailed metadata for each.
- **Schedule Management** — Browse, list, and inspect schedule sessions to keep your event timeline up to date.
- **Speaker Coordination** — Access speaker profiles and presenter details to ensure all bio information is accurate.
- **Custom Lists** — Manage Exhibitors, Sponsors, or any other custom data lists within your app.
- **Venue & Locations** — Retrieve all defined locations and map data for your event.
- **Rate Limit Tracking** — Monitor your API usage to stay within your daily quota.

### How it works

1. Subscribe to this server
2. Enter your Guidebook API Key (JWT token)
3. Start managing your app content from Claude, Cursor, or any MCP-compatible client

No more manual data entry in the Builder interface. Your AI assistant acts as a dedicated content coordinator for your mobile apps.

### Who is this for?

- **Event Organizers** — quickly verify session times and speaker assignments without digging through the CMS.
- **Content Managers** — automate the retrieval and auditing of custom lists like exhibitors or sponsors.
- **App Developers** — integrate Guidebook content flows into your development environment seamlessly.


## Available Tools
- **get_guide**: Get detailed information about a specific guide
- **get_rate_limit**: Check current API usage and rate limits
- **get_session**: Get details for a specific schedule session
- **get_speaker**: Get details for a specific speaker profile
- **list_custom_lists**: List custom list items (e.g., Exhibitors, Sponsors) for a guide
- **list_guides**: List all guides available in the account
- **list_locations**: List all locations/venues defined for a guide
- **list_schedules**: List schedules for a specific guide
- **list_sessions**: List all schedule sessions for a specific guide
- **list_speakers**: List all speakers/presenters for a specific guide


## Installation & Usage

To install and use the **Guidebook** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/guidebook](https://vinkius.com/mcp/guidebook)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
