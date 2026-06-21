# NOAA Tides & Currents API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/noaa-tides-currents-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/noaa-tides-currents-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/noaa-tides-currents-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Monitor tidal data — audit water levels and predictions via AI.

## Description
Empower your AI agent to orchestrate your entire maritime research and tidal auditing workflow with the **NOAA Tides & Currents API**, the authoritative source for United States coastal data. By connecting NOAA's Center for Operational Oceanographic Products and Services (CO-OPS) to your agent, you transform complex water level searches into a natural conversation. Your agent can instantly retrieve real-time water levels, audit high and low tide predictions, and query atmospheric metadata without you ever touching a technical portal. Whether you are planning maritime logistics or conducting coastal research, your agent acts as a real-time oceanographic consultant, ensuring your data is always verified and precise.

### What you can do

- **Water Level Auditing** — Retrieve real-time water level data for thousands of NOAA stations and maintain a clear view of coastal changes.
- **Tide Oversight** — Audit high and low tide predictions to understand the temporal distribution of maritime scale instantly.
- **Atmospheric Discovery** — Query real-time air and water temperature metadata to assist in regional environmental planning.
- **Station Intelligence** — Retrieve high-resolution details for specific NOAA station IDs to assist in deep-dive oceanographic classification.
- **Maritime Monitoring** — Check API status to ensure your maritime research workflow is always operational.

### How it works

1. Subscribe to this server
2. No API Key required (NOAA CO-OPS is a free and open service)
3. Start managing your maritime intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Mariners & Harbor Masters** — monitor water levels and retrieve tidal metadata straight from your workflow.
- **Coastal Researchers** — verify tide patterns and audit environmental markers without manual searching.
- **Logistics Planners** — perform rapid audits of port conditions and identify relevant maritime markers through natural language.
- **Operations Leads** — automate oceanographic data querying to orchestrate cross-functional maritime teams smoothly.


## Available Tools
- **check_api_status**: Check if the NOAA Tides & Currents service is operational
- **get_air_temperature**: Get real-time air temperature data for a specific NOAA station
- **get_tide_predictions**: Get high and low tide predictions for a specific NOAA station
- **get_water_levels**: Get real-time water levels for a specific NOAA station
- **get_water_temperature**: Get real-time water temperature data for a specific NOAA station


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NOAA Tides & Currents API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get tide predictions for station '9414290' (San Francisco) for '20240510' using NOAA Tides."

**🤖 AI Agent:**
> I've retrieved the tide predictions for San Francisco! Notable entries include a High Tide at 10:30 AM (5.2 ft) and a Low Tide at 4:45 PM (0.5 ft). Would you like the real-time water level or air temperature for this station?

---

**👤 You:**
> "What is the current water temperature at station '8443970' (Boston)?"

**🤖 AI Agent:**
> I've checked the sensors for Boston. The water temperature is currently 52°F. I can provide the historical temperature metadata for the last 24 hours if you'd like to identify trends.

---

**👤 You:**
> "Show real-time water levels for station '9410660' (Los Angeles)."

**🤖 AI Agent:**
> I've retrieved the real-time water levels for Los Angeles! The current value is identified as 3.2 ft above MLLW. I can assist you with an audit of predicted vs actual water level metadata if you'd like.


## Installation & Usage

To install and use the **NOAA Tides & Currents API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noaa-tides-currents-api](https://vinkius.com/mcp/noaa-tides-currents-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
