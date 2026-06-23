# Fieldwire MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fieldwire)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Manage construction projects via Fieldwire — track tasks, organize floorplans, and coordinate field teams directly from any AI agent.

## Description
Connect your **Fieldwire** account to any AI agent to streamline your construction management workflows through natural conversation.

### What you can do

- **Project Oversight** — List all active projects and fetch detailed metadata for specific construction sites.
- **Task Management** — Create, update, and query tasks. Monitor progress, assign owners, and update statuses like 'In Progress' or 'Completed'.
- **Floorplan Organization** — List project floorplans and manage them in batches, including moving them to specific collections for better site organization.
- **Field Communication** — Access 'task bubbles' to retrieve comments, photos, and media attachments linked to specific site issues.
- **Team Coordination** — Invite new users to your account and list all personnel assigned to specific projects to ensure proper resource allocation.

### How it works

1. Subscribe to this server
2. Enter your Fieldwire API Token
3. Start managing your jobsite from Claude, Cursor, or any MCP-compatible client

No more switching between mobile apps and desktop browsers to check the status of a floorplan or a specific task. Your AI acts as a digital foreman or project coordinator.

### Who is this for?

- **Project Managers** — Instantly retrieve site statuses, list pending tasks, and coordinate team members without leaving your workflow.
- **Superintendents & Foremen** — Check task descriptions, media attachments, and floorplan locations straight from the field or office.
- **Specialty Contractors** — Update task progress and review site comments to stay aligned with the general contractor's schedule.


## Available Tools (17)
- **add_aws_post_tokens**: Generate AWS POST tokens for uploading files
- **batch_move_floorplans**: Move floorplans to collections
- **batch_update_statuses**: Batch create, update, or delete task statuses
- **create_project**: Create a new Fieldwire project
- **create_sheet_upload**: Create a sheet upload after uploading to S3
- **create_task**: Create a new task in a Fieldwire project
- **enable_collections**: Enable collections for floorplans in a project
- **get_form_full**: If a job is triggered, it returns a jid. Call again with the jid to poll until the full JSON payload is returned.

Get full data for a form (triggers job or polls)
- **get_project**: Get details for a specific Fieldwire project
- **invite_user**: Invite a user to the Fieldwire account
- **list_floorplans**: List floorplans in a Fieldwire project
- **list_project_users**: List users in a Fieldwire project
- **list_projects**: List all projects in the Fieldwire account
- **list_statuses**: Get custom task statuses for a project
- **list_task_bubbles**: Get comments and media (bubbles) for a task
- **list_tasks**: List tasks in a Fieldwire project
- **update_task**: Update an existing Fieldwire task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fieldwire** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects in my Fieldwire account."

**🤖 AI Agent:**
> I've found 3 active projects: 'Downtown Plaza' (UUID: ...), 'Westside Bridge' (UUID: ...), and 'City Hospital' (UUID: ...). Which one would you like to explore?

---

**👤 You:**
> "Create a new task 'Fix leak in Room 302' in project [UUID]."

**🤖 AI Agent:**
> Task 'Fix leak in Room 302' has been successfully created in the project. The Task UUID is 8829-abc. Would you like to assign it to a user?

---

**👤 You:**
> "Show me the comments and photos for task [UUID] in project [UUID]."

**🤖 AI Agent:**
> I've retrieved the task bubbles. There are 2 comments: 'Leak identified' and 'Parts ordered', along with one photo attachment showing the pipe damage.


## ❓ FAQ

**Q: Can I see photos and comments attached to a specific task?**
Yes! Use the `list_task_bubbles` tool with the Project and Task UUIDs. It retrieves all messages, photos, and files attached to that specific task.

**Q: How do I organize multiple floorplans into a collection?**
You can use `batch_move_floorplans` to move an array of floorplan UUIDs into a target collection. Make sure to use `enable_collections` first if they aren't active for the project.

**Q: Is it possible to invite new team members to my Fieldwire account via AI?**
Yes, the `invite_user` tool allows you to send an invitation to a user's email address directly from the agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fieldwire](https://vinkius.com/mcp/fieldwire)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fieldwire** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fieldwire` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fieldwire** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fieldwire": {
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
