# Business Timezone & Holiday Scheduler MCP Server

Eradicate LLM scheduling errors. Calculate exact business days skipping global public holidays and convert precise timezones flawlessly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/business-timezone-holiday-scheduler)

## Overview
**Category:** productivity
**Tools Count:** 2

## Description
LLMs hallucinate dates. They forget leap years, daylight saving time rules, and have no idea when Easter or local bank holidays occur. This MCP makes your AI a perfect executive assistant by giving it real-time calendar and holiday intelligence.

### Superpowers

- **Business Day Calculation:** Ask the AI for a 45-day SLA deadline. The MCP automatically skips weekends and fetches actual national public holidays (via the public Nager.Date API) for any country.
- **Flawless Timezones:** Instantly convert meeting times between complex IANA timezones (e.g., from `America/Sao_Paulo` to `Asia/Tokyo`), accounting for real-world offset rules.


## Available Tools
- **add_business_days**: It automatically skips weekends. If you provide a countryCode (e.g. "US", "BR", "JP"), it will also query the Nager.Date API to skip national public holidays for that country.

Calculates a future date by adding a specific number of business days (skipping weekends and optional public holidays)
- **convert_timezone**: Uses IANA timezone strings (e.g. "America/Sao_Paulo", "Asia/Tokyo").

Converts an exact date and time from one timezone to another


## Installation & Usage

To install and use the **Business Timezone & Holiday Scheduler** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/business-timezone-holiday-scheduler](https://vinkius.com/mcp/business-timezone-holiday-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
