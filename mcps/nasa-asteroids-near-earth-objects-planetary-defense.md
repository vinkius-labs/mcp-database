# NASA Asteroids — Near-Earth Objects & Planetary Defense MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nasa-asteroids-near-earth-objects-planetary-defense)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nasa-asteroids-near-earth-objects-planetary-defense-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nasa-asteroids-near-earth-objects-planetary-defense-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Track near-Earth asteroids and space rocks in real-time: browse the NeoWs asteroid database, monitor upcoming close approaches from JPL CNEOS, look up specific asteroids by ID, and review atmospheric fireball events detected by government sensors worldwide.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NASA Asteroids — Near-Earth Objects & Planetary Defense** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What asteroids are passing near Earth this week?"

**🤖 AI Agent:**
> ☄️ **Near-Earth Objects This Week**

| Asteroid | Size (m) | Distance (km) | Speed (km/s) | Hazardous |
|----------|----------|---------------|-------------|----------|
| 2024 AA1 | 45-100 | 4,200,000 | 12.3 | No |
| 2023 BX5 | 150-340 | 1,800,000 | 18.7 | ⚠️ Yes |
| 2024 CD2 | 22-50 | 6,500,000 | 8.1 | No |

14 NEOs this week, 1 potentially hazardous.

---

**👤 You:**
> "Are there any large asteroids approaching Earth next month?"

**🤖 AI Agent:**
> Next month, the most significant close approach is by asteroid 2001 FO32, which has an estimated diameter of 550 meters. It will pass safely at a distance of 5 lunar distances (about 1.25 million miles).

---

**👤 You:**
> "Tell me about the recent fireball detected over the Pacific."

**🤖 AI Agent:**
> A significant fireball was detected by government sensors over the central Pacific Ocean yesterday. The calculated total radiated energy suggests it was a small bolide roughly 2 meters in size that burned up completely in the upper atmosphere.


## Installation & Usage

To install and use the **NASA Asteroids — Near-Earth Objects & Planetary Defense** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasa-asteroids-near-earth-objects-planetary-defense](https://vinkius.com/mcp/nasa-asteroids-near-earth-objects-planetary-defense)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
