# TimezoneDB MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/timezonedb)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/timezonedb-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/timezonedb-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage global time — audit timezones and offsets via AI.

## Description
Empower your AI agent to orchestrate your entire global time and timezone research workflow with **TimezoneDB**, the authoritative source for world clock data. By connecting TimezoneDB to your agent, you transform complex offset lookups into a natural conversation. Your agent can instantly retrieve current time for any zone, audit daylight saving statuses, and identify regional time variations without you ever touching a manual converter. Whether you are planning international calls or building global scheduling systems, your agent acts as a real-time time consultant, ensuring your data is always precise and synchronized.

### What you can do

- **Time Auditing** — Retrieve the exact current time for over 400 timezones and maintain a clear view of global offsets.
- **Location Oversight** — Query timezone details based on geographic coordinates to understand local time patterns instantly.
- **Zone Discovery** — List all supported timezones by country to identify regional variations and abbreviations.
- **DST Intelligence** — Check if daylight saving time is currently active for any zone to assist in precise scheduling.
- **Spatial Discovery** — Retrieve latitude and longitude metadata for specific zones to maintain spatial context.

### How it works

1. Subscribe to this server
2. Enter your TimezoneDB API Key
3. Start managing your global time intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — monitor international team hours and retrieve zone metadata straight from your workflow.
- **Travel Coordinators** — verify local times and audit DST transitions without manual searching.
- **Data Engineers** — perform rapid audits of geographic time data and identify correct offsets through natural language.
- **App Developers** — automate timezone data querying to orchestrate cross-functional global services smoothly.


## Available Tools
- **check_api_status**: Check if the TimezoneDB API is operational
- **get_dst_status**: Check if daylight saving time is currently active for a zone
- **get_time_by_location**: Get current time for specific geographic coordinates
- **get_time_by_zone**: g., "America/New_York.

Get current time and details for a specific timezone (e.g., "America/New_York")
- **list_timezones**: List all supported timezones, optionally filtered by country


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TimezoneDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current time in 'Asia/Tokyo' using TimezoneDB?"

**🤖 AI Agent:**
> I've retrieved the current time for Tokyo. It is currently 10:30 PM (GMT+9). Daylight saving is not active. Would you like the details for another zone?

---

**👤 You:**
> "Check time for latitude 40.7128, longitude -74.0060."

**🤖 AI Agent:**
> I've identified the location as New York, United States (America/New_York). The current time is 8:30 AM (GMT-5). Would you like to check the DST status?

---

**👤 You:**
> "List all timezones in 'Brazil'."

**🤖 AI Agent:**
> I've scanned the zones for Brazil. It includes several timezones, such as America/Sao_Paulo (GMT-3) and America/Manaus (GMT-4). I can provide the current time for any of these.


## Installation & Usage

To install and use the **TimezoneDB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/timezonedb](https://vinkius.com/mcp/timezonedb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
