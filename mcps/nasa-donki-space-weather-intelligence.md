# NASA DONKI — Space Weather Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nasa-donki-space-weather-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nasa-donki-space-weather-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nasa-donki-space-weather-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

NASA's Space Weather Database: coronal mass ejections (CMEs), solar flares (C/M/X class), geomagnetic storms, interplanetary shocks, solar energetic particles, radiation belt events, and real-time notifications from the DONKI system.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NASA DONKI — Space Weather Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Were there any solar flares this month?"

**🤖 AI Agent:**
> ☀️ **Solar Flares — April 2026**

| Date | Class | Peak | Region |
|------|-------|------|--------|
| Apr 2 | M2.1 | 14:32 UT | AR 3842 |
| Apr 3 | C7.4 | 08:15 UT | AR 3840 |
| Apr 3 | X1.2 | 22:47 UT | AR 3842 |

3 flares this month. 1 X-class — may cause HF radio blackouts.

---

**👤 You:**
> "Were there any major geomagnetic storms last year?"

**🤖 AI Agent:**
> Yes, there were 12 significant geomagnetic storms last year reaching Kp index 6 or higher. The most severe was a G4-class storm in May, which caused auroras to be visible as far south as Texas.

---

**👤 You:**
> "Check if any interplanetary shocks are approaching."

**🤖 AI Agent:**
> Based on DONKI data, there is 1 interplanetary shock approaching. It is linked to a CME that erupted two days ago and is expected to pass by the DSCOVR satellite within the next 8-12 hours.


## Installation & Usage

To install and use the **NASA DONKI — Space Weather Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasa-donki-space-weather-intelligence](https://vinkius.com/mcp/nasa-donki-space-weather-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
