# Fieldwire MCP Server

Manage construction projects via Fieldwire — track tasks, organize floorplans, and coordinate field teams directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fieldwire)

## Overview
**Category:** construction
**Tools Count:** 17

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


## Available Tools
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


## Installation & Usage

To install and use the **Fieldwire** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fieldwire](https://vinkius.com/mcp/fieldwire)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
