# Sunsama MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sunsama)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect your AI to Sunsama. Actively manage your day, orchestrate tasks, and balance your work natively from the terminal.

## Description
Integrate the mindful focus of the **Sunsama** daily planner directly into your conversational AI environment. Empower your engineering or administrative focus by allowing your LLM to intuitively pull tasks, filter backlog activities, and assign contexts dynamically without constant tab-switching. With this MCP connector attached securely to your workspace, your conversational agent functions as an objective scheduling assistant, seamlessly tracking and resolving your agenda.

### What you can do

- **Agenda Discovery** — Query your scheduled events actively using `list_tasks` and retrieve deep contextual dependencies of an item utilizing `get_task_details`.
- **Task Orchestration** — Add new action items seamlessly via `create_task` or modify ongoing assignments intuitively using `update_task`.
- **Taxonomy Mapping** — Review your organizational frameworks executing `list_channels` and `list_contexts` to accurately file items according to team domains.
- **Profile Confirmations** — Safely extract your user metadata boundaries and operational statuses natively invoking `get_user_profile`.

### How it works

1. Enable the Sunsama MCP module orchestrator as an active system integration.
2. Bind your verified `SUNSAMA_API_KEY` directly from your workspace parameters precisely to your environment matrix.
3. Instruct your artificial intelligence concisely: "Analyze my pending tasks for today, generate a new assigned block under the 'Development' channel, and mark yesterday's review as completed."

### Who is this for?

- **Founders & Executives** — Mitigate schedule conflicts iteratively without breaking focus, directing agenda adjustments via an analytical AI agent.
- **Software Engineers** — Centralize your daily planned agenda cleanly inside your IDE or local conversational CLI, reporting progress directly in real-time.
- **Project Managers** — Consolidate activities safely tracking team deliverables and personal timelines without bloated secondary interfaces.


## Available Tools (8)
- **create_task**: Provide text and an optional planned date.

Creates a new task in Sunsama
- **get_user_profile**: Retrieves the current user profile
- **list_tasks**: You can filter by date.

Lists all tasks in Sunsama
- **update_task**: Updates an existing task
- **delete_task**: This action is irreversible.

Permanently deletes a task
- **get_task_details**: Retrieves details for a specific task
- **list_channels**: g., "Work", "Personal").

Lists available Sunsama channels
- **list_contexts**: Lists available Sunsama contexts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sunsama** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my tasks for today, complete the design review, and schedule a documentation update for next Monday."

**🤖 AI Agent:**
> Accessing API matrix logically and retrieving tasks...
**Today's Schedule (`list_tasks`)**:
- `Design Architecture Review`
- `Sprint Synchronization`

Applying targeted operational parameters resolutely:
- Task `Design Architecture Review` successfully marked as complete naturally.
- Executed `create_task` effectively. "Documentation Update" dynamically listed safely on schedule appropriately.

---

**👤 You:**
> "Read my custom organizational domains running `list_channels` securely, and pull contextual details applying `list_contexts` effectively."

**🤖 AI Agent:**
> Verifying team structures reliably properly structurally...
**Team Compartments (`list_channels`)**:
- `Frontend Sprints`
- `Platform Reliability`

**Tag Frameworks (`list_contexts`) smoothly optimally**:
- Context `Urgent` and `Low Priority` mapped correctly.

---

**👤 You:**
> "Verify my identity token evaluating the API user profile comprehensively."

**🤖 AI Agent:**
> Parsing account telemetry cleanly natively...
**User Profile Confirmation (`get_user_profile`)**:
The workspace environment authorized your access efficiently as `Admin` under your active operational email directly seamlessly. Done.


## ❓ FAQ

**Q: Are organizational channels safely isolated when using programmatic executions?**
Yes. The AI intrinsically utilizes `list_channels` and `list_contexts` effectively to accurately parse pre-existing frameworks before assignment seamlessly.

**Q: Can the agent inadvertently destroy historical tracking via deletion?**
The tool bounds the logic reliably using isolated mutation calls like `delete_task`. These are triggered explicitly, protecting chronological historical records systematically effectively internally.

**Q: Does the integration sync with external calendars like Google Calendar?**
The MCP operates through the Sunsama API, which already consolidates events from Google Calendar, Outlook, and other connected services. Tasks you create or update via the AI will appear alongside your synced calendar events.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sunsama](https://vinkius.com/mcp/sunsama)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sunsama** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sunsama` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sunsama** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sunsama": {
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
