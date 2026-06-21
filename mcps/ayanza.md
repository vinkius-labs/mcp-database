# Ayanza MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ayanza)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

AI-powered project management and team collaboration — manage tasks, projects, and wikis via AI.

## Description
Orchestrate your team's rhythm with **Ayanza**, the AI-first project management platform designed for modern velocity. By connecting Ayanza to your AI agent, you transform project oversight from a manual chore into a natural conversation. Your agent gains the power to navigate complex task workflows, access team wikis, and manage project milestones without you ever opening a dashboard. It’s not just about tracking tasks; it’s about giving your agent the context it needs to act as a digital coordinator within your workspace.

### What you can do

- **Task Orchestration** — List, create, update, and delete tasks in Ayanza using natural language through your AI agent.
- **Project Oversight** — Get a comprehensive view of all projects or dive into specific project details to monitor progress effortlessly.
- **Knowledge Retrieval** — Access and list wiki pages to quickly find team documentation and shared knowledge.
- **Workspace Management** — View workspace users to understand team structure and assign tasks effectively.
- **Dynamic Updates** — Modify task descriptions and statuses in real-time to keep your team aligned and productive.

### How it works

1. Subscribe to this server
2. Enter your Ayanza API Token
3. Start managing your workspace from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — automate task status updates and get instant summaries of project health
- **Engineering Teams** — access technical documentation in the wiki and manage sprint tasks via chat
- **Operations Leads** — maintain workspace cleanliness by updating or removing outdated tasks via AI
- **Knowledge Workers** — quickly retrieve team guides and project context without leaving your primary workflow


## Available Tools (10)
- **create_task**: Create a new task in Ayanza
- **delete_task**: Delete an Ayanza task
- **get_me**: Get current authenticated user info
- **get_project**: Get details for a specific Ayanza project
- **get_task**: Get details for a specific Ayanza task
- **list_projects**: List projects in Ayanza
- **list_tasks**: List tasks in Ayanza
- **list_users**: List users in the Ayanza workspace
- **list_wiki_pages**: List wiki pages in Ayanza
- **update_task**: Update an existing Ayanza task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ayanza** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my tasks in Ayanza."

**🤖 AI Agent:**
> I've retrieved your tasks from Ayanza. You have 5 active tasks, including 'Prepare Q4 presentation' and 'Review team goals'. Would you like me to update the status of any of these?

---

**👤 You:**
> "Create a new task called 'Prepare Q4 presentation'."

**🤖 AI Agent:**
> Task 'Prepare Q4 presentation' has been successfully created in Ayanza. I've set it to the default status. Would you like me to add a description or assign it to a project?

---

**👤 You:**
> "Show my wiki pages in Ayanza."

**🤖 AI Agent:**
> I've listed your Ayanza wiki pages. You have access to 'Onboarding Guide', 'Tech Specs', and 'Marketing Strategy'. Which page would you like me to read for you?


## ❓ FAQ

**Q: Can my AI agent create tasks in specific Ayanza projects?**
Yes! Your agent can list all projects to find the correct ID and then create tasks directly within that project context.

**Q: Is it possible to recover deleted tasks via the AI agent?**
Currently, the MCP server supports the deletion of tasks, but recovery must be handled directly within the Ayanza web interface.

**Q: Can the agent access private wiki pages?**
The AI agent can only access wiki pages that are visible to the user associated with the provided API token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ayanza](https://vinkius.com/mcp/ayanza)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ayanza** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ayanza` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ayanza** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ayanza": {
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
