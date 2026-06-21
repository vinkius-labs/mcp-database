# Habitify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/habitify)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/habitify-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/habitify-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate habit tracking via Habitify — manage habits, logs, and personal growth directly from any AI agent.

## Description
Connect your **Habitify** account to any AI agent and take full control of your personal growth and habit-tracking workflows through natural conversation.

### What you can do

- **Habit Oversight** — List all habits you are tracking and retrieve detailed information for each.
- **Journal Monitoring** — Get a daily overview of your completion status and progress for any specific date.
- **Log Management** — Record progress for your habits (reps, minutes, etc.) and view history logs efficiently.
- **Statistical Insights** — Retrieve performance statistics for any habit within a custom date range.
- **Personalized Growth** — Create new habits or update existing ones directly from your chat or IDE.
- **Area Categorization** — Organize and browse your habits by areas of focus like Health, Work, or Mindset.

### How it works

1. Subscribe to this server
2. Enter your Habitify API Key (found in app Settings)
3. Start managing your habits from Claude, Cursor, or any MCP-compatible client

No more manual data entry in the mobile app. Your AI assistant acts as a dedicated accountability partner and habit coach.

### Who is this for?

- **High Performers** — instantly check daily goals and log progress without switching apps.
- **Productivity Enthusiasts** — automate habit reporting and analyze long-term trends through conversation.
- **Self-Improvement Seekers** — integrate habit tracking into your daily digital workflow for better consistency.


## Available Tools
- **add_habit_log**: g., number of reps, minutes, or completion) to a habit.

Record progress for a specific habit
- **create_habit**: Create a new habit to track
- **delete_habit**: Permanently delete a habit
- **get_habit**: Get detailed information about a specific habit
- **get_habit_stats**: Get statistics for a habit within a date range
- **get_journal**: Get habits with completion status for a specific date
- **list_areas**: List all habit areas (categories)
- **list_habits**: List all habits in your Habitify account
- **list_habit_logs**: List all logs for a specific habit
- **update_habit**: Update an existing habit details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Habitify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What habits do I need to complete today?"

**🤖 AI Agent:**
> I've checked your journal for today. You have 4 habits pending: 'Drink 2L Water', 'Morning Meditation', 'Read 20 Pages', and 'Go for a Run'. Which one would you like to log progress for?

---

**👤 You:**
> "Log 30 minutes of reading for today."

**🤖 AI Agent:**
> Habit log added! I've successfully recorded 30 minutes for your 'Reading' habit. Keep up the great consistency!

---

**👤 You:**
> "Show me my stats for 'Morning Meditation' from last week."

**🤖 AI Agent:**
> Retrieving statistics... Last week, you completed 'Morning Meditation' 5 out of 7 days (71% consistency). Your longest streak for this habit is currently 12 days. Would you like to see the details for the missed days?


## Installation & Usage

To install and use the **Habitify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/habitify](https://vinkius.com/mcp/habitify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
