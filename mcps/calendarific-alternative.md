# Calendarific MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calendarific-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/calendarific-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/calendarific-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Universal holiday intelligence — get public, bank, and religious holidays worldwide via AI.

## Description
Equip your AI agent with global temporal intelligence through the **Calendarific** MCP server. This integration provides real-time access to a comprehensive database of public, bank, and religious holidays for over 200 countries. Your agent can retrieve holiday lists for specific years, filter results by month or day, and explore the list of supported countries and languages. Whether you are scheduling international meetings, planning travels, or auditing regional availability, your agent acts as a dedicated global calendar coordinator through natural conversation.

### What you can do

- **Holiday Retrieval** — Fetch all public and bank holidays for a country and year.
- **Temporal Filtering** — Narrow down holidays by specific months or days for precise scheduling.
- **Country Intelligence** — List all supported countries and their ISO codes for global operations.
- **Metadata Access** — View detailed holiday descriptions and types (religious, national, etc.).
- **Holiday Auditing** — Summarize and compare holiday calendars between different countries for better coordination.

### How it works

1. Subscribe to this server
2. Enter your Calendarific API Key (get it for free at calendarific.com)
3. Start querying global holidays from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — coordinate timelines across international teams by accounting for local holidays.
- **Travel Planners** — identify bank holidays and public festivals in destination countries.
- **Operations Teams** — automate calendar updates and regional availability checks.
- **E-commerce Managers** — plan marketing campaigns around specific regional and religious holidays.


## Available Tools
- **get_holidays**: Get holidays for a country and year
- **list_supported_countries**: List all supported countries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calendarific** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the bank holidays in the UK for May 2024?"

**🤖 AI Agent:**
> Retrieving UK holidays for May 2024... I've found two: the Early May Bank Holiday on May 6th and the Spring Bank Holiday on May 27th. Would you like more details?

---

**👤 You:**
> "Check if there are any holidays in Japan on November 3rd."

**🤖 AI Agent:**
> Checking Japanese calendar... Yes, November 3rd is 'Culture Day' (Bunka no Hi) in Japan. It is a national holiday to promote culture and the arts. Would you like to see other holidays in November?

---

**👤 You:**
> "List all countries supported by Calendarific."

**🤖 AI Agent:**
> Retrieving the country list... Calendarific supports over 200 countries and regions, including Afghanistan (AF), Brazil (BR), Canada (CA), France (FR), and Zimbabwe (ZW). I can provide the specific ISO code for any country you're interested in.


## Installation & Usage

To install and use the **Calendarific** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calendarific-alternative](https://vinkius.com/mcp/calendarific-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
