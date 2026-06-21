# BR Business Days Calculator MCP Server

Stop LLMs from calculating SLAs incorrectly. An local, deterministic engine that adds business days while perfectly avoiding weekends and Brazilian national holidays.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/br-business-days-calculator)

## Overview
**Category:** productivity
**Tools Count:** 2

## Description
LLMs cannot reliably calculate SLAs or business delivery times. If you ask an AI to 'add 5 business days to Feb 10th', it will frequently ignore Carnival or count a Saturday. This MCP solves this by providing a static, local-first calculation engine that perfectly handles Brazilian national holidays and weekends.

### The Superpowers

- **Flawless SLA Math:** Guarantee that your agents' promised delivery dates are exactly right, automatically skipping weekends and static/dynamic BR holidays.
- **Zero Latency & 100% Local:** Unlike our global `business-timezone-scheduler` that uses the Nager.Date API, this engine uses a hardcoded Brazilian holiday list in the V8 isolate. Zero external network calls. Instant execution.
- **Absolute Determinism:** Eliminates the hallucination of non-existent business days, bringing enterprise reliability to AI agents.


## Available Tools
- **add_business_days**: Pass a starting date and the number of days to add (use negative values to subtract). The engine skips weekends and Brazilian holidays automatically.

Adds or subtracts X Brazilian business days from a given date
- **is_business_day**: Pass the date as an ISO string (YYYY-MM-DD). The engine accounts for all Brazilian national holidays and weekends.

Checks if a given date is a Brazilian business day (excludes weekends and BR national holidays)


## Installation & Usage

To install and use the **BR Business Days Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/br-business-days-calculator](https://vinkius.com/mcp/br-business-days-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
