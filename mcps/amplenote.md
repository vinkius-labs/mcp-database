# Amplenote MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amplenote)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect your Amplenote workspace to your AI agent — search notes, manage tasks, and organize ideas via natural language.

## Description
Connect your **Amplenote** account to any AI agent to fuse your personal knowledge base and task manager directly into your daily computational workflows.

### What you can do

- **Notes & Ideas** — Read, create, list, and natively search your entire note library to pull exact context into your AI conversations seamlessly.
- **Task Execution** — Query specific pending to-dos, update task states, or rapidly create new tasks within specific notes without leaving the chat.
- **Tag Management** — Dynamically list and analyze the tag hierarchy of your Amplenote system, keeping the AI aware of your organizational framework.
- **Action Tracking** — Instruct the agent to invoke native Amplenote actions, maintaining deep synchronization between the AI and your existing mental models.

### How it works

1. Install this integration in your active workspace.
2. Provide your secure Amplenote Personal Access Token.
3. Converse directly with your ideas via Claude, Cursor, or any compatible agent.

### Who is this for?

- **Knowledge Workers** — command the agent to search your older research notes and synthesize a brand new outline for an upcoming essay.
- **Project Leads** — easily ask the AI to check all your incomplete tasks tagged with `#urgent` and formulate an execution plan for today.
- **Developers in Flow** — quickly dump meeting minutes or architecture concepts securely into Amplenote through your IDE agent without breaking deep work.


## Available Tools (12)
- **list_notes**: Use as the primary way to browse the entire knowledge base.

List all notes in the Amplenote workspace
- **search_notes**: Use when the user wants to find content by keyword.

Full-text search across all Amplenote notes and tasks
- **list_tasks**: Returns task content, completion status, due dates, and parent note references. Use for task management overview.

List all tasks across all notes
- **get_task**: Use to inspect or update a single task.

Retrieve a specific task by its ID
- **create_task**: Tasks in Amplenote live inside notes and have due dates, priorities, and completion tracking. Use for adding actionable items.

Create a new task
- **update_task**: Use for task progress tracking and management.

Update a task content, completion status, or other properties
- **list_tags**: Returns tag names and usage counts. Use to discover the knowledge taxonomy.

List all tags used across notes and tasks
- **get_note_actions**: Use to discover what operations can be performed on a note.

Retrieve available actions for a specific note
- **get_note**: Essential for reading or analyzing a specific document.

Retrieve the full content and metadata of a specific note by UUID
- **create_note**: Use for adding documentation, meeting notes, or project plans.

Create a new note with a title and Markdown body content
- **update_note**: Use for editing content, fixing errors, or appending information.

Update an existing note title and/or Markdown body by UUID
- **delete_note**: Permanently delete a note by UUID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amplenote** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new note titled 'Project Alpha Planning' and assign it the tag '#work/projects'."

**🤖 AI Agent:**
> Note successfully created! The note ID is `62h28d-9b19` and you can access it inside the `#work/projects` framework. Would you like me to start populating it with an initial brainstorm structure?

---

**👤 You:**
> "Search my Amplenote vault for all active tasks containing the word 'Budget'."

**🤖 AI Agent:**
> I found 3 tasks matching 'Budget' across your notes:
1. Revise Q3 Marketing Budget (Inside Note: 'Q3 Objectives')
2. Consolidate AWS cloud budget anomalies (Inside Note: 'Daily Ops')
3. Send budget approval to Sarah (Inside Note: 'To-do Master')
Shall I mark the last one as complete?

---

**👤 You:**
> "Get the content of my 'Weekly Sync' note."

**🤖 AI Agent:**
> Here is the content of 'Weekly Sync' (UUID: 8a93-11bb):

# Updates
- Engineering launched v2.1
- Support tickets down 5%

### Blockers
There are minor bottlenecks with the primary database query speeds. Mark is investigating.

Would you like me to inject a new task for Mark to summarize his database findings by Friday?


## ❓ FAQ

**Q: Can the agent interact with specific individual tasks within my notes?**
Yes. Amplenote's integration treats tasks as distinct manageable objects. You can not only list the pending items inside a note but also ask the agent to complete them, update their content, or inject an entirely new to-do row directly inside.

**Q: How does searching work across hundreds of deeply tagged notes?**
The integration utilizes Amplenote's robust search protocol. You simply tell the agent to 'find notes containing strategy tagged with #work/2026', and it will parse your complex nested structures efficiently without blindly guessing.

**Q: Can I trust the AI agent to update existing notes without wiping the rest of the text?**
Absolutely. Under the hood, the integration exposes granular update capabilities where the agent carefully dictates new structural alterations. It will append or replace specific regions accurately without overwriting unrelated brainstorming details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amplenote](https://vinkius.com/mcp/amplenote)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amplenote** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amplenote` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amplenote** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amplenote": {
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
