# Zammad MCP Server

Automate helpdesk workflows via Zammad — manage tickets, users, and organizations directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zammad)

## Overview
**Category:** communication-messaging
**Tools Count:** 41

## Description
Connect your **Zammad** helpdesk to any AI agent to streamline your customer support and user management through natural conversation.

### What you can do

- **Ticket Management** — List, retrieve, and create tickets to stay on top of customer requests using `list_tickets` and `get_ticket`.
- **User & Organization Control** — Search, create, and update user profiles and organizational data with tools like `search_users` and `list_organizations`.
- **Group & Role Insights** — List and search through system groups and roles to understand permissions and assignments.
- **Data Privacy** — Securely handle user deletions via specialized data privacy tasks using `data_privacy_delete_user`.

### How it works

1. Subscribe to this server
2. Enter your Zammad URL and Personal Access Token
3. Start managing your helpdesk from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Leads** — quickly get ticket statuses and user history without switching tabs.
- **System Admins** — manage users, groups, and organizations directly from the terminal or AI interface.
- **DevOps Engineers** — integrate helpdesk data into automated workflows and reporting.


## Available Tools
- **add_tag**: Add a tag to an object
- **create_ticket_article**: Create a new article on a ticket
- **create_ticket**: Create a new Zammad ticket
- **create_user**: Create a new Zammad user
- **data_privacy_delete_user**: Delete a user via Data Privacy task (Recommended over direct delete)
- **delete_ticket**: Delete a Zammad ticket
- **delete_user**: Delete a Zammad user
- **get_group**: Get details for a specific Zammad group
- **get_links**: Get links for a specific object
- **get_me**: Get current Zammad user details
- **get_organization**: Get details for a specific Zammad organization
- **get_shared_draft**: Get shared draft for a ticket
- **get_ticket_article**: Get details for a specific ticket article
- **get_ticket**: Get details for a specific Zammad ticket
- **get_user**: Get details for a specific Zammad user
- **list_all_tags**: List all tags in the system (Admin)
- **list_calendars**: List calendars
- **list_checklist_items**: List checklist items
- **list_checklist_templates**: List checklist templates
- **list_checklists**: List checklists
- **list_groups**: List all Zammad groups
- **list_mentions**: List mentions
- **list_organizations**: List all Zammad organizations
- **list_roles**: List all Zammad roles
- **list_slas**: List SLAs
- **list_tags_for_object**: List tags for a specific object (e.g., Ticket)
- **list_ticket_articles**: List articles for a specific ticket
- **list_ticket_priorities**: List ticket priorities
- **list_ticket_states**: List ticket states
- **list_tickets**: List Zammad tickets
- **list_time_accountings**: List time accountings for a ticket
- **list_users**: List all Zammad users
- **remove_tag**: Remove a tag from an object
- **search_groups**: Search for groups in Zammad
- **search_organizations**: Search for organizations in Zammad
- **search_roles**: Search for roles in Zammad
- **search_tickets**: Search for tickets in Zammad
- **search_users**: Search for users in Zammad
- **summarize_ticket**: Trigger async generation of a ticket summary
- **update_ticket**: Update an existing Zammad ticket
- **update_user**: Update an existing Zammad user


## Installation & Usage

To install and use the **Zammad** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zammad](https://vinkius.com/mcp/zammad)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
