# RescueTime MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rescuetime)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track productivity, manage Focus Sessions, and analyze time usage directly from your AI agent.

## Description
Connect your **RescueTime** account to any AI agent to gain deep insights into your productivity and manage your focus in real-time through natural conversation.

### What you can do

- **Productivity Analytics** — Query historical activity data, category breakdowns, and efficiency metrics using `get_analytic_data`.
- **Focus Management** — Trigger or end Focus Sessions programmatically to block distractions with `start_focus_time` and `end_focus_time`.
- **Daily Summaries** — Get high-level rollups of your time logged and productivity pulse via `get_daily_summary_feed`.
- **Highlights & Achievements** — Log daily wins and retrieve your highlights feed to track progress over time.
- **Offline Logging** — Record time spent in meetings or exercise to maintain a complete picture of your day.

### How it works

1. Subscribe to this server
2. Enter your RescueTime API Key
3. Start optimizing your workflow from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Knowledge Workers** — stay in the flow by starting focus sessions directly from your IDE or chat.
- **Managers** — retrieve team-level productivity trends and summaries without manual reporting.
- **Self-Improvement Enthusiasts** — analyze time spent on specific activities to build better habits.


## Available Tools (54)
- **add_offline_focus_work**: Add offline focus time (accumulates)
- **archive_project**: Archive or restore a project
- **cancel_or_stop_focus_session**: End active focus session
- **create_alert**: Create an alert
- **create_extra_work**: Create an extra-work entry
- **create_goal**: Create a goal
- **create_project**: Create a project
- **delete_timeline_activities**: Bulk delete tracked time in a range
- **end_focus_time**: End the current Focus Session (Premium only)
- **extend_focus_session**: Extend active session duration
- **get_accounts**: Retrieve account-level settings
- **get_alerts**: List active alerts
- **get_alerts_feed**: Get running log of recently triggered user-defined alerts
- **get_analytic_data**: Query historical activity data and productivity metrics
- **get_calendar_events**: List synced calendar events
- **get_categories**: List activity categories
- **get_daily_summary_feed**: Get high-level rollup of daily time logged
- **get_daily_user_summaries**: Get pre-computed daily roll-ups
- **get_devices**: List user-machines that have reported time
- **get_extra_works**: List extra-work entries
- **get_focus_sessions**: List persistent session records
- **get_focustime_ended_feed**: Get feed of ended Focus Sessions
- **get_focustime_started_feed**: Get feed of started Focus Sessions
- **get_goals**: List goals
- **get_highlights_feed**: Get daily highlights feed (Premium only)
- **get_managed_users**: List users in teams managed by the caller
- **get_meeting_events**: List events classified as meetings
- **get_organizations**: Retrieve organization details
- **get_overview_tree**: Get personalized hierarchy with scoring overrides
- **get_overviews**: List top-level activity buckets
- **get_productivities**: List productivity score definitions
- **get_profile_entities**: List per-account category/score overrides
- **get_projects**: List projects
- **get_schedules**: List work schedules
- **get_tasks**: List tasks
- **get_teams**: List teams the user belongs to
- **get_timeline_activities**: Fetch normalized activity stream for a day
- **get_user_settings**: Retrieve API-writable user settings
- **get_users**: Retrieve current user info
- **get_web_notification_counts**: Get read/unread counts for notifications
- **get_web_notifications**: List in-app notifications
- **log_project_time**: Log time against a project/task
- **merge_project_time**: Combine adjacent time entries
- **opt_in_beta**: Opt in or out of beta features
- **post_highlight**: Create a new daily highlight (Premium only)
- **post_offline_time**: Log offline time (Premium only)
- **register_live_activity**: Register Apple Live-Activity push tokens
- **start_focus_session**: Start a global focus session
- **start_focus_time**: Trigger a Focus Session (Premium only)
- **start_focus_zone**: Start a focus zone (DND block)
- **toggle_timesheet_finalized**: Toggle finalization (lock) for a date
- **update_user**: Update user profile settings
- **update_web_notification**: Mark notification as read or dismissed
- **upsert_profile_entity**: Upsert an override for an app/site


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RescueTime** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my productivity summary for the last 7 days."

**🤖 AI Agent:**
> I've retrieved your daily summary feed. Over the last week, your average productivity pulse was 72. Your most productive day was Tuesday, with 6 hours of focused work logged.

---

**👤 You:**
> "Start a 45-minute Focus Session for me."

**🤖 AI Agent:**
> Focus Session started! I've triggered a 45-minute session via RescueTime. Distractions are now blocked so you can stay in the zone. Good luck!

---

**👤 You:**
> "What were my top 5 most distracting activities yesterday?"

**🤖 AI Agent:**
> Analyzing your activity data... Yesterday, your top distractions were: 1. YouTube (45m), 2. Twitter (30m), 3. News sites (20m), 4. Personal Email (15m), and 5. Reddit (10m).


## ❓ FAQ

**Q: Can I start a Focus Session directly from the chat?**
Yes! Use the `start_focus_time` tool and specify the duration in minutes. Your agent will trigger the session to block distracting websites and apps immediately.

**Q: How do I see my top productivity categories for yesterday?**
You can ask the agent to run `get_analytic_data` with `restrict_kind` set to 'category' and the dates set to yesterday. It will return a ranked list of where your time went.

**Q: Is it possible to log achievements or daily wins?**
Absolutely. Use the `post_highlight` tool to record a description of what you accomplished. You can later retrieve these using `get_highlights_feed`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rescuetime](https://vinkius.com/mcp/rescuetime)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RescueTime** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rescuetime` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RescueTime** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rescuetime": {
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
