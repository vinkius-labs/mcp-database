# WakaTime (Coding Stats) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wakatime-coding-stats)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wakatime-coding-stats-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wakatime-coding-stats-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track your coding activity and productivity metrics directly through WakaTime — monitor projects, goals, and time spent in your IDE.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WakaTime (Coding Stats)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my coding stats for the last 7 days."

**🤖 AI Agent:**
> I've retrieved your stats for the last 7 days. You coded for a total of 24 hours and 15 minutes. Your top language was TypeScript (12h), followed by Python (8h). Your most active project was 'vurb-mcp-server'.

---

**👤 You:**
> "What are my current coding goals and how am I doing?"

**🤖 AI Agent:**
> You have 2 active goals: 'Code 4 hours daily' which is currently at 85% completion for this week, and 'Contribute to Open Source' which is at 40%. Keep it up!

---

**👤 You:**
> "Give me a summary of my coding activity for yesterday."

**🤖 AI Agent:**
> Yesterday, you logged 5 hours and 30 minutes of coding activity. You worked on 3 projects: 'API-Gateway' (3h), 'Frontend-App' (2h), and 'Documentation' (30m).


## Installation & Usage

To install and use the **WakaTime (Coding Stats)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wakatime-coding-stats](https://vinkius.com/mcp/wakatime-coding-stats)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
