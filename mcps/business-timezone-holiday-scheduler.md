# Business Timezone & Holiday Scheduler MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/business-timezone-holiday-scheduler)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/business-timezone-holiday-scheduler-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/business-timezone-holiday-scheduler-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Eradicate LLM scheduling errors. Calculate exact business days skipping global public holidays and convert precise timezones flawlessly.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Business Timezone & Holiday Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If I sign a contract in Brazil today (2026-05-15), what is the exact date 45 business days from now, skipping Brazilian holidays?"

**🤖 AI Agent:**
> I calculated 45 business days from 2026-05-15.

Skipping all weekends and public holidays in Brazil (BR), your deadline falls precisely on: **July 20, 2026**.

---

**👤 You:**
> "Convert our project launch time (October 15, 2026 at 14:30 in New York) to Tokyo time."

**🤖 AI Agent:**
> I converted the timezone.

**From (America/New_York):** October 15, 2026 at 2:30 PM
**To (Asia/Tokyo):** October 16, 2026 at 3:30 AM

Your launch in Tokyo will be early the next morning.


## Installation & Usage

To install and use the **Business Timezone & Holiday Scheduler** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/business-timezone-holiday-scheduler](https://vinkius.com/mcp/business-timezone-holiday-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
