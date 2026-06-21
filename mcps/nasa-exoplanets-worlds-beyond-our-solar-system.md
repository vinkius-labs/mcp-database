# NASA Exoplanets — Worlds Beyond Our Solar System MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nasa-exoplanets-worlds-beyond-our-solar-system)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nasa-exoplanets-worlds-beyond-our-solar-system-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nasa-exoplanets-worlds-beyond-our-solar-system-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Explore 5,700+ confirmed exoplanets from NASA's Exoplanet Archive: search by discovery method, find habitable zone candidates, browse transit planets from Kepler and TESS missions, and analyze global discovery statistics spanning three decades of planet hunting.

## Description
Direct SQL-like access to NASA's Exoplanet Archive — the world's most comprehensive database of confirmed planets beyond our solar system.

### What you can do
- **Search Planets** — By name, method, facility, year
- **Transit Planets** — Kepler and TESS discoveries
- **Habitable Zone** — Rocky planets where water could exist
- **Statistics** — Totals, methods, trends

### No API Key Required
The Exoplanet Archive TAP service is completely open.


## Available Tools
- **query_confirmed_planets**: Filter by planet name, discovery method (Transit, Radial Velocity, Imaging, Microlensing), discovery facility (Kepler, TESS, Keck), or year. Returns orbital period, radius, mass, equilibrium temperature.

Search confirmed exoplanets by name, discovery method, facility, or year
- **get_transit_planets**: Transit is the most productive method (>75% of all discoveries). Kepler and TESS are the primary transit missions.

Get exoplanets discovered via the transit method (Kepler/TESS)
- **get_habitable_zone**: These are the most promising candidates for life.

Get exoplanets in the habitable zone — where liquid water could exist
- **get_planet_stats**: Shows how exoplanet science has exploded since Kepler's launch in 2009.

Get global exoplanet discovery statistics: totals, methods, yearly trends


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NASA Exoplanets — Worlds Beyond Our Solar System** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many exoplanets have been discovered?"

**🤖 AI Agent:**
> 🪐 **Exoplanet Discovery Stats**

Total confirmed: **5,748** planets

By method:
- Transit: 4,234 (73.7%)
- Radial Velocity: 1,081 (18.8%)
- Imaging: 72 (1.3%)
- Microlensing: 214 (3.7%)

Peak year: 2016 (1,518 planets — Kepler batch)
Active missions: TESS, JWST

---

**👤 You:**
> "Show me planets in the habitable zone"

**🤖 AI Agent:**
> 🌍 **Habitable Zone Candidates**

| Planet | Radius (R⊕) | Temp (K) | Method | Year |
|--------|------------|----------|--------|------|
| TRAPPIST-1 e | 0.92 | 251 | Transit | 2017 |
| TRAPPIST-1 f | 1.05 | 219 | Transit | 2017 |
| Kepler-442 b | 1.34 | 233 | Transit | 2015 |
| TOI-700 d | 1.19 | 268 | Transit | 2020 |

Rocky planets (< 2 R⊕) with 200-320K equilibrium temperature.


## Installation & Usage

To install and use the **NASA Exoplanets — Worlds Beyond Our Solar System** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasa-exoplanets-worlds-beyond-our-solar-system](https://vinkius.com/mcp/nasa-exoplanets-worlds-beyond-our-solar-system)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
