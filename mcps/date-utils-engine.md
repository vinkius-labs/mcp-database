# Date Utils Engine MCP Server

Stop AI from hallucinating dates, missing leap years, or failing timezone conversions. Offloads all calendar math to the deterministic date-fns engine.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/date-utils-engine)

## Overview
**Category:** loved-by-devs
**Tools Count:** 4

## Description
LLMs suffer from 'calendar blindness'. Because they lack a continuous clock and process dates as text tokens, asking an AI 'What is 45 days from October 12th?' often results in a hallucinated, incorrect date (forgetting November has 30 days, or missing a leap year). This MCP brings the industry standard `date-fns` and `date-fns-tz` to your agentic workflows.

### The Superpowers

- **Flawless Date Math:** Safely add or subtract days, months, and years while guaranteeing 100% calendar accuracy.
- **Timezone Mastery:** Convert UTC timestamps into any exact IANA timezone (e.g. `America/Sao_Paulo`) automatically accounting for Daylight Savings Time shifts without guessing.
- **Zero Latency:** Executes as native V8 javascript local. Does not rely on external calendar APIs.


## Available Tools
- **add_days**: Pass the base ISO date and the number of days (negative to subtract). Receives the exact resulting date.

Adds or subtracts a specific number of calendar days from a date deterministically
- **diff_dates**: Pass both ISO date strings and receive the delta in days, hours, minutes, and seconds.

Calculates the exact number of calendar days between two dates
- **parse_date**: Pass the raw date string and receive a confirmed valid date object.

Parses an ISO date string safely to ensure it is valid
- **to_timezone**: Pass the ISO date string and the IANA timezone identifier (e.g. "America/Sao_Paulo", "Europe/London"). Accounts for daylight saving time automatically.

Converts a UTC or ISO date string to a specific IANA timezone safely accounting for daylight savings


## Installation & Usage

To install and use the **Date Utils Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/date-utils-engine](https://vinkius.com/mcp/date-utils-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
