# Reclaim.ai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reclaimai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI to directly manage tasks, habits, and scheduling links via your smart Reclaim.ai calendar assistant.

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


## Available Tools (10)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reclaim.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new task to draft the Q3 analytics report taking 3 hours with P1 priority."

**🤖 AI Agent:**
> I submitted the `create_task` command for your Q3 analytics report (duration: 180 min, priority: P1). Reclaim has successfully added it to your backlog and is actively attempting to secure dedicated focus blocks on your calendar before any deadlines.

---

**👤 You:**
> "Delete task with ID 20392."

**🤖 AI Agent:**
> Using the `delete_task` operation, I have permanently removed the task with ID 20392. Note that any calendar holds or events associated solely with this auto-scheduled task have also been cleared from your calendar.

---

**👤 You:**
> "Show my time spent analytics between 2024-01-01 and 2024-01-31."

**🤖 AI Agent:**
> I requested your statistical summary via `get_analytics`. During January 2024, you dedicated roughly 84 hours to 'Deep Work', spent 30 hours locked in manual multi-participant meetings, and sustained your 'Reading' habit strictly spanning 12 aggregate hours across 20 distinct days.


## ❓ FAQ

**Q: Where do I obtain my Reclaim API Key?**
Log into your Reclaim.ai web application. Head towards 'Settings', select 'Integrations' from the sidebar, and look for 'API' at the bottom of the connected apps. Generate your personal token there and provide it using the setup authorization parameter below.

**Q: Does creating a task automatically schedule it on my calendar?**
Yes. When the AI uses the `create_task` tool, Reclaim.ai takes your input duration, designated priority (P1 to P4), and due date to contextually slot it securely into an available window on your connected Google or Outlook calendar without extra prompts.

**Q: Can I query what was already booked in the past by AI vs manually added?**
Yes. The `list_calendar_events` query imports event types accurately across any given time period, allowing the AI to effectively understand both the manual meetings you accepted and the tasks Reclaim auto-negotiated on your schedule.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reclaimai](https://vinkius.com/mcp/reclaimai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reclaim.ai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reclaimai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reclaim.ai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reclaimai": {
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
