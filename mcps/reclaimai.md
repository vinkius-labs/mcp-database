# Reclaim.ai MCP Server

Equip your AI to directly manage tasks, habits, and scheduling links via your smart Reclaim.ai calendar assistant.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/reclaimai)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Reclaim.ai** intelligent scheduling assistant directly to your AI agent. Enabling this integration turns your AI into an advanced executive assistant, capable of instantly scanning your schedule, managing priorities, and inserting new smart tasks into your Google Calendar effortlessly.

### What you can do

- **Smart Task Management** — Create, update, or delete dynamic tasks, adjusting their duration and priority while letting Reclaim handle the automated calendar placement.
- **Habit Tracking** — Review your recurring protected time blocks (Habits) scheduled to accommodate deep work, routines, and breaks.
- **Calendar Review** — List both manual and AI-scheduled events for specific date ranges to understand your true availability.
- **Scheduling Links** — Retrieve your shareable booking page URLs instantly to send to teammates or clients directly from chat.
- **Time Analytics** — Extract quantitative data tracking how you allocate focus across categories over customized ranges.

### How it works

1. Authorize the Reclaim.ai MCP server within your platform.
2. Add your Reclaim API Key (obtained from your Reclaim Settings > Integrations dashboard).
3. Ask your AI to block off 2 hours for a new "Q3 Report" task with 'P1' priority or retrieve a meeting link for your next prompt.

### Who is this for?

- **Founders & Executives** — Seamlessly clear out calendar conflicts and command the AI to protect time for strategic initiatives without context switching.
- **Project Managers** — Bulk load weekly team action items straight to Reclaim and let the AI balance individual workloads and task durations.
- **Developers (Deep Work)** — Dynamically review assigned sprints and generate unbreakable focus blocks via the `create_task` directive directly from IDE terminals.


## Available Tools
- **create_task**: Specify title, duration in minutes, due date, and priority (P1 to P4).

Creates a new task to be auto-scheduled by Reclaim.ai
- **delete_task**: This action is irreversible.

Deletes a task from Reclaim.ai
- **get_analytics**: Retrieves time analytics for a specific date range
- **get_current_user**: Retrieves the authenticated user profile
- **get_task**: Retrieves details for a specific Reclaim.ai task
- **list_calendar_events**: Lists all events on the Reclaim.ai planner for a date range
- **list_habits**: Lists all habits configured in Reclaim.ai
- **list_scheduling_links**: Lists all Reclaim.ai scheduling links
- **list_tasks**: You can filter by status (NEW, SCHEDULED, IN_PROGRESS, COMPLETE).

Lists all tasks managed by Reclaim.ai
- **update_task**: Provide a JSON object with the updates.

Updates an existing Reclaim.ai task


## Installation & Usage

To install and use the **Reclaim.ai** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reclaimai](https://vinkius.com/mcp/reclaimai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
