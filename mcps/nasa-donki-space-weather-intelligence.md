# NASA DONKI — Space Weather Intelligence MCP Server

NASA's Space Weather Database: coronal mass ejections (CMEs), solar flares (C/M/X class), geomagnetic storms, interplanetary shocks, solar energetic particles, radiation belt events, and real-time notifications from the DONKI system.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nasa-donki-space-weather-intelligence)

## Overview
**Category:** the-unthinkable
**Tools Count:** 7

## Description
DONKI (Database Of Notifications, Knowledge, Information) is NASA's comprehensive space weather database.

### 7 Event Types
- ☀️ CME — Coronal Mass Ejections
- 🔥 Solar Flares — C, M, X class
- 🧲 Geomagnetic Storms — Kp ≥ 4
- 💥 Interplanetary Shocks
- ⚡ Solar Energetic Particles
- 🛡️ Radiation Belt Events
- 📡 All Notifications (unified feed)


## Available Tools
- **get_cme**: CMEs are massive bursts of solar wind and magnetic fields from the Sun. Earth-directed CMEs cause geomagnetic storms and aurora. Default: last 30 days.

Get Coronal Mass Ejection (CME) events from NASA DONKI
- **get_solar_flares**: Classes: C (common), M (moderate), X (extreme). X-class flares cause radio blackouts and satellite disruption. Includes begin/peak/end times, active region, and instruments that detected it.

Get solar flare events by class (C, M, X) from NASA DONKI
- **get_geomagnetic_storms**: Includes Kp index and linked CME/shock data. Storms above Kp=7 are severe, Kp=9 is extreme. Affects power grids, GPS, satellites, and enables aurora at low latitudes.

Get geomagnetic storm events from NASA DONKI
- **get_interplanetary_shocks**: Shocks often precede geomagnetic storms and are caused by CME-driven disturbances in the solar wind.

Get interplanetary shock wave events from NASA DONKI
- **get_solar_energetic_particles**: SEPs are dangerous to astronauts and can damage satellite electronics.

Get Solar Energetic Particle (SEP) events from NASA DONKI
- **get_radiation_belt**: The Van Allen radiation belts can be energized during geomagnetic storms, posing risks to satellites in medium Earth orbit.

Get radiation belt enhancement events from NASA DONKI
- **get_donki_notifications**: A unified feed of all space weather events: CMEs, flares, storms, shocks, and radiation events. Good for a quick overview of recent solar activity.

Get all recent DONKI space weather notifications


## Installation & Usage

To install and use the **NASA DONKI — Space Weather Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasa-donki-space-weather-intelligence](https://vinkius.com/mcp/nasa-donki-space-weather-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
