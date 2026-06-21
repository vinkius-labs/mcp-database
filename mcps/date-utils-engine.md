# Date Utils Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/date-utils-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/date-utils-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/date-utils-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Stop AI from hallucinating dates, missing leap years, or failing timezone conversions. Offloads all calendar math to the deterministic date-fns engine.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Date Utils Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add exactly 45 calendar days to `2026-02-15`."

**🤖 AI Agent:**
> ✅ **New Date:** `2026-04-01`

---

**👤 You:**
> "Calculate the exact number of days between `2024-01-01` and `2024-12-25`."

**🤖 AI Agent:**
> ✅ **Difference:** There are exactly `359` days between the two dates (accounts for leap year natively).

---

**👤 You:**
> "Convert the UTC timestamp `2026-06-15T12:00:00Z` to the `America/Sao_Paulo` timezone."

**🤖 AI Agent:**
> ✅ **Timezone Shift:** `2026-06-15 09:00:00-03:00`


## Installation & Usage

To install and use the **Date Utils Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/date-utils-engine](https://vinkius.com/mcp/date-utils-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
