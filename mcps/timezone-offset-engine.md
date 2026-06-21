# Timezone Offset Engine MCP Server

Calculate the exact offset between two timezones at any moment, with full DST awareness. Powered by Luxon.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/timezone-offset-engine)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
When a scheduling agent needs to know the time difference between São Paulo and London on July 15th, the answer changes depending on DST. LLMs get DST wrong 100% of the time. This MCP uses Luxon with the full IANA timezone database.

### The Superpowers

- **DST Aware:** Calculates offsets at a specific moment, correctly handling all DST transitions worldwide.
- **Full IANA Database:** Supports all 400+ IANA timezones (America/Sao_Paulo, Europe/London, Asia/Kolkata, etc.).
- **Bidirectional:** Shows both the source and target local times plus the exact offset in hours and minutes.


## Available Tools
- **get_timezone_offset**: Pass two IANA timezone names (e.g. "America/Sao_Paulo", "Europe/London") and optionally an ISO 8601 datetime. The engine returns the exact offset in hours/minutes and whether each zone is in DST. Never calculate DST offsets yourself — you will get it wrong.

Calculates the exact offset between two IANA timezones at a specific moment, respecting Daylight Saving Time (DST). Powered by Luxon


## Installation & Usage

To install and use the **Timezone Offset Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/timezone-offset-engine](https://vinkius.com/mcp/timezone-offset-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
