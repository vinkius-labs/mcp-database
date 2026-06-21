# World Time (Keyless) MCP Server

Get precise current atomic time, UTC offsets, and DST states for any timezone worldwide — no API key required.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/world-time-keyless)

## Overview
**Category:** productivity
**Tools Count:** 2

## Description
Connect to the **World Time API** and empower your AI agent with precise, synchronized time data through natural conversation. This server provides micro-service level access to atomic time across all IANA timezone regions without requiring any manual signups or complex API keys.

### What you can do

- **Precise Synchronization** — Retrieve the exact current time for any valid IANA region (e.g., 'Europe/London' or 'America/New_York') with millisecond precision
- **Offset Discovery** — Verify the current UTC offset and check whether a specific location is currently observing Daylight Saving Time (DST)
- **Timezone Browsing** — List all supported timezone strings to ensure you are using the correct identifier for your requests
- **IP-Based Inference** — Automatically retrieve the current local time based on the inferred location of the network IP address
- **Standardized Data** — Access high-quality JSON responses including Unix timestamps, day of year, and week number for scheduling purposes
- **Global Coverage** — Get reliable time data for any part of the world, from major cities to remote islands

### How it works

1. Subscribe to this server
2. No API Key required (just click connect)
3. Start asking about the time in any city through Claude, Cursor, or any MCP-compatible client

No more manual math to figure out a time difference. Your AI agent becomes your global master clock.

### Who is this for?

- **Developers** — verify UTC offsets and time synchronization for server-side logging or scheduling
- **Project Managers** — quickly check local times for distributed team members before planning meetings
- **Operations Teams** — monitor DST transitions and verify week numbers for business reporting
- **Everyday Users** — find out what time it is anywhere in the world through a simple chat command


## Available Tools
- **get_current_time**: You can provide a timezone string (e.g. "America/Sao_Paulo") or use "ip" to infer from the network.

Retrieves the exact current atomic time, UTC offset, and DST state for a specified timezone
- **list_available_timezones**: Lists all valid timezone regions (e.g. Europe/London) supported by the World Time API


## Installation & Usage

To install and use the **World Time (Keyless)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/world-time-keyless](https://vinkius.com/mcp/world-time-keyless)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
