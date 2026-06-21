# Capsule CRM MCP Server

Manage contacts, sales opportunities, and projects via Capsule CRM — search parties, track pipelines, and manage tasks directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/capsule-crm-alternative)

## Overview
**Category:** sales-automation
**Tools Count:** 31

## Description
Connect your **Capsule CRM** account to any AI agent to streamline your sales and relationship management workflows through natural conversation.

### What you can do

- **Contact Management** — List, search, and retrieve detailed profiles for people and organizations (Parties) using `search_parties` and `get_party`.
- **Sales Pipeline** — Track opportunities, update milestones, and manage your sales funnel with `list_opportunities` and `update_opportunity`.
- **Project Tracking** — Oversee projects from inception to completion with `list_projects` and `get_project`.
- **Task & Activity Logging** — Create and manage tasks, and view history entries with `list_tasks` and `list_entity_entries` to keep track of every interaction.
- **Customization** — Access tags and custom fields via `list_tags` and `list_custom_fields` to maintain your specific business data structure.

### How it works

1. Subscribe to this server
2. Enter your Capsule CRM Personal Access Token
3. Start managing your CRM data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — quickly update opportunity status and add notes after calls without leaving the chat interface.
- **Account Managers** — retrieve full contact history and background info before meetings.
- **Project Leads** — monitor project progress and task completion across the organization.


## Available Tools
- **create_entry**: Create a new note entry
- **create_opportunity**: Create a new opportunity
- **create_party**: Create a new party (person or organisation)
- **create_project**: Create a new project (kase)
- **create_task**: Create a new task
- **delete_opportunity**: Delete an opportunity
- **delete_party**: Delete a party
- **delete_project**: Delete a project (kase)
- **delete_task**: Delete a task
- **get_current_user**: Show the authenticated user
- **get_opportunity**: Get details for a specific opportunity
- **get_party**: Get details for a specific party
- **get_project**: Get details for a specific project (kase)
- **get_task**: Get details for a specific task
- **list_custom_fields**: List custom field definitions for parties, opportunities, or kases
- **list_deleted_parties**: List deleted parties since a specific date
- **list_entity_entries**: List entries for a specific party, project, or opportunity
- **list_entries**: List recent entries (notes & emails)
- **list_opportunities**: List all opportunities
- **list_parties**: List all parties (people and organisations)
- **list_projects**: List all projects (kases)
- **list_tags**: List tag definitions for parties, opportunities, or kases
- **list_tasks**: List tasks (default: open)
- **list_teams**: List all teams
- **list_users**: List all users
- **search_opportunities**: Search for opportunities
- **search_parties**: Search for parties
- **update_opportunity**: Update an existing opportunity
- **update_party**: Update an existing party
- **update_project**: Update an existing project (kase)
- **update_task**: Update an existing task


## Installation & Usage

To install and use the **Capsule CRM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/capsule-crm-alternative](https://vinkius.com/mcp/capsule-crm-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
