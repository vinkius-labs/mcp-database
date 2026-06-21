# Taiwan Weather (CWA) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/taiwan-weather-cwa)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/taiwan-weather-cwa-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/taiwan-weather-cwa-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Access official weather forecasts, typhoon tracking, and real-time earthquake reports for Taiwan from the Central Weather Administration.

## Description
The **Taiwan Weather MCP Server** integrates your AI agent with the official Central Weather Administration (CWA) of Taiwan — one of the most advanced meteorological services in the Pacific Rim.

### Core Capabilities

- **36-Hour General Forecast** — Detailed weather predictions for every city and county in Taiwan, including temperature ranges, precipitation probability, and weather conditions.
- **1-Week Township Forecast** — Extended forecasts with 12-hour granularity across all townships, ideal for travel planning and logistics.
- **Earthquake Reports** — Official seismic event data from Taiwan's dense monitoring network. As a key location on the Pacific Ring of Fire, Taiwan experiences frequent seismic activity, making this data critical for safety applications.
- **Small-Magnitude Events** — Comprehensive minor earthquake tracking for research and seismological analysis.

Free API key required (instant registration). Taiwan's CWA maintains one of the densest meteorological sensor networks in Asia, delivering high-precision data essential for anyone operating in the Western Pacific typhoon corridor.


## Available Tools
- **get_taiwan_earthquakes**: Taiwan sits on the Pacific Ring of Fire and experiences frequent seismic activity. Reports include magnitude, depth, epicenter coordinates, and official assessment.

Get significant earthquake reports for Taiwan and the surrounding Pacific region
- **get_taiwan_forecast**: Returns weather conditions, temperature ranges, and probability of rain for all major cities. You can optionally filter by city name using Traditional Chinese characters or English romanization.

Get the 36-hour weather forecast for cities and counties across Taiwan
- **get_taiwan_weekly_forecast**: Use for longer-range travel and event planning in Taiwan.

Get the 1-week weather forecast for townships across Taiwan with 12-hour intervals
- **get_taiwan_small_earthquakes**: 5) that may not trigger major alerts but are relevant for seismological monitoring and research.

Get small-magnitude earthquake reports for Taiwan from CWA


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Taiwan Weather (CWA)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the weather forecast for Taipei this week?"

**🤖 AI Agent:**
> I've pulled the CWA forecast for Taipei. Expect partly cloudy skies with afternoon thunderstorms through Wednesday, temperatures ranging from 24°C to 31°C. Rain probability peaks at 60% on Tuesday afternoon. Clear conditions expected by the weekend.

---

**👤 You:**
> "Have there been any significant earthquakes near Taiwan recently?"

**🤖 AI Agent:**
> I've checked the CWA seismological feed. The most recent significant earthquake was a magnitude 5.2 event centered 23 km east of Hualien at a depth of 15 km. Minor shaking was felt across eastern Taiwan. No tsunami warning was issued. The CWA registered 3 additional minor events in the surrounding area over the past 48 hours.


## Installation & Usage

To install and use the **Taiwan Weather (CWA)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/taiwan-weather-cwa](https://vinkius.com/mcp/taiwan-weather-cwa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
