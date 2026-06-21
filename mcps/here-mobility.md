# HERE Mobility MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/here-mobility)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/here-mobility-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/here-mobility-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

AI transit planning: discover routes, schedules, and stations for public transport via agents.

## Description
### What you can do

Connect AI agents to the HERE Transit API for comprehensive public transportation planning:

- **Discover transit trips** between any two locations with bus, train, subway, tram, and ferry
- **Find nearby stations** by GPS coordinates or name search
- **Get detailed route information** with step-by-step transit instructions and transfers
- **Check departure/arrival schedules** for any station in real-time
- **Plan multimodal journeys** combining transit, walking, cycling, and scooter
- **Get station details** including accessibility, amenities, and serving lines
- **Search trips with specific transport modes** for customized travel preferences

### How it works

1. **Get your HERE API key** from the HERE Developer Portal (free tier available)
2. **Ask your AI agent** to plan trips, find stations, or check schedules
3. **Natural language commands** replace manual transit app navigation
4. **Real-time transit data** from HERE's global coverage of 70+ countries

### Who is this for?

Essential for **urban commuters**, **travelers**, **tourists**, **accessibility advocates**, **transit enthusiasts**, and **city planners**. Let AI agents find optimal public transit routes, compare multimodal options, check real-time departures, and plan complex journeys across transportation networks. Perfect for anyone in cities with public transit who wants to reduce driving costs, minimize carbon footprint, and navigate efficiently without car ownership.


## Available Tools
- **discover_trips**: Returns trip details including departure/arrival times, duration, number of transfers, and transport modes. Use origin and destination in lat,lng format. Optionally specify departure or arrival time in ISO 8601 format. Best for planning multimodal journeys.

Discover public transit trips between origin and destination using HERE Transit API
- **get_nearby_stations**: More precise than get_stations with customizable radius. Returns station IDs, names, distances, coordinates, and available lines. Use this for comprehensive station discovery in an area.

Find all transit stations within a specific radius of coordinates
- **get_route_details**: Requires the trip ID from a discover_trips result plus original origin/destination and departure time. Use this to review full route before traveling.

Get detailed route information for a specific transit trip
- **get_schedule**: Useful for checking when the next bus, train, or subway arrives. Requires station ID from get_stations result. Optionally filter by direction (e.g., "northbound", "downtown").

Get departure/arrival schedule for a specific transit station
- **get_station_details**: Requires station ID from station search results. Use this to review station facilities before planning trips.

Get detailed information about a specific transit station
- **get_stations_by_name**: g., "Central Station", "Times Square"). Returns matching stations with IDs, names, coordinates, and available transport lines. Use this when you know the station name but not exact coordinates.

Find transit stations by name
- **get_stations**: Returns station IDs, names, coordinates, and available transport lines. Use this to find stations before planning trips.

Find transit stations near a GPS coordinate
- **search_multimodal_trips**: Modes can include: transit (bus/train/subway/tram/ferry), walk, bicycle, scooter, taxi. Returns multimodal route options with time breakdown per mode. Use this when user wants to combine walking or cycling with public transit for optimal journey.

Search trips combining multiple transport modes (transit, walk, bike, scooter)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HERE Mobility** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me the best public transit route from Brandenburg Gate to Berlin Central Station departing at 8am tomorrow"

**🤖 AI Agent:**
> I'll discover the best transit options with departure times, transfers, and walking segments.

---

**👤 You:**
> "What buses and trains depart from Times Square in the next 30 minutes?"

**🤖 AI Agent:**
> I'll check the departure schedule for Times Square station right now.

---

**👤 You:**
> "Plan a multimodal trip from my location combining subway and bike sharing"

**🤖 AI Agent:**
> I'll search for trips combining transit and bicycle modes for an efficient journey.


## Installation & Usage

To install and use the **HERE Mobility** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/here-mobility](https://vinkius.com/mcp/here-mobility)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
