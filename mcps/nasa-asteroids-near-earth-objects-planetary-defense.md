# NASA Asteroids — Near-Earth Objects & Planetary Defense MCP Server

Track near-Earth asteroids and space rocks in real-time: browse the NeoWs asteroid database, monitor upcoming close approaches from JPL CNEOS, look up specific asteroids by ID, and review atmospheric fireball events detected by government sensors worldwide.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nasa-asteroids-near-earth-objects-planetary-defense)

## Overview
**Category:** the-unthinkable
**Tools Count:** 5

## Description
Complete asteroid intelligence from NASA's NeoWs API and JPL's Center for Near Earth Object Studies (CNEOS).

### What you can do
- **NEO Feed** — Asteroids making close approaches this week
- **Asteroid Details** — Size, orbit, velocity, hazard assessment
- **Close Approaches** — Future Earth encounters from CNEOS
- **Fireballs** — Atmospheric impacts detected by sensors
- **Browse Catalog** — Paginated access to all known NEOs


## Available Tools
- **get_neo_feed**: Includes estimated diameter, velocity, miss distance, and whether potentially hazardous. Source: NASA NeoWs.

Get near-Earth asteroids approaching within a date range
- **get_neo_lookup**: Use SPK-IDs from the feed endpoint.

Get detailed information about a specific asteroid by its NASA SPK-ID
- **get_neo_browse**: Returns 20 asteroids per page. Use for exploring the complete known catalog of near-Earth objects.

Browse the complete catalog of known near-Earth asteroids
- **get_close_approaches**: Filter by distance threshold, date range, and minimum size. Critical for planetary defense monitoring.

Get future close approaches of asteroids to Earth from JPL CNEOS
- **get_fireballs**: Includes location, velocity, energy (kilotons of TNT equivalent), and altitude. Covers events worldwide.

Get atmospheric fireball (bolide) events detected by US government sensors


## Installation & Usage

To install and use the **NASA Asteroids — Near-Earth Objects & Planetary Defense** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasa-asteroids-near-earth-objects-planetary-defense](https://vinkius.com/mcp/nasa-asteroids-near-earth-objects-planetary-defense)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
