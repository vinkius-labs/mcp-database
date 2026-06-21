# NOAA Space Weather — Solar & Geomagnetic Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/noaa-space-weather-solar-geomagnetic-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/noaa-space-weather-solar-geomagnetic-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/noaa-space-weather-solar-geomagnetic-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Real-time space weather intelligence: planetary Kp geomagnetic index, 3-day Kp forecast, solar wind speed and magnetic field, aurora probability forecast (Ovation model), solar flux (F10.7), and Dst storm index from NOAA SWPC.

## Description
Real-time space weather from NOAA's Space Weather Prediction Center.

### What you can do
- **Kp Index** — Current geomagnetic activity (aurora threshold)
- **Kp Forecast** — 3-day predictions
- **Solar Wind** — Speed (km/s) and Bz from DSCOVR satellite
- **Aurora Forecast** — Ovation probability model (global)
- **Solar Flux** — F10.7 solar activity proxy
- **Dst Index** — Ring current storm intensity

### Who Needs This?
Aurora hunters, satellite operators, HF radio operators, power grid managers, airline operators (polar routes), and space enthusiasts.


## Available Tools
- **get_planetary_k_index**: Kp ranges 0-9. Values ≥5 indicate geomagnetic storms with visible aurora at lower latitudes. Updated every 3 hours. Essential for aurora hunters, satellite operators, and power grid managers.

Get the NOAA Planetary K-index — geomagnetic activity and aurora probability
- **get_k_index_forecast**: Use this to plan for aurora viewing, satellite vulnerabilities, or HF radio propagation impacts.

Get the 3-day Kp index forecast — predicted geomagnetic activity
- **get_solar_wind**: The solar wind drives geomagnetic storms — when speed exceeds 500 km/s with southward Bz, aurora probability increases dramatically.

Get real-time solar wind speed and magnetic field conditions
- **get_aurora_forecast**: Powered by real-time solar wind data. The gold standard for aurora forecasting worldwide.

Get the aurora probability forecast map data (Ovation model)
- **get_solar_flux**: 7 solar flux index. Higher values (>100 SFU) indicate increased solar activity, more sunspots, and higher probability of solar flares and CMEs. Normal quiet-sun values are 70-80 SFU.

Get the 10.7cm solar radio flux — a proxy for solar activity level
- **get_dst_index**: Measures the intensity of the ring current around Earth. Values below -50 nT indicate a moderate storm, below -100 nT a strong storm, below -250 nT a severe storm. Critical for satellite operators and power grid monitoring.

Get the Dst index — real-time geomagnetic storm intensity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NOAA Space Weather — Solar & Geomagnetic Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can I see the aurora tonight?"

**🤖 AI Agent:**
> 🌌 **Aurora Probability Tonight**

Current Kp: 4 (Active)
Forecast: Kp 5 (Minor Storm) expected 9pm-midnight
Solar Wind: 520 km/s (elevated)
Bz: -6 nT (southward — favorable!)

✅ Aurora likely visible from:
- Northern US states (WA, MT, MN, WI, MI, NY, ME)
- Southern Canada
- Northern Europe

❌ Not visible from: Southern US, tropics

---

**👤 You:**
> "What is the current solar wind status?"

**🤖 AI Agent:**
> ☀️ **Solar Wind (Real-Time)**

Speed: 485 km/s (moderate)
Bz: -3.2 nT (slightly southward)
Bt: 7.8 nT
Density: 4.2 p/cm³

Solar Flux (F10.7): 148 SFU (above average)
Dst: -28 nT (quiet)

⚡ Conditions: mildly disturbed. HF radio propagation good. No significant storm expected in next 24h.


## Installation & Usage

To install and use the **NOAA Space Weather — Solar & Geomagnetic Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noaa-space-weather-solar-geomagnetic-intelligence](https://vinkius.com/mcp/noaa-space-weather-solar-geomagnetic-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
