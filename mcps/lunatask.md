# Lunatask MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lunatask)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage tasks, habits, and notes via the Lunatask REST API (Encrypted Metadata Only).

## Description
Connect your **Lunatask** account to any AI agent to streamline your privacy-focused productivity. This MCP server enables your agent to create, update, and manage tasks, track habits, and log journal entries directly from natural language interfaces.

### What you can do

- **Task Creation** — Add new tasks to specific Areas of Life with statuses like 'next' or 'later'
- **Habit Tracking** — Log completions for your daily habits to stay consistent with your goals
- **Encrypted Journaling** — Create secure, end-to-end encrypted journal entries directly from your conversation
- **Metadata Inspection** — List all tasks and notes to monitor your productivity structure and statuses
- **Workflow Management** — Update task priorities and move them through your personal workflow stages

### Important Note on Privacy

Lunatask uses end-to-end encryption. While this API allows creating and updating content, **it cannot read back the names or notes** of your tasks once they are stored. The agent will only see technical metadata (IDs, dates, statuses).

### How it works

1. Subscribe to this server
2. Enter your Lunatask Access Token
3. Start managing your productivity from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Privacy-Conscious Professionals** — Manage your tasks via AI without compromising the encryption of your content
- **Goal-Oriented Individuals** — Quickly track habits and log journal thoughts via natural language commands
- **Power Users** — Automate task creation and organizational metadata updates directly from your development tools


## Available Tools
- **create_journal_entry**: Add a new journal entry
- **create_new_task**: Requires a name and an area_id.

Create a new task
- **delete_task**: Delete a task
- **get_task_metadata**: Get metadata for a specific task
- **list_notes_metadata**: List metadata for all notes
- **list_tasks_metadata**: Note: Due to encryption, names and notes are not available via API.

List metadata for all tasks
- **track_habit_completion**: Log a completion for a habit
- **update_existing_task**: Update an existing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lunatask** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List metadata for all my tasks in Lunatask."

**🤖 AI Agent:**
> I've retrieved the metadata for your tasks. You have 12 tasks across various areas. Note that I can see statuses like 'next' and 'later', but the actual task names are encrypted.

---

**👤 You:**
> "Track a completion for habit ID 'habit-123'."

**🤖 AI Agent:**
> Successfully logged a completion for habit 'habit-123'. Your consistency has been updated in Lunatask.

---

**👤 You:**
> "Create a new task named 'Review quarterly report' in area 'area-abc'."

**🤖 AI Agent:**
> I've sent the request to create the task. While I cannot read it back due to encryption, the new entry has been successfully added to your area 'area-abc'.


## ❓ FAQ

**Q: Why can't the agent read my task names?**
Lunatask uses end-to-end encryption. Task names and note bodies are encrypted on your device before being sent to the server. The API only has access to metadata like IDs and statuses.

**Q: Where do I find my Area ID?**
In the Lunatask desktop app, go to an Area's settings. The unique Area ID (UUID) is displayed there for use in the API.

**Q: Can I track habits using this agent?**
Yes, use the `track_habit_completion` tool with the unique habit ID to log a successful completion event.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lunatask](https://vinkius.com/mcp/lunatask)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lunatask** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lunatask` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lunatask** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lunatask": {
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
