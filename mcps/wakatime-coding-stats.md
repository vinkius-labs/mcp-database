# WakaTime (Coding Stats) MCP Server

Track your coding activity and productivity metrics directly through WakaTime — monitor projects, goals, and time spent in your IDE.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/wakatime-coding-stats)

## Overview
**Category:** productivity
**Tools Count:** 14

## Description
Connect your **WakaTime** account to any AI agent to analyze your coding habits, track project progress, and monitor productivity goals through natural conversation.

### What you can do

- **Coding Statistics** — Get summarized stats for specific ranges (7 days, 30 days, etc.) or your all-time total coding time.
- **Project Tracking** — List all projects detected by your IDE plugins and see daily summaries of activity per project.
- **Goal Monitoring** — Check your progress on custom coding goals and retrieve specific details for individual targets.
- **Activity Analysis** — Inspect raw heartbeats and duration blocks to understand exactly when and how you are working.

### How it works

1. Subscribe to this server
2. Enter your WakaTime API Key
3. Start querying your coding data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — track your own productivity and see which projects consume most of your time.
- **Team Leads** — monitor high-level project activity and goal progress without manual reporting.
- **Data Enthusiasts** — analyze coding patterns and heartbeats to optimize your workflow.


## Available Tools
- **create_external_duration**: Create activity from an external app
- **create_heartbeat**: Create a raw coding activity ping
- **get_all_time_since_today**: Get total time logged since account creation
- **get_goal**: Get a specific user-defined coding goal
- **get_stats**: Get summarized coding statistics for a given range
- **list_commits**: List of commits for a project with time spent on each
- **list_custom_rules**: Get rules to modify or delete coding activity based on patterns
- **list_durations**: Get coding activity joined into blocks based on keystroke timeout
- **list_external_durations**: g., Google Calendar).

Get activity created from external apps
- **list_goals**: List user-defined coding goals and their progress
- **list_heartbeats**: Get raw coding activity pings from IDE plugins
- **list_projects**: List of projects detected for the user
- **list_summaries**: Get daily totals of coding activity
- **update_custom_rules**: Update rules to modify or delete coding activity


## Installation & Usage

To install and use the **WakaTime (Coding Stats)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wakatime-coding-stats](https://vinkius.com/mcp/wakatime-coding-stats)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
