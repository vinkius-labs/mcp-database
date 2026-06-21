# Wakapi (WakaTime Alternative) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wakapi-wakatime-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wakapi-wakatime-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wakapi-wakatime-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track coding time, analyze productivity stats, and manage projects via Wakapi — an open-source WakaTime alternative.

## Description
Connect your **Wakapi** instance to any AI agent to monitor your development workflow through natural conversation. Wakapi is a self-hosted, open-source alternative to WakaTime that tracks your coding activity across different editors and languages.

### What you can do

- **Coding Statistics** — Retrieve detailed stats including languages, editors, and operating systems used over various time ranges using `get_stats`.
- **Activity Summaries** — Fetch granular summaries of your work for specific date ranges or individual projects with `get_summaries`.
- **Project Listing** — View all projects you have tracked time for using `list_projects` to keep your portfolio or billable hours organized.
- **Heartbeat Tracking** — Manually send coding activity heartbeats via `send_heartbeats` to ensure your timeline is always accurate.

### How it works

1. Subscribe to this server
2. Enter your Wakapi API URL and API Key
3. Start analyzing your coding habits from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Individual Developers** — track your own productivity and see which languages you spend the most time on.
- **Engineering Managers** — get high-level summaries of team activity and project distribution.
- **Freelancers** — accurately report time spent on specific client projects without manual timers.


## Available Tools
- **send_heartbeats**: Provide a heartbeat object or an array of heartbeat objects.

Send coding activity heartbeats to Wakapi
- **list_projects**: List all projects tracked by the user
- **get_stats**: Retrieve coding statistics for a user
- **get_summaries**: Retrieve a detailed summary of activity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wakapi (WakaTime Alternative)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show my coding stats for the last 7 days."

**🤖 AI Agent:**
> I've retrieved your stats for the last week. You spent 24 hours coding, primarily in TypeScript (60%) using VS Code. Your most active project was 'mcp-server-wakapi'.

---

**👤 You:**
> "List all my projects tracked in Wakapi."

**🤖 AI Agent:**
> I found 12 projects in your Wakapi account. Some of the recent ones include: 'website-frontend', 'api-backend', and 'mobile-app-v2'. Would you like stats for any of these?

---

**👤 You:**
> "Get a summary of my activity from 2023-10-01 to 2023-10-07."

**🤖 AI Agent:**
> Generating summary for that week... You logged a total of 32 hours. Your peak activity was on Tuesday with 8 hours of work across 3 different projects.


## Installation & Usage

To install and use the **Wakapi (WakaTime Alternative)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wakapi-wakatime-alternative](https://vinkius.com/mcp/wakapi-wakatime-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
