# EPA AirNow MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/epa-airnow)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/epa-airnow-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/epa-airnow-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Monitor localized air quality indices and critical environmental forecasts directly from the Environmental Protection Agency.

## Description
The **EPA AirNow MCP Server** connects your AI agent to the beating heart of environmental tracking. Gather deep insights into regional air safety, allowing proactive mitigation of respiratory risks and wildfire smoke exposure.

### Core Capabilities

- **Real-Time AQI Observations** — Instantly check current pollutant levels (Ozone, PM2.5, PM10) to determine if the local air is safe to breathe today.
- **Regional Forecasts** — Look ahead to anticipate upcoming hazardous environmental conditions, enabling dynamic safety planning for events or communities.
- **Flexible Targeting** — Pinpoint any community instantly using standard postal codes or exact geographic coordinates to get a tight observation radius.

Ideal for health-conscious applications, community dashboards, outdoor adventure planners, and risk assessment workflows tailored to individuals with sensitivities like asthma.


## Available Tools
- **get_current_aqi_by_latlon**: Get real-time Air Quality Index observation using geographic coordinates
- **get_current_aqi_by_zip**: Requires a 5-digit US ZIP Code.

Get current real-time Air Quality Index observation using a US ZIP code
- **get_forecast_aqi_by_zip**: Get future AQI forecasts for a given US ZIP code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EPA AirNow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current air quality index in Beverly Hills?"

**🤖 AI Agent:**
> I've checked the latest observations for Beverly Hills. The current AQI is 45 (Good). It's a great day for outdoor activities without any health risks.

---

**👤 You:**
> "Will the air quality be safe for a marathon in Seattle tomorrow?"

**🤖 AI Agent:**
> Let me check the AirNow forecast for Seattle tomorrow. The AQI is predicted to peak at around 55 (Moderate), largely due to PM2.5. It remains generally safe for the marathon, though unusually sensitive athletes should monitor how they feel.

---

**👤 You:**
> "Fetch the PM10 specific metrics for ZIP code 90210 safely via AirNow."

**🤖 AI Agent:**
> Retrieving specific pollutant values securely...
**Area: Beverly Hills (90210)**
- PM10 concentration reported optimally clear (AQI 22). Parameter checked actively and correctly without errors.


## Installation & Usage

To install and use the **EPA AirNow** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epa-airnow](https://vinkius.com/mcp/epa-airnow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
