# ProofHub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/proofhub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Empower your AI agent to manage your ProofHub projects — list tasks, create to-dos, read discussions, and track timesheets instantly.

## Description
Connect your **ProofHub** domain to any AI agent to streamline project management and team collaboration directly from your workflow.

### What you can do

- **Project Overviews** — Retrieve all active projects, detailed metadata, and overarching status instantly
- **Task & To-do Management** — Fetch to-do lists, see assigned tasks, and even create new work items on the fly
- **Team Collaboration** — Read project discussions, track newly uploaded files, and access shared notebooks and documentation
- **Resource Management** — List all team members, check active statuses, and audit logged hours and productivity via timesheets

### How it works

1. Subscribe to this server
2. Provide your ProofHub Domain and API Key
3. Start collaborating and managing your team workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — easily pull up task progress and project statuses without digging through boards
- **Team Leads** — audit timesheets, verify team availability, and read recent discussions in plain text
- **Remote Teams** — create quick to-dos and check shared files seamlessly from your AI chat


## Available Tools (10)
- **list_projects**: ProofHub is a collaboration tool with tasks, discussions, and files.

Lists all projects in ProofHub
- **get_project**: Retrieves full details of a ProofHub project
- **list_todolists**: Use this to find the correct list ID before querying or creating tasks.

Lists all to-do lists within a ProofHub project
- **list_tasks**: Lists all tasks in a ProofHub to-do list
- **create_task**: You must provide a valid project ID and todolist ID.

Creates a new task in a ProofHub to-do list
- **list_discussions**: Lists all discussions (topics) in a ProofHub project
- **list_files**: Lists all files uploaded to a ProofHub project
- **list_people**: Lists all team members in ProofHub
- **list_notes**: Lists all notes/notebooks in a ProofHub project
- **list_timesheets**: Lists all timesheet entries for a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ProofHub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects on ProofHub right now."

**🤖 AI Agent:**
> You have 4 active projects. The main ones are 'Q4 Marketing Campaign' (ID: 102) and 'Website Overhaul' (ID: 105). Would you like to dig into the tasks or timesheets for any of these?

---

**👤 You:**
> "Check the to-do list for 'Website Overhaul' and show what's pending."

**🤖 AI Agent:**
> For 'Website Overhaul', the main To-Do list (ID: 201) has 3 pending tasks: 
1. Optimize hero images
2. Fix CSS spacing on mobile
3. Write FAQ section
Should I create a new task to add to this list?

---

**👤 You:**
> "Create a task in project 105 (todolist 201) to 'Test checkout flow'."

**🤖 AI Agent:**
> Task 'Test checkout flow' has been successfully created in the selected To-Do list for the Website Overhaul project. Your team will see it instantly.


## ❓ FAQ

**Q: How do I connect my account?**
Subscribe and provide two things: your **ProofHub Domain** (the 'mycompany' part of `mycompany.proofhub.com`) and your **API Key**. The API Key is somewhat hidden: log into ProofHub, click your profile picture in the bottom-left corner 5 times straight to reveal the 'API access' option, then generate or copy your key.

**Q: Can my agent create tasks directly?**
Yes! Just tell your agent the project name (or ID), the to-do list, and the title of the task you want created. It will use the `create_task` tool to instantly drop that work item into the specified ProofHub list for your team to pick up.

**Q: How can I see what the team has been discussing?**
Ask your agent to 'list discussions for project X'. It retrieves all recent discussion topics securely, allowing you to stay in the loop on project blockers, decisions, and brainstorming without opening multiple communication tabs.

**Q: Can this server pull files and notes?**
Yes. Beyond tasks, the agent can query both `list_files` and `list_notes` for any given project ID. If someone uploaded project requirements or drafted meeting notes, your AI assistant can surface their metadata and context on demand.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/proofhub](https://vinkius.com/mcp/proofhub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ProofHub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `proofhub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ProofHub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "proofhub": {
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
