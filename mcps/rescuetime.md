# RescueTime MCP Server

Track productivity, manage Focus Sessions, and analyze time usage directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/rescuetime)

## Overview
**Category:** productivity
**Tools Count:** 54

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


## Available Tools
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


## Installation & Usage

To install and use the **RescueTime** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rescuetime](https://vinkius.com/mcp/rescuetime)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
