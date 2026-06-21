# BugHerd MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bugherd-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage BugHerd projects, tasks, and comments through AI Agents.

## Description
### O que você pode fazer
- Create and list your BugHerd projects.
- Manage tasks seamlessly inside projects.
- Retrieve, add, and monitor comments on specific bug tasks.
- View all members within your BugHerd workspace.

### Como funciona
1. Install the BugHerd MCP Server on your Vinkius Edge.
2. Add your personal BugHerd API key in the credentials page.
3. Empower your AI agent to fetch bugs, add comments, and triage tickets naturally via chat.

### Para quem é?
Ideal for development and QA teams looking to interact with BugHerd tickets directly via Cursor, Claude, or any MCP-enabled agent. Turn your AI into a full-fledged QA assistant.


## Available Tools
- **add_comment**: Add a comment to a BugHerd task
- **create_project**: Create a new project in BugHerd
- **create_task**: Create a new task in a BugHerd project
- **get_project**: Get a specific project in BugHerd
- **get_task**: Get a specific task in BugHerd
- **list_comments**: List comments on a BugHerd task
- **list_projects**: List projects in BugHerd
- **list_tasks**: List tasks for a project in BugHerd
- **list_users**: List users in the BugHerd account
- **update_task**: Can update description, status, priority, or assigned_to_id.

Update a task in BugHerd


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BugHerd** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in BugHerd."

**🤖 AI Agent:**
> Here are your active BugHerd projects...

---

**👤 You:**
> "Create a new bug task in project 123 saying 'Login button is broken'."

**🤖 AI Agent:**
> I've successfully created the new bug task for the broken login button.

---

**👤 You:**
> "Read the comments on task 456 in project 123."

**🤖 AI Agent:**
> Fetching comments for task 456...


## ❓ FAQ

**Q: Can the AI Agent resolve or close a task automatically?**
Yes, using the `update_task` tool, the agent can change the task status to 'closed' or 'done' within BugHerd.

**Q: Are attachments or screenshots supported?**
Currently, the MCP Server manages text-based tasks, comments, and project structures. Adding direct screenshot files via AI is not supported in this version.

**Q: Can I read comments from any ticket?**
Yes! The agent can fetch and read all comments attached to a specific task using the `list_comments` tool, provided you supply the Project ID and Task ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bugherd-alternative](https://vinkius.com/mcp/bugherd-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BugHerd** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bugherd-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BugHerd** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bugherd-alternative": {
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
