# LocationIQ MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/locationiq)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/locationiq-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/locationiq-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [geocoding-maps](../categories/geocoding-maps.md)

Convert addresses to coordinates, find places nearby, and calculate routes with LocationIQ's geocoding and mapping tools.

## Description
Connect **LocationIQ** to your AI agent to access powerful location-based services. This server enables forward and reverse geocoding, point-of-interest search, and routing capabilities directly within your conversation.

### What you can do

- **Forward Geocoding** — Convert any address or place name into precise latitude and longitude coordinates using the `search` tool.
- **Reverse Geocoding** — Identify the human-readable address for any specific set of coordinates with the `reverse` tool.
- **Autocomplete** — Get real-time suggestions for addresses as you type using the `autocomplete` tool.
- **Nearby Search** — Find points of interest like cafes, gas stations, or parks around a specific location with the `nearby` tool.
- **Routing & Directions** — Calculate the best path between multiple coordinates with distance and duration metrics using the `directions` tool.
- **Static Maps** — Generate map image URLs to visualize locations instantly with the `static_map` tool.
- **Timezone Data** — Retrieve local time and timezone offsets for any point on Earth using the `timezone` tool.

### How it works

1. Subscribe to this server
2. Enter your LocationIQ API Key
3. Start querying locations and routes from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Fleet Managers** — Calculate routes and verify delivery addresses directly from your agent.
- **Travel & Hospitality** — Find nearby attractions and local timezones for travel planning.
- **Developers** — Quickly test geocoding results and generate map previews without leaving the IDE.


## Available Tools
- **autocomplete**: Autocomplete API
- **directions**: Directions API
- **nearby**: ) around a given coordinate.

Nearby POI (Points of Interest)
- **reverse**: Reverse Geocoding
- **search**: Search / Forward Geocoding
- **static_map**: Static Maps
- **timezone**: Timezone API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LocationIQ** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the coordinates for '1600 Pennsylvania Avenue NW, Washington, DC'."

**🤖 AI Agent:**
> I've found the location using the `search` tool. The coordinates for the White House are Latitude 38.8977 and Longitude -77.0365.

---

**👤 You:**
> "What is the current local time at coordinates 48.8566, 2.3522?"

**🤖 AI Agent:**
> Using the `timezone` tool for those coordinates (Paris, France), the current local time is 2:45 PM (CET) with a UTC offset of +1.

---

**👤 You:**
> "Show me a map of the Eiffel Tower at zoom level 15."

**🤖 AI Agent:**
> I've generated a static map URL for you using the `static_map` tool, centered on the Eiffel Tower (48.8584, 2.2945) at zoom level 15.


## Installation & Usage

To install and use the **LocationIQ** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/locationiq](https://vinkius.com/mcp/locationiq)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
