# Habitify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/habitify)
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


## ❓ FAQ

**Q: How do I find my Habitify API Key?**
Open the Habitify mobile app, go to **Settings > API Credentials** (or Settings > Account > API), and tap **Generate New Key**. Note that API access may require a premium subscription.

**Q: Can I record progress for my habits via the AI agent?**
Yes! Use the `add_habit_log` tool. You can specify the habit ID and the value you want to record (e.g., '10 reps' or '30 minutes').

**Q: Does the integration support viewing statistics?**
Yes, you can use the `get_habit_stats` tool to retrieve performance data for any habit within a specific date range, helping you analyze your consistency.

**Q: Can I create new habits through this integration?**
Yes! The `create_habit` tool allows you to add new habits to your Habitify account directly from your conversational interface.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/habitify](https://vinkius.com/mcp/habitify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Habitify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `habitify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Habitify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "habitify": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
