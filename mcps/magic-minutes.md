# Magic Minutes MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/magic-minutes)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Generate meeting minutes automatically with AI that listens, summarizes key decisions, and distributes action items to your team.

## Description
Connect your **Magic Minutes** account to any AI agent and take full control of your meeting orchestration and team productivity through natural conversation. Magic Minutes provides a comprehensive platform for organizing meetings, and this integration allows you to retrieve meeting metadata, manage action items (tasks), and oversee minutes directly from your chat interface.

### What you can do

- **Meeting & Agenda Orchestration** — List all managed meetings and retrieve detailed metadata programmatically to ensure your team's schedule is always synchronized.
- **Task & Action Lifecycle Management** — Create, update, and monitor meeting action items directly from the AI interface to maintain high-fidelity task execution.
- **Minutes & Summary Intelligence** — Access and monitor meeting attributes and retrieve detailed attendee metadata via natural language to drive better collaboration.
- **Folder & Structure Control** — List and oversee your meeting folders and organization metadata using simple AI commands.
- **Operational Monitoring** — Track system responses and manage contact metadata to ensure your meeting workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Magic Minutes API Key from your account settings
3. Start managing your meetings from Claude, Cursor, or any MCP-compatible client

No more manual searching for meeting notes in your inbox. Your AI acts as a dedicated meeting coordinator or administrative assistant.

### Who is this for?

- **Project Managers & Leads** — quickly retrieve meeting summaries and monitor task progress without switching apps.
- **Executive Assistants** — automate the retrieval of attendee metadata and track action item assignments via natural conversation.
- **Operations Managers** — streamline the retrieval of meeting folder metadata and monitor organizational productivity directly within the chat.


## Available Tools (12)
- **create_task**: Create a new task
- **get_current_user**: Get authenticated user profile
- **get_meeting_details**: Get details for a specific meeting
- **get_meeting_minutes**: Retrieve the minutes or agenda of a meeting
- **get_task_details**: Get details for a specific task
- **list_meeting_attendees**: List attendees for a meeting
- **list_contacts**: List all contacts
- **list_folders**: List folders and structure
- **list_meetings**: List all meetings
- **list_tasks**: List all tasks and action items
- **list_webhooks**: List active webhooks
- **check_api_health**: Check API health status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Magic Minutes** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my meetings from this week in Magic Minutes."

**🤖 AI Agent:**
> I've retrieved your meetings. You had 5 sessions this week, including 'Q4 Strategy' and 'Weekly Sync'. Which one would you like to see the minutes for?

---

**👤 You:**
> "Show me the action items for the 'Board Meeting'."

**🤖 AI Agent:**
> I've retrieved 3 action items: 1. Update budget (Sarah), 2. Finalize deck (John), 3. Schedule follow-up. Would you like me to create reminders for these?

---

**👤 You:**
> "List all attendees for today's sync."

**🤖 AI Agent:**
> There were 5 attendees: John Miller, Sarah Chen, and 3 external guests. Would you like to see their contact info?


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific meeting by its ID?**
Yes! Use the `get_meeting` tool with the Meeting ID. Your agent will respond with complete metadata for the record, including the agenda and start time in seconds.

**Q: How do I find my Magic Minutes API Key?**
Log in to your Magic Minutes account at magicminutes.co.uk, navigate to **Settings** > **API**, and you will find your unique secret token there.

**Q: Does it support task management?**
Yes, use the `list_tasks` tool to retrieve all action items generated during your meetings, allowing the AI to track team assignments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/magic-minutes](https://vinkius.com/mcp/magic-minutes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Magic Minutes** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `magic-minutes` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Magic Minutes** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "magic-minutes": {
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
