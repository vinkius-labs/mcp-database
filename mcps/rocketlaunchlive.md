# RocketLaunch.Live MCP Server

Track rocket launches worldwide — search upcoming launches, vehicles, companies, locations and missions.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/rocketlaunchlive)

## Overview
**Category:** data-management
**Tools Count:** 9

## Description
Connect to **RocketLaunch.Live** and explore the world's curated rocket launch database through natural conversation — no API key needed for basic access.

### What you can do

- **Upcoming Launches** — Get the next upcoming rocket launches with vehicle, provider and mission details
- **Launch Search** — Search launches by date range, location, provider, vehicle or free-text query
- **Launch Details** — Get complete info on a specific launch including webcast links and status
- **Companies** — Browse launch providers and manufacturers (SpaceX, NASA, Roscosmos, etc.)
- **Locations** — Explore launch sites and facilities worldwide
- **Launch Pads** — Find specific launch pads (LC-39A, SLC-40, etc.)
- **Vehicles** — Search rockets and launch vehicles (Falcon 9, Starship, SLS, etc.)
- **Missions** — Browse missions and payloads (Starlink, Artemis, CRS, etc.)
- **Tags** — Filter launches by category (crew, satellite, ISS, etc.)

### How it works

1. Subscribe to this server
2. No API key needed for basic access (5 upcoming launches)
3. Start tracking rocket launches from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Space Enthusiasts** — track upcoming launches, explore vehicles and follow space missions
- **Educators** — demonstrate real-world rocket launches, providers and space industry to students
- **Researchers** — analyze launch frequency, provider market share and launch site utilization


## Available Tools
- **get_tags**: Returns tag text and IDs for filtering launches.

Search launch tags
- **get_vehicles**: Returns vehicle names, descriptions, families and manufacturers.

Search launch vehicles (rockets)
- **get_companies**: Returns company names, countries, logos and active status. Filter by name or country code.

Search launch providers and manufacturers
- **get_launch**: Returns vehicle, provider, location, pad, mission, launch time, status and webcast links.

Get a specific launch by ID
- **get_locations**: Returns location names, country codes and associated launch pads.

Search launch locations
- **get_missions**: Returns mission names, descriptions and objectives.

Search launch missions
- **get_next_launches**: Free tier supports up to 5 launches without API key. Premium key unlocks full access.

Get the next upcoming rocket launches
- **get_pads**: Returns pad names, locations, maps and associated launch facilities.

Search launch pads
- **search_launches**: Live database for rocket launches. Supports free-text search, date range filtering, and filtering by location, provider, vehicle and tag. Returns launches with vehicle info, provider, launch site, mission details and status.

Search rocket launches


## Installation & Usage

To install and use the **RocketLaunch.Live** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rocketlaunchlive](https://vinkius.com/mcp/rocketlaunchlive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
