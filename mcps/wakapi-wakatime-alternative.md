# Wakapi (WakaTime Alternative) MCP Server

Track coding time, analyze productivity stats, and manage projects via Wakapi — an open-source WakaTime alternative.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/wakapi-wakatime-alternative)

## Overview
**Category:** productivity
**Tools Count:** 4

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


## Installation & Usage

To install and use the **Wakapi (WakaTime Alternative)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wakapi-wakatime-alternative](https://vinkius.com/mcp/wakapi-wakatime-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
